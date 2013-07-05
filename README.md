Domgrep
=======

Domgrep is a tool to query for stuff from the internet.
It has two modes: "normal" mode and "interactive" mode. 

Normal usage example:

    # This lists all the hrefs of a elements on Google
    ./domgrep "http://www.google.com" -s a -a href 
    # This lists the inner text of all a elements on google whose hrefs include the string "authuser".
    ./domgrep "http://www.google.com" -s a --regex authuser --regex-attr href 

If you run domgrep with just a URL as an argument, it will fetch the URL and display a prompt "&gt;".
Here, you can enter a CSS selector and see what matches. 
When you get matches, you can enter an attribute to be displayed (default: the raw HTML will be shown).

More information is available by running domgrep --help, or by reading the source code :)

 --Cian
