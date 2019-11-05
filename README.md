# opencart-composer-extension-test
A test Composer package for installing a simple extension in OpenCart by automatically copying the files.

### Installation:

1. `composer require composer require themreza/opencart-composer-extension-test dev-master`
2. `composer require sasedev/composer-plugin-filecopier`
3. Add this to your OpenCart's composer.json, and make sure to change the destination to match your upload/public folder:

```
"extra": {
        "filescopier": [
            {
                "source": "vendor/themreza/opencart-composer-extension-test/src",
                "destination": "upload",
                "debug": "true"
            }
        ]
    }    
```
