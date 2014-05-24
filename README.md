# Kex

Kex is a Kerl inspirexd tool to easy building and installing of [Elixir](http://elixir-lang.org) instancs.

## Downloading

You can download the script directly from github:

```
$ curl -O https://raw.githubusercontent.com/glejeune/kex/master/kex
```

Then ensure it is executable

```
$ chmod a+x kerl
```

and drop it in your `$PATH`

## Usage

`kex list` : list availables releases

`kex install <version>` : install version `<version>`

`kex update` : update

`. ~/.kex/insalls/<version>/activate` : Use version `<version>`

