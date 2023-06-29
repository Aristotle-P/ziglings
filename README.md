# Ziglings
My personal repo for ziglings to track my progress and move between machines. If you're interested in Ziglings and learning Zig yourself please visit the official [repo here](https://github.com/ratfactor/ziglings/)

## Getting Started

Install a [development build](https://ziglang.org/download/) of
the Zig compiler.  (See the "master" section of the downloads
page.)

Verify the installation and build number of `zig` like so:

```
$ zig version
0.11.0-dev.3853+xxxxxxxxx
```

Clone this repository with Git:

```
$ git clone https://github.com/ratfactor/ziglings
$ cd ziglings
```

Then run `zig build` and follow the instructions to begin!

```
$ zig build
```

Note: The output of Ziglings is the unaltered output from the Zig
compiler. Part of the purpose of Ziglings is to acclimate you to
reading these.

## Advanced Usage

It can be handy to check just a single exercise or _start_ from a
single exercise:

```
zig build -Dn=19
zig build -Dn=19 start
```

You can also run without checking for correctness:

```
zig build -Dn=19 test
```

Or skip the build system entirely and interact directly with the
compiler if you're into that sort of thing:

```
zig run exercises/001_hello.zig
```

Calling all wizards: To prepare an executable for debugging,
install it to zig-cache/bin with:

```
zig build -Dn=19 install
```

To get a list of all possible options, run:

```
zig build -Dn=19 -l

  install          Install 019_functions2.zig to prefix path
  uninstall        Uninstall 019_functions2.zig from prefix path
  test             Run 019_functions2.zig without checking output
  ...
```

