BrowserUpdateWarning
===========

A browser update warning plugin for Moo Tools. 

Dependencies
------------

- MooTools Core v1.4.4


How to use
----------

**Include mootools framework and BrowserUpdateWarning plugin**

	<script src="path-to-mootools-framework" type="text/javascript"></script>
	<script src="path-to-browser-update-warning-js" type="text/javascript"></script>

**Include BrowserUpdateWarning stylesheet**

	<link href="path-to-browser-update-warning-css" type="text/css" rel="stylesheet" />

**Example 1**

Shows basic usage.

Javascript:

	window.addEvent('domready', function() {
		
		var browserWarning = new BrowserUpdateWarning();
		
		browserWarning.check();
	}
	
**Example 2**

Example with options

Javascript:

	window.addEvent('domready', function() {
	
		var browserWarning = new BrowserUpdateWarning({
		
			// Custom Images Directory
			imagesDirectory: 'ui/js/mootools.BrowserUpdateWarning/Source/images/',
			
			// Example minimum version override
			minVersion_safari: 6,
			
			// Opacity for shade div over content
			opacity: 30,
			
			// Show Continue to site button
			allowContinue: true
			
		});
		
		browserWarning.check();
	}


Screenshot
-----------------

![Screenshot](http://andyfleming.com/code/browser-update-warning-for-mootools/images/screenshot-1.png)

Please report bugs, errors and advices in the github project page: https://github.com/andyfleming/BrowserUpdateWarning


Terms & Conditions
-----
 
BrowserUpdateWarning
Copyright 2012 Andy Fleming

This copyright notice and permission notice shall be included in
all copies of the Software, in part or as a whole.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.