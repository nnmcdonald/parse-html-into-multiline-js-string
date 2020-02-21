# parse-html-into-multiline-js-string
HTML template for parsing html into javascript ES5 multiline string

I found myself needing to create a multiline string from a lot of HTML for the purposes of dynamic
form creation. It was necessary to create a multiline string that was compliant with ES5,
therefore I created this template to display the parsed text in the browser.

NOTE: If the exact string "CREATE_NEW_LINE" appears in the HTML to be parsed THIS WILL NOT WORK!
      You must replace 'CREATE_NEW_LINE' in the following:
        var lines = stringToParse.replace(/(\r\n|\n|\r)/gm, 'CREATE_NEW_LINE').split('CREATE_NEW_LINE');
      with an unique identifier that does not appear in the HTML

Just place the code you would like to parse into the div with id="parse"
Then open the file in your browser, copy and paste text

This script uses single quotes in the generated multiline string, 
to change to double quotes set:

  single_quotes=false;

in the footer script
