# requirejs-anonymous-define

There are two files:

**_requirejs-anonymous-define.html_**
  This is the mail file. It's an HTML file. It has two buttons:
    ### On Demand Require:
      On clicking this button, a library code is loaded using requirejs to print "On Demand require working" in the console. If we see that text in console, it means requrejs is working as expected
    ### Load Anonymous Define:
      On cliking this button, an external JS is loaded that is defined by the constant SCRIPT_HAVING_ANONYMOUS_DEFINE

**_anonymous-define.js_**
  This is an JS file that has a anonymous define that when loaded causes requirejs to throw error

## To use this POC:
- Load the page probably using http-server
- Should see the console log _Page loaded_
- Click on _On Demand Require_ button. Should see console log of _On Demand require working_
- Click on _Load Anonymous Define_ button. The file defined by SCRIPT_HAVING_ANONYMOUS_DEFINE const variable should get loaded and a console log _Anonymous Define Loaded_ should be seen
- Click on _On Demand Require_ button. Console error denoting anonymous define gets displayed
- Consequent click of _On Demand Require_ works fine

This tool can be used to test that the file loaded using SCRIPT_HAVING_ANONYMOUS_DEFINE works fine without the anonymous define error.
