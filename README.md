[<img src="https://www.intelgic.com/static/img/intelgic.png" width="200">](https://www.intelgic.com/ "Powered By Intelgic")
  

 📧 Dropbox Automation
====================================

# :sparkler: Dropbox File or Folder upload
This bot can be used to upload files or folders to Dropbox. It will take the Sheet1 of "master.xlsx" for reference of which files or folders need to be uploaded. When it gets a folder to upload it will search in the Dropbox if the folder name already exists or not. If no folder exists in the Dropbox with the same name at first the bot will create a folder and then read the whole folder and upload each file one by one to Dropbox else it will upload files to the existing folder.

## 🔥 Features:
- Read Sheet1 of "master.xlsx" which consists of 3 columns i.e. File name with proper extension, file path without a file name, and Type. 
- upload files or folders to Dropbox.
- When it gets a folder to upload it will search in the Dropbox if the folder name already exists or not. If there is no folder existing in the Dropbox with the same name at first the bot will create a folder and then read the whole folder and upload each file one by one to Dropbox else it will upload files to the existing folder.
## :heavy_check_mark: How to use?
1. Import the script XML file to your working directory of Dwmaker. `Default: My Scripts`
2. Set Client ID, Client secret, and Refresh token(with scope 'offline_access' and 'files.readwrite.all') which you have got from your Apps setup in Dropbox App console  `(Line:1-3) `.
3. Set the full path to the directory where you have saved your "master.xlsx" file `(Line: 4) Default: C:\Intelgic\master.xlsx`.
        - ***Please note:*** *Sample of "master.xlsx" with Sheet1 and Sheet2 is provided in the folder name "Intelgic". Sheet1 needs to be customized as per the user's requirement but Sheet2 needs to be kept as it is. In the Sheet1 of the "master.xlsx" user need to add the files and folders they want to upload with name and local path as sample*
4. Save the bot.
5. Run the bot.
        - ***Please note:*** *Bot will upload the files and folders to the Dropbox associated with the user you have logged in with the APP and accepted the consent*