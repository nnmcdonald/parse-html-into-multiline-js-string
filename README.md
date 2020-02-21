# parse-html-into-multiline-js-string
HTML template for parsing html into javascript ES5 multiline string

I found myself needing to create a multiline string from a lot of HTML for the purposes of dynamic
form creation. It was necessary to create a multiline string that was compliant with ES5,
therefore I created this template to display the parsed text in the browser.

Just place the code you would like to parse into the div with id="parse"
Then open the file in your browser, copy and paste text

This script uses single quotes in the generated multiline string, 
to change to double quotes set:

  single_quotes=false;

in the footer script
