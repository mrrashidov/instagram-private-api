----------
## Installation

### Dependencies

Install/enable the required php extensions and dependencies. You can learn how to do so [here](https://github.com/shoxruxrashidov/instagram-private-api/wiki/Dependencies).

### Install this library
We use composer to distribute our code effectively and easily. If you do not already have composer installed, you can download and install it here [here](https://getcomposer.org/download/).

Once you have composer installed, you can do the following:
```sh
composer require shoxrux/instagram-private-php
```

```php
require __DIR__.'/../vendor/autoload.php';

$ig = new \InstagramAPI\Instagram();
```

If you want to test new and possibly unstable code that is in the master branch, and which hasn't yet been released, then you can do the following (at your own risk):

```sh
composer require shoxrux/instagram-private-php dev-master
```

#### _Warning about moving data to a different server_

_Composer checks your system's capabilities and selects libraries based on your **current** machine (where you are running the `composer` command). So if you run Composer on machine `A` to install this library, it will check machine `A`'s capabilities and will install libraries appropriate for that machine (such as installing the PHP 7+ versions of various libraries). If you then move your whole installation to machine `B` instead, it **will not work** unless machine `B` has the **exact** same capabilities (same or higher PHP version and PHP extensions)! Therefore, you should **always** run the Composer-command on your intended target machine instead of your local machine._

## Examples

All examples can be found [here](https://github.com/shoxruxrashidov/instagram-private-api/tree/master/examples).
