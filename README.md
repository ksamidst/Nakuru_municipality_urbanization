_____________INTRODUCTION_____________<br/>

This application is part of project MIDST; (Monitoring for Information and Decisions using Space Technologies) piloted by the Kenya Space Agency (KSA), in 
collaboration with a team from other government institutions. It is part of a subproject Spatial Planning. The application allows is users to compare land cover 
classification images of the Nakuru municipality areas between the years 1989, 2000, 2010 and 2020.

______________RUNNING THE SCRIPTS______________<br/>

This process will consist of six steps as follows:<br/>
1.) Accessing GEE<br/>
2.) Downloading the files<br/>
3.) Ingesting the assets into the GEE platform<br/>
4.) Paste the script code onto GEE and convert imports<br/>
5.) Importing the assets/ shapefiles into the script<br/>
6.) Run the script to view products<br/>

To better understand the script and how to do Machine learning with the google earth engine platform, refer from [Supervised classification in Earth Engine](https://developers.google.com/earth-engine/guides/classification)

_______________1.) ACCESSING THE GEE PLATFORM_______________<br/>
The GEE code editor platform is accessed [here](https://code.earthengine.google.com). It requires the users to have a [google account (Gmail)](https://mail.google.com). For new GEE users, it will prompt them to request for access. The response varies in duration.
For more information and a detailed introduction to the platform, refer to the [GEE playground](https://developers.google.com/earth-engine/guides/playground).

_______________2.) DOWNLOADING THE FILES____________________<br/>

![image](https://user-images.githubusercontent.com/75077556/186091882-cea46de0-0824-4f12-950e-ca60c56662d8.png)<br/>
Click on the 'Clone' button at the top of this page, then click on 'Download ZIP', as shown in the image above. Once the zipped file is downloaded, extract the files to a location of your choice. You can open the folders to view the files. There are a number of different files in the folder; there is the script file containing the GEE code and the sub-folders containing the assets (shape files).

_______________3.) INGESTING THE ASSETS/ SHAPE FILES ONTO THE GEE PLATFORM_____________<br/>

![image](https://user-images.githubusercontent.com/75077556/125578391-7ab741aa-633a-4f5b-92dd-ab10c8ea1425.png)<br/>
Once you have been able to access the GEE code editor platform from step one above, on the left hand panel, click on the 'assets' tab as shown in the image above, then click 'NEW'. Under 'Table Upload' click on 'Shape files'.<br/>
![image](https://user-images.githubusercontent.com/75077556/125578723-c0d0d13e-62bc-485d-b3b6-36aa4805cc1e.png)<br/>
As shown above, the 'Upload a new Shapefile asset' dialog box will appear as shown above. Click on the 'SELECT' button and navigate to the folder containing your shape files. Select all the files contained within the shapefiles folder, and put in a name of your choice, for the asset. Scroll down the dialog box and click 'UPLOAD'. Wait for the upload to complete and your asset will appear under the assets tab with the name you set for it. You will need to do this for the 'Nakuru_AOI' and the 'Nakuru_Data' in the nakuru municipality project folder. For more details on asset management on GEE, refer from the [GEE asset manager](https://developers.google.com/earth-engine/guides/asset_manager)

_______________4.) PASTE THE SCRIPT CODE ONTO THE PLATFORM___________________________<br/>

From within the project folder, open the 'nakuruscript.js' file using a text editor of your choice. You will see a huge collection of almost incomprehensible code. Not to worry, as the earth engine code editor has the ability to manage the huge code. Select and copy all the code from the text editor and paste it onto the GEE code editor platform. Scroll to the top of the code editor where you will see the geometry imports with their raw definitions. When you place your cursor above the code, you will see a prompt at the bottom. It lists all the geometry objects defined and gives you an option to 'convert to import records' as highlighted below. Once you select the option, your imports will be organized on your code editor.<br/>
![image](https://user-images.githubusercontent.com/75077556/125584368-d970818f-b5f8-49d7-a84e-c02744911aeb.png)<br/>

_______________5.) IMPORT THE ASSETS/ SHAPE FILES INTO YOUR SCRIPT___________________<br/>
![image](https://user-images.githubusercontent.com/75077556/186093254-f576cd1e-47ee-4b26-8a5b-38d7f644f818.png)<br/>
As shown in the image above, once your imports are in an organized fashion (import records), you will have to replace the highlighted imports with the assets you ingested in step 3 above. Name the imports with the same names in the existing imports, i.e.<br/>
-'AOI'<br/>

![image](https://user-images.githubusercontent.com/75077556/125587500-92fe80ac-13b9-4648-8571-54accc9e1041.png)<br/>
Use the bucket icon on the left hand side of the import, as shown in the image above, to delete the existing import. The icon appears once you hover your cursor on the left side of the imports.<br/>
![image](https://user-images.githubusercontent.com/75077556/186094753-641d9350-247e-45b2-b28c-69f602cfab2e.png)<br/>
Use the arrow icon to the right hand side of the asset you want to import into your script, to import the asset into your script, in the 'assets' tab as shown in the image above.

_______________6.) RUN THE SCRIPT TO VIEW PRODUCTS____________________________________<br/>

At this point you should now be able to run the script and view the products. For more information and details, refer from the [Google Earth Engine Official Documentation](https://earthengine.google.com/).
