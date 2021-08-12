# cli-markdown

[![License](https://img.shields.io/packagist/l/phpcom-lab/cli-markdown.svg?style=flat-square)](LICENSE)
[![Php Version](https://img.shields.io/badge/php-%3E=7.2.0-brightgreen.svg?maxAge=2592000)](https://packagist.org/packages/phpcom-lab/cli-markdown)
[![GitHub tag (latest SemVer)](https://img.shields.io/github/tag/phpcom-lab/cli-markdown)](https://github.com/phpcom-lab/cli-markdown)
[![Actions Status](https://github.com/phpcom-lab/cli-markdown/workflows/Unit-Tests/badge.svg)](https://github.com/phpcom-lab/cli-markdown/actions)

Render colored markdown contents on console terminal

**Preview**

![demo](example/demo.png)

## Features

- support auto render color on terminal
- support custom set cli color tags

## Install

**composer**

```bash
composer require phpcom-lab/cli-markdown
```

## Usage

quick usage:

```php
<?php

use PhpComLab\CliMarkdown\CliMarkdown;

require dirname(__DIR__) . '/vendor/autoload.php';

$contents = file_get_contents(dirname(__DIR__) . '/README.md');
$praser = new CliMarkdown;

$rendered = $praser->render($contents);

echo $rendered;
```

## Base on

package | description
---------|--------------
`cebe/markdown` | parse markdown contents
`toolkit/cli-utils` | provide cli color render

## License

[MIT](LICENSE)
