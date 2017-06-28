# TorrentBar

Script for showing users statistics (upload, download, ratio) of torrent trackers based on Torrent Pier.

### Installation

1. Unpack to some folder on your server, for example here:
     http://127.0.0.1/torrentpier/torrentbar/
2. Then edit public/index.php. Add the right path to TorrentPier configuration file ($torrentpier_config_path), for example:
     `$torrentpier_config_path = "/home/localhost/www/torrentpier/forum/config.php";`
   or like this:
     `$torrentpier_config_path = "../forum/config.php";`
3. (OPTIONAL) Change some other variables in Presets area or view Templates folder
   to create new templates.
4. Installation Complete :)

------------------------------------------------------------------------------

### Usage

After that, just add to your signature (on Forum):  
  (Without .htaccess)  
    `[img]http://127.0.0.1/torrentbar/public/{user_id}.png[/img]`  
  or  
    `[img]http://127.0.0.1/torrentbar/public?id={user_id}[/img]`  
    `[img]http://127.0.0.1/torrentbar/public?id={user_id}&style={style_name}[/img]`  

  (With .htaccess)  
    `[img]http://127.0.0.1/torrentbar/public/{user_id}-{style_name}.png[/img]`  

Where `{user_id}` is your ID on Forum and `{style_name}` is the name of template.  

How to find out your ID? Easy :) Just click on your profile and look at the address bar:  
    `http://127.0.0.1/torrentpier/forum/profile.php?mode=viewprofile&u=2` (*2* is my ID)
