# Blackberry OG Themes
CSS changes to many popular home theater services. Flat and minimal, cleans up unneeded clutter, and fixes many UI issues on desktop. In the case of Plex, it creates a whole new mobile interface (WebUI and video player), and modifies the desktop UI to better fit within OrganizrV2. For those who do not want OrganizrV2 specific view enhancements such as hiding the user icon, please use [Improved Plex Mobile CSS](https://github.com/Archmonger/Improved-Plex-Mobile-CSS). 

**Installation**
<br/>For services that don't allow native CSS themes, you can edit your Nginx configuration to add in the CSS. One method is to download the CSS to your root directory and href it. This can be accomplished with sub_filter (http_sub_module). 
```
sub_filter '</head>' '<link rel="stylesheet" type="text/css" href="https://mydomain.com/css/PlexMobile.css"> </head>';
sub_filter_once on;
```
Another option available is to use [rawgit.com](https://rawgit.com) to host the CSS file for you.

**Screenshots**
<br/>Images are available within the repo's `Screenshots` folder.

**More Information**

| Service | Last Tested Version | Requires Nginx Subfilter |
| ------------- | :-------------: | :-------------: |
| Plex | 1.13.5.5332 | YES |
| Ombi | 3.0.3477 | NO |
| Synclounge | 2.0.0 | YES |
| Filebrowser | 1.9.0  | NO |
