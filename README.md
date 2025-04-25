# SlicerMorph102
## Introduction to 3D Morphometrics with SlicerMorph

<!-- ## Course Evaluation: please go to  https://forms.gle/cK3stUy8XigeXJTb9 to fill the course evaluation form. -->


### Course Prerequisites

If you do not already have them, please obtain accounts at:
* https://github.com
* https://orcid.org.
  
GitHub and ORCID are mandatory to use MorphoCloud. 
  
Also you will **need a 3-button mouse (cannot emphasize this enough)** to operate 3D Slicer (or any other 3D software) effectively. Optionally, [install the latest preview version (v5.9) of Slicer.](https://download.slicer.org) on your own computer as a backup, in case you have issues with cloud connections. 

Finally, having a second monitor is advised, since that will allow you to keep your zoom and cloud sessions on separate screens. 

### MorphoCloud On Demand
You should have received an email from me with your access credentials to your MorphoCloud On Demand instance. We will use a special version of our regular instances that will allow us to keep all the instances online through out the course. There is no need to shelve or unshelve these instances, or extend the session. They will be available 24/7 throughout the course. These instances will be deleted promptly after the course. Should you like to continue using the MorphoCloud (which we hope you do), you can request a new instance at https://instance.morpho.cloud

Some important points about MorphoCloud On Demand sessions:
* Use the `CTRL(CMD in Mac) + ALT + SHIFT` combination to make the cloud connection side window visible (or to make it disappear, if visible).
* For best user experience, switch to full screen mode in your browser window (not advisable if you do not have a second monitor, as you won't be able to see the zoom window).

#### MorphoCloud Desktop
- **A:** Side toolbar that gets activated by pressing the `CTRL (or CMD)` +
  `ALT` + `SHIFT` keys. It allows copy/paste into the remote session, browse and
  download files on the remote drive and adjust screen zoom levels (cut from the
  screenshot).
- **B:** Shortcuts to commonly used applications and to **MyData** storage
  volume.

- **C:** Displays list of available applications (searchable)

- **D:** Right mouse clicking anywhere on desktop brings this menu, including
  changing screen resolution (Display settings).

- **E:** Click on this icon anytime to extend your session for additional 4
  hours.

<p align="center">
  <img src="https://github.com/MorphoCloud/MorphoCloudInstances/blob/main/MCI_Desktop.png" />
</p>

#### Mapping the Sample Data Drive
Remember the course sample data is available under **/media/shares/MorphoCloudCephShare/SlicerMorph102**</br>
This path should already mapped to your instance, however, if any reason it is not there, you can put this command in a terminal window. 

```
curl https://jetstream2.exosphere.app/exosphere/assets/scripts/mount_ceph.py | sudo python3 - mount \
  --access-rule-name="MorphoCloudCephShare-ro" \
  --access-rule-key="AQAIDi1nKwbRFRAA9KKHUddANj6Ywj8ag7N9pg==" \
  --share-path="149.165.158.38:6789,149.165.158.22:6789,149.165.158.54:6789,149.165.158.70:6789,149.165.158.86:6789:/volumes/_nogroup/60bf684c-51d1-4abb-93f5-188d4d164111/1fe273cd-1e4d-4087-ad2b-01d548a16fe0" \
  --share-name="MorphoCloudCephShare"
```
This is a one-time setup, unless the instance has to be deleted and re-created. Share will be mapped to:

`/media/share/MorphoCloudCephShare`

#### Data transfer between your local computer and remote instance
**Uploading to remote:** If your files are small (<100MB) and you have a stable connection, just dragging and dropping individual files to the browser window. Those files will be saved under your **MyData** volume, which is located at `/media/volumes/MyData/`. If your data is already on the cloud (e.g., MorphoSource, dropbox, google drive, etc), the fastest way is to use the Firefox browser built into the instance and directly download them to your remote session. Just remember to copy them to your `MyData`. </br>
**Downloading from the remote:** If the file is small, you can use the interface shown above in the screenshot (Box D:), which works one file at a time. 

If you have many files, or your files are large, we advise to use SFTP (Secure FTP) tools for bulk upload/download. There are many free tools, search one for your computer. Remember, any data you have generated and important for you, you should download to your own computer. 

### Resources to use through out the course:

1. [Official Slicer User Manual](https://slicer.readthedocs.io/en/latest/)
2. [Official SlicerMorph Tutorials](https://github.com/SlicerMorph/Tutorials/)
3. [Slicer community forum](https://discourse.slicer.org)

### [Day 1](./Day_1.MD)

### [Day 2](./Day_2.MD)

### [Day 3](./Day_3.MD)

### [Day 4](./Day_4.MD) 
