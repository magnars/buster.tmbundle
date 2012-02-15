# Textmate Bundle for Buster.JS

## Commands

* cmd+shift+r => Run all tests

## Common snippets

* tc => new testCase (one for node, browser and node+browser)
* tt => additional test
* cx => nested context
* su => setup method
* td => teardown method

Assert and refute snippets follow a common pattern. They start with `as` or `re`
the a mnemonic shortcut. Most are simply the 'initials' of the method name, but
the best shortcuts are saved for the most common assertions.

    ase - assert.equals
    asm - assert.match

    asc1 - assert.calledOnce
    asc2 - assert.calledTwice
    asc3 - assert.calledThrice
    ascw - assert.calledWith
    ascn - assert.className
    astn - assert.tagName
    asx - assert.exception
    asd - assert.defined
    asid - assert.inDelta
    asif - assert.isFunction
    asin - assert.isNull
    asio - assert.isObject

    ass - assert.same
    asto - assert.typeOf
    ast - assert.threw
    asat - assert.alwaysThrew
    asc - assert.called
    ascc - assert.callCount
    asco - assert.callOrder
    asco - assert.calledOn
    asaco - assert.alwaysCalledOn
    asacw - assert.alwaysCalledWith
    asacwe - assert.alwaysCalledWithExactly
    ascwe - assert.calledWithExactly

Refute mirrors assert exactly, except that they start with `re` instead of
`as`. It's the beauty of symmetry.

## Prerequisites

* Buster.js has to be installed.
* The shell script for the `Run all tests` command has to find node in PATH. To ensure this either update your `~/.MacOSX/environment.plist` or set the PATH variable in TextMates Preferences/Advanced/Shell Variables accordingly. See the [TextMate manual](http://manual.macromates.com/en/shell_commands#search_path) for details.
* The shell script for the `Run all tests` command requires `buster/node_modules/buster-test-cli`. To ensure this add a Shell Variable `NODE_PATH` referencing your node modules in TextMates Preferences/Advanced/Shell Variables, e.g. to `/usr/local/lib/node_modules`.

## Installation

    mkdir -p ~/Library/Application\ Support/TextMate/Bundles/
    cd ~/Library/Application\ Support/TextMate/Bundles
    git clone git://github.com/magnars/buster.tmbundle.git "Buster.tmbundle"

Then reload your bundles:

    osascript -e 'tell app "TextMate" to reload bundles'

Alternately, in TextMate, from your drop down menu, select Bundles -> Bundle Editor -> Reload Bundles.

## Credits

The Buster.JS TM Bundle is currently authored by Magnar Sveen. Contributors and co-maintainers are welcome.

* **Magnar Sveen** - Author/Main contributor
* **Stefan Scheidt** - Improved support for multiple platforms
* **Thomas Pickert** - Added some more snippets

## License

Copyright (c) 2011 Magnar Sveen, Norway

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
