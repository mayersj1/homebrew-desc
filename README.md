# brew-desc.rb - Searchable descriptions for Homebrew formulas

## What is it?

It's an [external
command](https://github.com/mxcl/homebrew/wiki/External-Commands) for
[Homebrew](https://github.com/mxcl/homebrew). It provides short
descriptions for many Homebrew packages, and I hope to eventually include
*all* Homebrew packages. You can also search for packages by description.

## Usage

If you already know the name of a package, and you want to see a bit about
it, that's easy:

    $ brew desc mutt
    mutt: Mongrel of Mail User Agents (part Elm, Pine, Mush, mh, etc)

If you know the kind of thing you're interested in, but not the name of
specific items, that's easy too:

    $ brew desc -s key-value
    redis: A persistent key-value database with built-in net interface
    kumofs: A scalable and highly available distributed key-value store
    cassandra: Highly scalable, eventually consistent, distributed key-value store

Both `-s` and `--search` are acceptable. Searches are always case
insensitive. (Notice that as a Homebrew [external
command](https://github.com/mxcl/homebrew/wiki/External-Commands), you
invoke the script as `brew desc`.)

## Installation

You can now install `brew desc` in two ways.

1. Tap this repository and install via `brew` itself.
1. Install manually.

For the first method, do the following:

    brew tap telemachus/homebrew-desc && brew install brew-desc

For the second method clone or download this repository. Then simply put
the file `brew-desc.rb` anywhere in your `$PATH`. For example:

    mv brew-desc.rb ~/bin

Leave the name as is if you follow this method. Homebrew knows how to find
it.

Once you've installed via either method, you can use the command as
described above.

## Contributors

+ [Sietse de Kaper](https://github.com/targeter)
+ [Max Nordlund](https://github.com/maxnordlund)
+ [Humza Yaqoob](https://github.com/secondplanet)
+ [Zearin](https://github.com/Zearin)

## Contributing

I started this project with the descriptions from the
[MacPorts](http://www.macports.org/) ports tree. I edited those, and since
then have added names and blank descriptions for many more Homebrew
packages. However, there are still many, many items without descriptions.

Please fork, add descriptions (or edit the ones already here) and send
a pull request. Thanks.
