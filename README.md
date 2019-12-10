#Documentation
can be fount in ./Latex/report.pdf
#How to test the script
To test laboratory.html you have to host in a web-server all these files:

	laboratory.html
	interpolizer.js
	N45E007.hgt
	N45E008.hgt

Hosting in a web-server is necessary otherwise modern browsers block
local file reading requests for security reasons and N45E007.hgt
and N45E008.hgt will not be accessible for laboratory.html anymore.

Older firefox relises and Microsoft edge should open laboratory.html
even if not hosted by a web-server (tested on 14/07/2019).
Microsoft edge is pretty slower than firefox. So when testing the script
wait a couple of minutes even if the browser seems to be frozen and
don't close the browser window.

When 45E007.hgt and N45E008.hgt access is blocked a cone with all red
spots will be displayed. No errors will be displayed by the browsers
if the debug console is not enabled.

A cone with all red spots will be also displayed if out-of-bound
sample requests are made to 45E007.hgt and N45E008.hgt. So, basically,
test the script only in Torino's bounds. Authomathic geolocalization
service will outomatically infer out-of-bounds requests if the script
is run out of Turin.
