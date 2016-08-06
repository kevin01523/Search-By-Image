Search-By-Image
===============

Search By Image | attempt to search map

Attempt to search a script map. With this script, you can quickly search for pictures.

Alternate Download:
> Https://greasyfork.org/scripts/2998-search-by-image
>
> Http://ext.ccloli.com/search-by-image/search-by-image.user.js

Instructions:
> * Search Image: Hold down the shortcut key (default Ctrl key) while clicking the right mouse button on the image, select To use the search engine in the menu
>
> * Upload Search: Hold down the shortcut key (default Ctrl key), while the non-image Click the right mouse button and select wish to use a search engine (version 1.4) upload pictures in the menu after clicking <br> transit schedule cancellation upload, after upload pictures stored in temporary transit server for search engines to crawl <br> uploads include the following (only support a single file)
>
>> * Click on "upload photos and search for" and select the file
>>
>> * Drag and drop files to the menu within
>>
>> * Press Ctrl + V to paste the clipboard in the image (not support Firefox, for unknown reasons)
>>
>> * Also search base64 form also need to upload image
>
> * Setup script: Hold down the shortcut key (default Ctrl key) while clicking the right mouse button and select the menu "Setting" to open the settings screen <br> or select "Search By Image Setting" in the user script command set to open <br> interface can be changed in the settings page, add, delete, search engines, configuration and reset settings "multi search" and shortcuts
>
>> * Change search engine: "Name" field to specify the name of the search engine, "Address" field specified search engine by calling the map (picture address {% s} instead)
>>
>> * Add a search engine: Click the "Add Item" button to add a search engine
>>
>> * Remove search engine: Click the right side of the search engine "×" to delete the search engine
>>
>> * Set Multi-search: Check the "Multi Search" box and saved, the search picture click "All" will open all check the "Multi Search" search engine
>>
>> * Change Shortcut: In the "HotKey" at the lower left corner of the search can be modified exhaled menu shortcuts
>>
>> * Reset settings: Click the "Reset" button to reset all settings (irreversible)
>>
>> * Save Settings: Click the "Save" button to save your settings
>
> * Modify the transit server: In the script, line 47 (subject to change) find server_url, needed to be modified (after the update also need to re-set), related presentations are listed in the script
>
> Using each interface, please refer to the following preview

Default support Web site:
> * Google
> * Baidu knowledge map
> * Baidu Photos
> * Bing
> * TinEye
> * Яндекс (Yandex)
> * Sogou
> 360 *
> * SauceNAO
> * IQDB
> * 3D IQDB

Internal Test:
> * 864907600cc (ccloli)
> * Arts (wenketel)

The script is based on the open source GPLv3 agreement http://www.gnu.org/licenses/gpl.html

! [Search menu] (https://cloud.githubusercontent.com/assets/8115912/3623778/b6d76498-0e53-11e4-96a0-09488c053e44.png)
! [Setting screen] (https://cloud.githubusercontent.com/assets/8115912/3623779/b734b490-0e53-11e4-9250-66707699db6e.png)

Additional explanation:
> First, the script can only search img tag images for css background-image anything, huh = =
>
> Secondly, because facilitate the design, it is estimated there are a lot of web design page image or picture dynamic effect, it will add a transparent layer above the image, this is also not get the picture = =
>
> In addition, when searching paste it in the picture, if you search the url situation appears to base64, see this post: http: //tieba.baidu.com/p/3145502558

Update History:
> 2015.12.27 1.4.11 GreasyFork feedback [# 7547] (https://greasyfork.org/zh-CN/forum/discussion/7547/x) search menu in the window beyond the visual size of its lower edge, press and hold click Search menu hotkey will open in a background tab, the tab will open in the foreground when pressed
>
> 2015.12.02 1.4.10 Fixed GreasyFork feedback [# 6806] (https://greasyfork.org/en/forum/discussion/6806/x) (not working on old Firefox), update most of default search engines url to HTTPS
>
> 2015.08.15 1.4.9 add multi-language support, and there is no use, there is nothing to add and use a custom upload server settings, repair repair 1.4.6 Menu Bar Menu Bar dislocation dislocation cause problems
>
> 2015.05.01 1.4.8 fixes Baidu Image Search is unavailable problems (See issue # 3)
>
> 2015.04.06 1.4.7 fixes in some visual editor (eg. MDN WYSIWYG editor) bug legacy menu appears (Thanks to lychichem, see issue http://tieba.baidu.com/p/3682475061)
>
> 2015.04.05 1.4.6 fixes exist when the body margin menu bar misalignment problem, repair the problem on a version of the mouse after the style has not entered into force, Яндекс (Yandex) default name to Yandex
>
> 2014.09.05 1.4.5 Adds mouse through the style options (I admit I'm lazy OTL)
>
> 2014.08.14 1.4.4 fixes still be closed when not in operation panel outgoing panel tries to repair GM 2.x under GM_registerMenuCommand conflict
>
> 2014.07.26 1.4.3 Adding transit upload server (Thanks to Retaker), modify the upload server is set up, Firefox tries to repair the problem can not be pasted uploaded
>
> 2014.07.18 1.4.2 fixes can not click the Settings button in the non-image problem exhaled search menu
>
> 2014.07.06 1.4.1.1 fixes the bug can not be uploaded
>
> 1.4.1 2014.07.06 pop removal notice (may frequently pop up in Firefox), add additional transit upload server (need to manually modify the script)
>
> 2014.07.06 1.4 supports upload image search, image search support base64 (transit upload)
>
> 2014.07.05 1.3.8 specification syntax changes and more search engines search the opening sequence, add base64 base64 address judgment and refused to search form images (known as search engines do not support)
>
> 2014.07.04 1.3.7 tries to repair the conflict under Chrome Tampermonkey script with other listeners mouse actions
>
> Add 360 2014.07.04 1.3.6 and 3D IQDB, repair a tab settings After modifying the settings in other tabs are not updated question (this version will overwrite the settings)
>
> 2014.07.04 1.3.5 modification of the wrong title
>
> 2014.07.04 Script 1.3.4 released
>
> Search menu 2014.07.04 1.3.3 fixes the problem of inaccurate positioning
>
> 2014.07.04 1.3.2 fix some bug
>
> 2014.07.04 1.3.1 fixes for failing to fill in a blank search engine option problems
>
> 2014.07.03 1.3 Add setting menu
>
> 2014.07.03 1.2.1 fix some bug
>
> 1.2 2014.07.03 added shortcut set (to be modified within the script)
>
> 2014.07.03 1.1 Add search menu
>
> 1.0 2014.07.03 start writing scripts, and complete the basic functions
