ui: platform-native GUI library for Go
Update 5 June 2016: You can FINALLY go get this package!
go get should work out of the box for the following configurations:

darwin/amd64
linux/386
linux/amd64
linux/arm (only tested on a Raspberry Pi 2)
windows/386
windows/amd64
Everything is now fully static — no DLLs or shared objects anymore!

Note that these might not fully work right now, as the libui Alpha 3.1 API isn't fully implemented yet, and there might be residual binding problems. Hopefully none which require an Alpha 3.2...

New README
This is a library that aims to provide simple GUI software development in Go.

It is based on my libui, a simple cross-platform library that does the same thing, but written in C. You must include this library in your binary distributions.

It runs on/requires:

Windows: cgo, Windows Vista SP2 with Platform Update and newer
Mac OS X: cgo, Mac OS X 10.8 and newer
other Unixes: cgo, GTK+ 3.10 and newer
It also requires Go 1.6 or newer (due to various bugs in cgo that were fixed only starting with 1.6).

(this README needs some work)

Installation
