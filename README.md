This repository is one of the ways to go through the English Version of [Linux Journey](https://linuxjourney.com) Course - https://linuxvoyage.github.io/

### Based on

* [Linux Journey](https://github.com/cindyq/linuxjourney/) is a site dedicated to making learning Linux fun and easy.

* [LunaGNUisance/linuxjourney](https://github.com/LunaGNUisance/linuxjourney) for ordering the content.

* [web.archive.org](https://web.archive.org/web/20220706072307/https://linuxjourney.com/) for copying the original site's styles

* [itamarg365/linuxjourney](https://github.com/itamarg365/linuxjourney) for helping to serve locally.

### Usage - Serve the MD lessons with python3 app

#### From your machine:
```bash
pip install -r requirements.txt
cd src
uvicorn main:app
```
#### From a typical container:
To serve from container, you might need to specify host address and port as
 1. running uvicorn will try to host at 127.0.0.1 which did not work while testing out of container
 2. you might have port 80 occupied for some other project.
```bash
uvicorn main:app --host 0.0.0.0 --port 9090
```
And...
![](./images/site.png "Website")



### Brief History

Though Linux Journey was created to document the journey of the [original author](https://github.com/cindyq) and their contributors to learn Linux, everyone's journey is a little different. So, One fine day, the linuxjourney.com website went down and open source community was concerned. Hence, someone volunteered to help us serve it locally and then put it together as static site. After over 2 months, it seems the domain owner/author of the site, resurrected it up again.  So, Now We can further improve the knowledge of the greater Linux community through contribution and collaboration, again. Feel free to refer to below issues and may be make a contribution or PR. Good day!

#### Related GitHub Issues:
* [213](https://github.com/cindyq/linuxjourney/issues/213#issuecomment-1420893647)
* [216](https://github.com/cindyq/linuxjourney/issues/216)


### License
The text content of this repo (Linux Journey) has been made free to modify and distribute. For full license terms see: [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/). This license does not include the images, site design and source code which is subject to All Rights Reserved.