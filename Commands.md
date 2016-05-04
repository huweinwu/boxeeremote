# Introduction #

XBMC and Boxee support a set of remote commands. For example, to get information about the currently playing track, I visit http://localhost:8800/xbmcCmds/xbmcHttp?command=getcurrentlyplaying() (or a different IP/host if boxee isn't on your local machine).

The key to adding functionality to the remote is to see if there's something you can do with these commands that would make sense as a feature of the remote. Sometimes you need to do more than one command. For example, to change the volume, we do a getvolume(), add or subtract from that, and then do, say, setvolume(80).

Play around with these commands and let me know which you think would make good features. Be sure to try them out and see if they work like you think, though, as not all of the commands are straightforward.


# Details #

| **command** | **XBMC/Boxee Action** | **In remote app?** |
|:------------|:----------------------|:-------------------|
| action      |                       |                    |
| addtoplaylist |                       |                    |
| addtoslideshow |                       |                    |
| broadcast   |                       |                    |
| broadcastlevel |                       |                    |
| choosealbum |                       |                    |
| clearplaylist |                       |                    |
| clearslideshow |                       |                    |
| config      |                       |                    |
| copyfile    |                       |                    |
| deletefile  |                       |                    |
| downloadinternetfile |                       |                    |
| execbuiltin |                       |                    |
| exit        |                       |                    |
| filecopy    |                       |                    |
| filedelete  |                       |                    |
| filedownload |                       |                    |
| filedownloadfrominternet |                       |                    |
| fileexists  |                       |                    |
| filesize    |                       |                    |
| fileupload  |                       |                    |
| getbroadcast |                       |                    |
| getcurrentlyplaying | information about the current track | used to display thumbnail and duration |
| getcurrentplaylist |                       |                    |
| getcurrentslide |                       |                    |
| getdirectory |                       |                    |
| getguidescription |                       |                    |
| getguisetting |                       |                    |
| getguistatus |                       |                    |
| getkeyboardtext |                       |                    |
| getloglevel |                       |                    |
| getmediaitems |                       |                    |
| getmedialocation |                       |                    |
| getmoviedetails |                       |                    |
| getmusiclabel |                       |                    |
| getpercentage |                       |                    |
| getplaylistcontents |                       |                    |
| getplaylistlength |                       |                    |
| getplaylistsong |                       |                    |
| getplayspeed |                       |                    |
| getrecordstatus |                       |                    |
| getshares   |                       |                    |
| getslideshowcontents |                       |                    |
| getsysteminfo |                       |                    |
| getsysteminfobyname |                       |                    |
| gettagfromfilename |                       |                    |
| getthumb    |                       |                    |
| getthumbfilename |                       |                    |
| getthumbnail | get base64-encoded thumbnail image | used to display thumbnail|
| getvideolabel |                       |                    |
| getvolume() | return volume percent `[0, 100]` | first step of volume buttons|
| getxbeid    |                       |                    |
| getxbetitle |                       |                    |
| guisetting  |                       |                    |
| help        |                       |                    |
| keyrepeat   |                       |                    |
| lookupalbum |                       |                    |
| move        |                       |                    |
| mute        |                       |                    |
| pause       |                       |                    |
| playfile    |                       |                    |
| playlistnext |                       |                    |
| playlistprev |                       |                    |
| playnext    |                       |                    |
| playprev    |                       |                    |
| playslideshow |                       |                    |
| querymusicdatabase |                       |                    |
| queryvideodatabase |                       |                    |
| removefromplaylist |                       |                    |
| reset       |                       |                    |
| restart     |                       |                    |
| restartapp  |                       |                    |
| rotate      |                       |                    |
| seekpercentage |                       |                    |
| seekpercentagerelative |                       |                    |
| sendkey     | send a keycode        | used for most buttons and trackball |
| setautogetpicturethumbs |                       |                    |
| setbroadcast |                       |                    |
| setcurrentplaylist |                       |                    |
| setfile     |                       |                    |
| setguisetting |                       |                    |
| setkey      | same as sendkey       |                    |
| setloglevel |                       |                    |
| setplaylistsong |                       |                    |
| setplayspeed |                       |                    |
| setresponseformat |                       |                    |
| setvolume(x) | set volume, x in `[0, 100]` | second step of volume buttons|
| showpicture |                       |                    |
| shutdown    |                       |                    |
| slideshowselect |                       |                    |
| spindownharddisk |                       |                    |
| stop        |                       |                    |
| takescreenshot |                       |                    |
| webserverstatus |                       |                    |
| zoom        |                       |                    |