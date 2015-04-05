**Q:**  There is a typo in the project name "transmisson-remote-gui". It should be "transmiss<font color='red'><b>i</b></font>on-remote-gui". Was it made for purpose?

**A:** Unfortunately, the typo was made during creation of the project on Google Code. The only way to fix it is to delete the current project and create a new project. The typo was noticed too late.

**Q:** Is it possible to run transgui directly from a USB stick?

**A:** Yes. Just create a folder on your USB stick and copy there the **transgui** executable file (and, optionally, the **lang** folder). Then create empty **transgui.ini** file in that folder. Now you can run the transgui executable directly from the USB stick. All settings will be stored at the stick as well.


**Q:** Is it possible to run several instances of the program?

**A:** Yes. By default, transgui stores all it's settings in the user's profile. To run an extra instance of the program, you need to explicitly specify some other folder to store the program's settings. To do that, pass the **`--home=<home_dir>`** parameter. Where `<home_dir>` is some folder where the program's settings of the new instance will be stored.

**Q:** What mean numbers like 4/28 in the Seeds column?

**A:** Seeds: 4/28:
  * 4 - number of peers, from which we are downloading now (connected seeders).
  * 28 - total number of available peers, which have this torrent (available seeders).

**Q:** What mean numbers like 2/7 in the Peers column?

**A:** Peers: 2/7:
  * 2 - number of peers, which are downloading from us (connected leechers).
  * 7 - total number of downloading peers on the tracker (total number of leechers).

**Q:** What's the meaning of an icon with red arrow (up or down) in the names column?

**A:** A red icon indicates a error. To find out the error message, look at the "Error" in the General page at the bottom of the main window.

**Q:** What is path mapping?

**A:** Path mappings are used to convert a remote path (on a computer where a Transmission daemon is running) to a local path (local computer where Transmission Remote GUI is running). And vice versa. The mappings are used to open remote files and folders. The path mappings are configured in the **Connection options** on the **Paths** page.

For example, your torrents are downloaded into the `/var/pub/downloads` folder by a Transmission daemon running on a NAS. You access the daemon from a Windows PC using Transmission Remote GUI. You have network access to the `/var/pub` folder on the NAS as network drive `K:`. In that case you should specify the following path mapping:

`/var/pub/downloads=K:\downloads`

If you can access the `/var/pub` folder using a UNC path such as `\\nas\pub`, then use the following path mapping:

`/var/pub/downloads=\\nas\pub\downloads`