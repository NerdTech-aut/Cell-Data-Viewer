# CM CSV Data Viewer
## About
This web tool allows anyone to make more out of the CSV files collected by the CellMapper application.

It is currently available at: [https://nerdtech-aut.github.io/cmcdv/cmcdv.html](https://nerdtech-aut.github.io/cmcdv/cmcdv.html)

![CM CSV Data Viewer main screenshot](/assets/documentation/imgs/Screenshot-Main.png)

This web tool lets you view, filter and export the data points you have collected with the CellMapper application on your Android device.

### Visualization
You to visualize the data points that you have collected with the CellMapper application on a map. You can see each collected data point in detail with information rich tooltips and popups.

![CM CSV Data Viewer popup screenshot](/assets/documentation/imgs/Screenshot-Popup.png)

### Filters
You can filter hundreds or thousands of data points to be able to focus only on what you actually care about. Available filters include PLMN, network type (LTE and NR), Band, ARFCN, (e/g)NodeB (site ID) and cell ID. You can apply filters at once or only a few depending on what you want. Additionally, you can search the filter options to quickly find what you are looking for.

![CM CSV Data Viewer filters screenshot](/assets/documentation/imgs/Screenshot-Filters.png)

### Export
You like what you see on the map. Then you can go ahead and export the map as a HTML file to preserve the currently displayed data points to look at them again later or for sharing with others. 

### Local in browser processing
All processing of the data happens on your device in the browser. The CSV files you select to view, filter and export are not uploaded to any server. The location permission is optional and only used to center the map based on your location. Your location is not shared with anyone!

![CM CSV Data Viewer export screenshot](/assets/documentation/imgs/Screenshot-Export.png)

## FAQ
### How can I save the points I collect to a CSV file?
1. Via the hamburger menu in the top left of the application (three horizontal lines) navigate to the settings of the app.
2. Enable the output to CSV file option which can be found in the Main Settings section.

![CM CSV SBS](/assets/documentation/imgs/CM-CSV-SBS.png)

### Where do I find the CSV files?
The CSV files can be found in the following folder: Internal Storage -> Android -> data -> cellmapper.net.cellmapper -> files

> [!IMPORTANT]
> Please note that if you use the web tool directly on an Android device the **CSV files can't be opened directly from this folder**. This limitation is due to the security aspect that apps shouldn't be able to access storage regions of other apps. The only exception is the build in Android Files application (com.google.android.documentsui) when it's opened from the launcher (home screen & app menu) or via an activity launcher. This should not be confused with the [Files by Google](https://play.google.com/store/apps/details?id=com.google.android.apps.nbu.files) application or any other manufacturer provided files application. With this Android Files application, it's possible to copy the CSV files in the Android Data folder to another folder like Downloads, Documents or any other folder outside of the Android folder. Then the CSV files can be opened from the web tool via the file picker. If your Android device doesn't have a shortcut to the Android Files application by default it is possible to add one either via the [Files shortcut app](https://play.google.com/store/apps/details?id=com.marc.files) from [Marc apps & software](https://marc-apps.nl/) / [Marc-JB](https://github.com/Marc-JB) (easy option) or via an activity launcher app such as [Activity Launcher](https://play.google.com/store/apps/details?id=de.szalkowski.activitylauncher) by [Adam M. Szalkowski](https://github.com/butzist) and add a shortcut to the com.android.documentsui.files.FilesActivity activity to the home screen (advanced option).<br>  
> If you want to use the web tool on a computer you can connect your Android device via a USB cable to access the CSV files. Alternatively, you can share the CSV files to a computer from the Android Files application described above.

## Third-party software and services
The following third-party software and services are used in this project:
- [Bootstrap](https://getbootstrap.com/) and [Bootstrap Icons](https://icons.getbootstrap.com/) from the [Bootstrap team](https://getbootstrap.com/docs/5.3/about/team/) and contributors under [MIT license](https://github.com/twbs/bootstrap/blob/main/LICENSE)
- [Leaflet](https://leafletjs.com/) from [Volodymyr Agafonkin](https://agafonkin.com/) and contributors under [BSD 2-Clause License](https://github.com/Leaflet/Leaflet/blob/main/LICENSE)
- [OpenStreetMap](https://www.openstreetmap.org/about) from the [OpenStreetMap Foundation](https://osmfoundation.org/) and contributors
- Satellite images by [ESRI](https://www.esri.com/en-us/home) and partners
- my own [arfcn-to-frequency-files](https://github.com/NerdTech-aut/arfcn-to-frequency-files) repository based on ETSI and 3GPP documents
- [jsDelivr](https://www.jsdelivr.com/) CDN service for external resources from Volentio JSD Limited
- [GitHub Pages](https://docs.github.com/en/pages) for the hosting of the web tool and directly associated resources from GitHub Inc

## Disclaimers
CellMapper and CellMapper logo are trademarks of CellMapper Services Limited  
Android, Google and their respective logos are trademarks of Google LLC  
NerdTech and the CM CSV Data Viewer project are not affiliated with any of these companies.  
NerdTech and the CM CSV Data Viewer project are not affiliated with any other developers unless explicitly stated.  
Any recommendations for third party software are because I (as in NerdTech) use them and think they are worth sharing in the scope of this project. Please inform yourself about the data collection and data sharing policies of any third-party software.