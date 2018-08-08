*******************************************************************
*                                                                 *
* | |_| |__   ___    /\  /\__ _ _ ____   _____  ___| |_ ___ _ __  *
* | __| '_ \ / _ \  / /_/ / _` | '__\ \ / / _ \/ __| __/ _ \ '__| *
* | |_| | | |  __/ / __  / (_| | |   \ V /  __/\__ \ ||  __/ |    *
*  \__|_| |_|\___| \/ /_/ \__,_|_|    \_/ \___||___/\__\___|_|    *
*                                                                 *
<<<<<<< HEAD:README.md
* TheHarvester Ver. 3.0.0                                         *
=======
* TheHarvester Ver. 3.0                                           *
>>>>>>> cd5580925e8ec10714acf3bf02c23686e4fb93e0:README
* Coded by Christian Martorella                                   *
* Edge-Security Research                                          *
* cmartorella@edge-security.com                                   *
*******************************************************************

What is this?
-------------

theHarvester is a tool for gathering subdomain names, e-mail addresses, virtual
hosts, open ports/ banners, and employee names from different public sources
(search engines, pgp key servers).

Is a really simple tool, but very effective for the early stages of a penetration
test or just to know the visibility of your company in the Internet.

The sources are:

**Passive**:
---------

-threatcrowd: Open source threat intelligence - https://www.threatcrowd.org/

-crtsh: Comodo Certificate search - www.crt.sh

-google: google search engine  - www.google.com

-googleCSE: google custom search engine

-google-profiles: google search engine, specific search for Google profiles

-bing: microsoft search engine  - www.bing.com

-bingapi: microsoft search engine, through the API (you need to add your Key in
          the discovery/bingsearch.py file)

-dogpile: Dogpile search engine - www.dogpile.com

-pgp: pgp key server - mit.edu

-linkedin: google search engine, specific search for Linkedin users


-vhost: Bing virtual hosts search

-twitter: twitter accounts related to an specific domain (uses google search)

-googleplus: users that works in target company (uses google search)

-yahoo: Yahoo search engine

-baidu: Baidu search engine

-shodan: Shodan Computer search engine, will search for ports and banner of the
         discovered hosts  (http://www.shodanhq.com/)


Active:
-------
-Port scanning and takeover options: this option will create connection to the hosts discovererd
-DNS brute force: this plugin will run a dictionary brute force enumeration
-DNS reverse lookup: reverse lookup of ip´s discovered in order to find hostnames
-DNS TDL expansion: TLD dictionary brute force enumeration


Modules that need API keys to work:
----------------------------------
-googleCSE: You need to create a Google Custom Search engine(CSE), and add your
 Google API key and CSE ID in the plugin (discovery/googleCSE.py)
-shodan: You need to provide your API key in discovery/shodansearch.py


Dependencies:
------------
-Requests library (http://docs.python-requests.org/en/latest/)
`pip install requests`


Changelog in 3.0.0:
------------------
-Subdomain takeover checks
-Port scanning (basic)
-Improved DNS dictionary


Changelog in 2.7.2:
------------------
-Added threatcrowd
-Added IP resolution for all results
-Basic local storage of results using Sqlite (WIP)


<<<<<<< HEAD:README.md
=======
Changelog in 2.7.1:
------------------
-Added Virustotal, Netcraft, Crt.sh engines


>>>>>>> cd5580925e8ec10714acf3bf02c23686e4fb93e0:README
Comments? Bugs? Requests?
------------------------
cmartorella@edge-security.com

Updates:
--------
https://github.com/laramies/theHarvester

Thanks:
-------
John Matherly -  SHODAN project
Lee Baird for suggestions and bugs reporting
Ahmed Aboul Ela - subdomain names dictionary (big and small)
