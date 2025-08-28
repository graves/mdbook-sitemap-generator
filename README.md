# mdbook-sitemap-generator
## What is this?
mdbook-sitemap-generator is a simple utility to generate sitemap.xml files for mdbook projects.

## Installation

```
git clone https://github.com/graves/mdbook-sitemap-generator
cargo install .
```

## Usage
The utility should be run from the root of the project.
```
USAGE:
    mdbook-sitemap-generator [OPTIONS] --domain <DOMAIN>

OPTIONS:
    -d, --domain <DOMAIN>
    -h, --help               Print help information
    -o, --output <OUTPUT>
```

When running the utility, you must pass the site's domain on URL via the `-d` flag, for example, `-d docs.example.com`.

If the `-o` flag is not passed, the sitemap will be written to stdout.

For example:
```
$ ls
book  book.toml  src
$ mdbook-sitemap-generator -d docs.example.com -o book/sitemap.xml

```
