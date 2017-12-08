# Modified PHPWord

This is only Modified PHPWord library based on PHPOffice/PHPWord library. I just put some modification in Word TemplateProcessor to recognize Images as a Template in the Document.

Thank you

## Installation
This library is installed via [Composer](https://getcomposer.org/).
To [add a dependency](https://getcomposer.org/doc/04-schema.md#package-links>) to PHPWord in your project, either

Run the following to use the latest master version
```sh
    composer require phpoffice/phpword:dev-master
```
You can of course also manually edit your composer.json file
```json
{
    "require": {
       "superipey/phpword": "dev-master"
    }
}
```

## Getting Started
First Step
-------
To try this library modification, first create the template with the image placed anywhere in your document, right click on the image, then select **Format AutoShape/Pictures**
![Figure 1](https://uymikg.bn1303.livefilestore.com/y4mpp0pGKTovYVCBRtu5jGJifUJtgu3iNjn0gvEnackzvYnlau-I9J2xhNDcQgvg5oKSACYGAyXGLj5drcLc2MsaQ5UiAruq_ui5VW7X6pUBOSNf-_1Vch68MfV_hRDo2pxrvI7JHY6XFdcHDEklfWgPduzVeRYANnw98blAWIYXY4BMrRrQXAmuaRYxS6NP3y1WMiCibZPC-63Y_FPyGQy7w?width=660&height=371&cropmode=none "Figure 1")

Second Step
-------
Type your fieldname in the **Alternative text**
![Figure 2](https://vcmikg.bn1303.livefilestore.com/y4mT5pV8FNSwsyN6YLfv0rSl3-aiF66-ncFYfISlICokoa76uZ-sbYAZnnNZ9MJpthW3XnuiH4bjjVJlatM5tEpOMzGcOgFtFEbGJm8KNC6GMQocfjUbfsK7QwVwIOg9iWFj0zadiTb-JadgdyyhMB0asydmUI3A4yTRIWFuAmQJ3ik6822YB0nmPqeSzUwcCv5FmkQDt_iuyOzKZJy2nxMWA?width=586&height=660&cropmode=none "Figure 2")

Third Step
-------
Use **setImageValueAlt** to set the image
```php
$template->setImageValueAlt(field, path-to-file);
```
Example:
```php
$template->setImageValueAlt("foto", "./uploads/foto/ferry.png");
```

## License

PHPWord is an open source project licensed under the terms of LGPL version 3. PHPWord is aimed to be a high quality software product by incorporating continuous integration and unit testing. You can learn more about PHPWord by reading the Developers' Documentation and the API Documentation.
