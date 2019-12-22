# Extension migration
Before version 1.1.0 it is necessary to replace the Pagekit class with Biskuit.

## Example
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
