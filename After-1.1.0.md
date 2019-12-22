# Extension migration
After 1.1.0 version it is necessary to replace the Pagekit class with Biskuit and move from pagekit-extension to biskuit-extension.

## Class migration
From biskuit/blog extension:
```
...
use Biskuit\Application as App;
...
use Biskuit\User\Model\Role;
...
```
The difference with the original Pagekit extension is the use of the Biskuit class instead of Pagekit:
```
...
use Pagekit\Application as App;
...
use Pagekit\User\Model\Role;
...
```
## Extension type migration
With the introduction of the new Marketplace, the types of extensions change to:
* biskuit-extension
* biskuit-theme
This wording needs to be updated in the composer.json file:
```
...
"type": "biskuit-extension",
...
```

A complete example is available [here](https://github.com/biskuitorg/biskuit/tree/master/packages/biskuit/blog).
