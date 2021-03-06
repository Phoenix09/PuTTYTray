# PuTTYTray

This is [PuTTYTray][1], a fork of [Simon Tatham's PuTTY][2].

## Usage

See [usage instructions][6] in our wiki.

## Documentation

* For a list of current features, see the [PuTTYTray website][1].
* The [github wiki][3] has documentation for some of these features, and help for other things, including contributing.
* Please feel free to report any problems or feature requests using the [github issue tracker][5].

## Aims

There are a lot of patches against PuTTY that have never been submitted to, or have been rejected from, upstream.  PuTTYTray is collecting these, with the aim of eventually getting them merged back in.

I'm looking to take ownership of any patches that are:

* Cool or useful to someone, even if that someone is just you,
* Maintainable against the PuTTY code; i.e. mostly independent with some hooks or appends to some functionality,
* Are at least vaguely following the original design goals of PuTTY, and follow the coding style a bit, and
* Not security related, or, at least, there not being any visible security risk.  PuTTY is a security product, and the security is critical.  I want everyone, even very paranoid people, to be able to use PuTTYTray.


## Building

Visual Studio 2010 project files are included.  These should **just work**, there are absolutely no dependencies beyond what Visual Studio ships; even the Express edition works fine.  There is a [full walkthrough of building PuTTYTray][4] on the wiki.

The original build system for PuTTY is intact, i.e. you can run `perl mkfiles.pl` and it will regenerate all the other build systems, including VS6 and various flavours of makefiles.

My released builds are still done with VS2010's `nmake` (using `windows/build-release.bat`), and will continue to be done so until XP drops out of support.

## License

This compilation is released under the same license as PuTTY itself;
the MIT license. Individual contributions may be copyrighted by the original authors.

See `LICENSE.MIT` for the full text.


  [1]: https://puttytray.goeswhere.com/
  [2]: http://www.chiark.greenend.org.uk/~sgtatham/putty/
  [3]: https://github.com/FauxFaux/PuTTYTray/wiki
  [4]: https://github.com/FauxFaux/PuTTYTray/wiki/Building-with-VS2010-Express
  [5]: https://github.com/FauxFaux/PuTTYTray/issues
  [6]: https://github.com/FauxFaux/PuTTYTray/wiki/Usage-instructions
