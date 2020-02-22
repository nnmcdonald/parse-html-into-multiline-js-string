# parse-html-into-multiline-js-string
HTML template for parsing html into javascript ES5 multiline string

I found myself needing to create a string on multiple lines from a lot of HTML for the purposes of dynamic
form creation. For example:

var html_as_string = "<form>"+
"&ltul>"+
"&ltli>"+
"&ltli>"+
"&lt/ul>"+
"&ltform>";


It was necessary to be compliant with ES5,
therefore I created this template to display the parsed text in the browser.

NOTE: If the exact string "CREATE_NEW_LINE" appears in the HTML to be parsed THIS WILL NOT WORK!
      You must replace 'CREATE_NEW_LINE' in the following:
        var lines = stringToParse.replace(/(\r\n|\n|\r)/gm, 'CREATE_NEW_LINE').split('CREATE_NEW_LINE');
      with an unique identifier that does not appear in the HTML

Just place the code you would like to parse into the div with id="parse"
Then open the file in your browser

This script uses single quotes in the generated multiline string, 
to change to double quotes set:

  single_quotes=false;

in the footer script
