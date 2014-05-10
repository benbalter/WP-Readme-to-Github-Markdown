# WP2MD

Convert WordPress Plugin Readme Files to GitHub Flavored Markdown

## Features

* Converts headings
* Formats contributors, donate link, etc.
* Inserts screenshots

## Usage

CLI:

    # with files as params
    wp2md convert -i readme.txt -o README.md
    # or with unix pipes
    wp2md convert < readme.txt > README.md


PHP:

```php
$markdown = \SunChaser\WP2MD\Converter::Convert($readme);
```

## Installation

### Composer (recommended)

Add a composer dependency to your project:

    "require-dev": {
        "sunchaser/wp2md": "*"
    }

The binary will be ```vendor/bin/wp2md```

### Download binary

You may install WP2MD binary globally

    sudo wget http://code.sunchaser.info/wp2md/downloads/wp2md.phar /usr/local/bin/wp2md
    sudo chmod a+x /usr/local/bin/wp2md
