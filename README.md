functx-pkg
==========

Package builder for the [FunctX](http://functx.com/) library.

This project is used to create a package out of FunctX.  It does not
contain the sources of FunctX themselves, but needs them to be built.
Just copy both [XSLT](http://xsltfunctions.com/xsl/download.html) and
[XQuery](http://xqueryfunctions.com/xq/download.html) sources to
`src/content/` before building this project (do not check them in!).

As we do not want to modify FunctX sources, we cannot add the public
import URIs within the source files themselves, so we cannot use
XProject and we need to provide an explicit `expath-pkg.xml`
descriptor.  Look into `build/Makefile` for build instructions
(normally just invoking `make` in that directory is all you need).
