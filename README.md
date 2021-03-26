# consolidation/robo binary

## Installation

```php
php -r "copy('https://github.com/drupol/robo-shim/releases/latest/download/robo.phar', 'robo.phar');"
php -r "copy('https://github.com/drupol/robo-shim/releases/latest/download/robo.phar.sha1sum', 'robo.phar.sha1sum');"
php -r "if (hash_file('sha1', 'robo.phar') === file_get_contents('robo.phar.sha1sum')) { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('robo.phar');unlink('robo.phar.sha1sum');} echo PHP_EOL;"
rm robo.phar.sha1sum
chmod +x robo.phar
```
