# Textmate Bundle for Buster.JS

## Common snippets

Important: For now you have to install Dr. Nic's JavaScript Node bundle, then 
change your current grammar to "JavaScript Node" (short cut: Shift+Ctrl+Alt+N)

* tc => scaffolding for a new testCase
* tcc => additional testCase
* tt => additional test
* ntc => nested test case
* setup => setup method
* assert snippets
  * ase - assert.equals(...)
  * asf - assert.isFunction(...)
  * aso - assert.isObject(...)
  * asc - assert.called(...)
  * ascw - assert.calledWith(...)
  * asnc - assert.notCalled(...)
  * asco - assert.calledOnce(...)
  * asex - assert.exception(...)

## Installation

    mkdir -p ~/Library/Application\ Support/TextMate/Bundles/
    cd ~/Library/Application\ Support/TextMate/Bundles
    git clone git://github.com/magnars/buster.tmbundle.git "Buster.tmbundle"
    osascript -e 'tell app "TextMate" to reload bundles'

Alternately, in TextMate, from your drop down menu, select Bundles -> Bundle Editor -> Reload Bundles.

## Credits

The Buster.JS TM Bundle is currently authored by Magnar Sveen. Contributors and co-maintainers are welcome.

* **Magnar Sveen** - Author/Main contributor

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
