# HTTPS Proxy for data.gov.uk organogram visualisation

This is a temporary work around to proxy a non-HTTPS resource to allow us to
move to using HTTPS without getting mixed content errors. The proxy responds to
both HTTP and HTTPS requests and can be used in the iframe that the visualisation
is displayed in using a protocol-relative link.

`organogram.js` has been modified to make the links protocol-relative to allow
the organograms page to be served as HTTP or HTTPS.

The original code can be found here:

https://github.com/UKGovLD/linked-data-api

# Installation instructions

`secure-reference.conf` should be installed in the standard Nginx configuration file locations.

`organogram.js` should be put in `/var/www/secure-reference/gov-structure/scripts/`.
