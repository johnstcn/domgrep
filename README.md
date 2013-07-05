Domgrep is a tool to query for stuff from the internet.
It has two modes: "normal" mode and "interactive" mode. 

Normal usage example:
./domgrep "http://www.google.com" -s a -a href # This lists all the hrefs of a elements on Google
./domgrep "http://www.google.com" -s a --regex authuser --regex-attr href # This lists the inner text of all a elements on google whose hrefs include the string "authuser".

More information is available by running domgrep --help, or by reading the source code :)
