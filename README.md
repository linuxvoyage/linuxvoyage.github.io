This is a clean way to go through the English Version of Linux Journey Course - https://linuxvoyage.github.io/

## Based on

* [Linux Journey](https://linuxjourney.com) was a site dedicated to making learning Linux fun and easy.

* [LunaGNUisance/linuxjourney](https://github.com/LunaGNUisance/linuxjourney) for ordering the content.

* [web.archive.org](https://web.archive.org/web/20220706072307/https://linuxjourney.com/) for copying the original site's styles

* [itamarg365/linuxjourney](https://github.com/itamarg365/linuxjourney) for helping to serve locally.



### Usage - To Serve Locally via container or
```bash
pip install -r requirements.txt
cd src
uvicorn main:app

# To serve from container, you might need to specify host address and port as
# 1. running uvicorn will try to host at 127.0.0.1 which did not work while testing out of container
# 2. you might have port 80 occupied for some other project.
uvicorn main:app --host 0.0.0.0 --port 9090
```
And...
![](./images/site.png "Website")



### License

Though Linux Journey was created to document the journey of the [original author](https://github.com/cindyq) and their contributors to learn Linux, everyone's journey is a little different. So, We can further improve the knowledge of the greater Linux community through contribution and collaboration.


### License
The text content of Linux Journey has been made free to modify and distribute. For full license terms see: [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/). This license does not include the images, site design and source code which is subject to All Rights Reserved.