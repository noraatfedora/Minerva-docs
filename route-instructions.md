# Creating delivery routes instructions

The website that Jared has created for managing delivery routes is https://minervagroceries.com .
The website supports accounts for food banks, delivery clients, and drivers. Currently, only the food banks should sign into the website.

![](https://i.imgur.com/sW5GpaC.png)
You can sign in with this button here.

![](https://i.imgur.com/Kmt57ox.png)
The email for the food bank is `info@madfseattle.org`, and you should have been given the password.



![](https://i.imgur.com/dqHRAa1.png)
You should see the "All Users" page when signed in successfully. You can change which page you're looking at by clicking on the menu at the top.

## All users page
- This page lets you edit the current list of users.
- Hit "Download as spreadsheet" to download the list of all users. **Do this regularly, and back up the spreadsheet in a safe place!**
- Gray cards correspond to disabled users (they won't be included in the routes), and blue cards are enabled. You can change if a user is disabled or enabled by clicking the button on their card.
- If you really want to fully delete a user, you can do that by clicking "Fully delete user", although this should be rarely necessary.
- You can edit a user's data (their address, phone number, any delivery instructions, etc.) by clicking on the "edit user data" button.
- Tip: You can use control-F to find a user quickly.

## Editing a user's data

![](https://i.imgur.com/IQWVl4j.png)
- This is the page you should see when you hit "edit user data". **Make sure to hit "save changes"** when you're done!

## Adding users
- Go to the "Upload users" page to add users.
![](https://i.imgur.com/XA4Y7pD.png)

- The best way to add new clients is by uploading a spreadsheet.
### How to process the Google Drive data
*Note: In this section I describe certain keyboard shortcuts for Google Drive. If you're on a Mac, hit "command" instead of "control."*
- You should have a spreadsheet from the google form on the madf website. This requires some manual formatting before you upload it. Here are the steps:
    1. Open the spreadsheet on Google drive.
    ![](https://i.imgur.com/K5zPzqm.png)
    2. On the bottom of the screen, you should see sheets with people who have been recently added. Click on the most recent one.
    ![](https://i.imgur.com/sPoAOm1.png)

    3. Look at who the most recently added client is. For example, in this screenshot, the most recently added person is Latia Brown. Remember their name.
    ![](https://i.imgur.com/uZFqxX0.png)
    4. Go back to the "From Responses 1" tab on the bottom.
    5. Find the most recently added person, which you should have from step 3. There might be a couple duplicate names on the spreadsheet. Make sure that if the client appears a couple times, that you find the most recent (lowest) row that they filled out.
    **Pro tip: You can use the keyboard shortcut control+f to quickly find a user.**
    ![](https://i.imgur.com/TalP9AA.png)
    6. Select the users that come after.
      **Pro tip: You can easily select entire rows by clicking and dragging on row numbers on the left.**
    ![](https://i.imgur.com/AZqLxib.png)

    Copy these users to your clipboard. You can do this by hitting control-C, or right clicking and click "copy."
    7. Crete a new sheet. Paste the new users by hitting control-V.
    ![](https://i.imgur.com/UGzy2TS.png)
    ![](https://i.imgur.com/ywBJiMN.png)
    ![](https://i.imgur.com/DbMnjxF.png)
    8. Right click on your sheet name.
    ![](https://i.imgur.com/DDysqeu.png)
    Click "Rename." You can organize these sheets however you want, but the naming convention that I have been using is "New clients after" and then the date of the least recent client on the sheet (in this case, it would be "New clients after Jan 19")
    ![](https://i.imgur.com/TUycjYQ.png)
    9. Create a new row at the top. You can do this by right clicking on the "1" corresponding to the top row, and then clicking `+ Insert 1 row above`.
    ![](https://i.imgur.com/8c9Os5m.png)
    ![](https://i.imgur.com/sZw4mwa.png)
    10. Add labels in your top row.  **Tip:** You can quickly add labels by copying the row from last week's sheet.
    
    Your labels should be:
    - Email
    - First Name
    - Last Name
    - Address
    - Apt
    - City
    - State
    - Zip
    - Phone
    - Notes
    
        You can skip labeling any other columns. **Make sure that your capitalization matches as shown! If you mess this up you'll get an error when you try to upload your users!**
    ![](https://i.imgur.com/zhAV5Rp.png)
    11. You'll want to create a new spreadsheet on your computer, with just this single sheet on it. The way I prefer to do this is:
        - Select all users on this sheet by doing control-A
        ![](https://i.imgur.com/HZAFofp.png)
        - Copy using control-C
        - Open up Excel or [Libreoffice Calc](https://www.libreoffice.org/) (a free alternative) and create a new document. (I'll be using Libreoffice for this, but it's the same process as Excel)
    ![](https://i.imgur.com/YEhOwI7.png)
        - Paste your users into it.
        ![](https://i.imgur.com/fcpOvEO.png)
        - Rename this sheet to `Master list`. Make sure that there's a capital `M` and a lowercase `l`. You can do this the same way that you did in Google Sheets earlier.
        ![](https://i.imgur.com/UZAfiOC.png)
        - Save your document, with whatever title you want. Make sure that the format you select is `.xlsx`, which should be the default if you're using Excel.
        ![](https://i.imgur.com/CbSXltT.png)
    12. Now that you have your properly formatted spreadsheet, you can upload it. Head over to the "Upload users" page, hit `browse`, and select the spreadsheet you just created. 
![](https://i.imgur.com/EUJiThA.png)
These default values should be correct. Hit `Submit`. It might take a bit of time (five to sixty seconds) to load.

## Generating routes
![](https://i.imgur.com/kVQ43Bu.png)
- This page lets you view, edit, and create new delivery routes.
- If you just want new routes, hit "Generate new routes" and wait half an hour.
- For most of the parameters under "Advanced options" button you don't really need to know or care about, as these default values should be good enough. 
![](https://i.imgur.com/SLhNZwV.png)
The only one you might want to click is "One city per route", which makes each route have a specific city that it focuses on. If you're really curious, you can click "What's this" next to any parameter here and it'll tell you.

## Loading screen
![](https://i.imgur.com/49pI0iX.png)

- This will be the screen that you see when you hit "Generate new routes".
- There is currently a bug in the loading screen where sometimes it might not tell you when routes are done. You can double check if routes are done by opening "Manage routes" at the top in a new tab. If it looks like the following:
![](https://i.imgur.com/MLsWA7i.png)
Then the routes are still being generated, and you can refresh the page until they appear.
- This issue will be fixed soon.

### Troubleshooting
- If you see a `503 internal server error`, nine times out of ten, this will work if you refresh the page.
- When uploading a spreadsheet, it'll give you an error message if the formatting is incorrect. Double check that your row labes are correct, and that the sheet is named `Master list`.
- Otherwise, create an issue on the [Github page](https://github.com/jaredgoodman03/Minerva/issues/new) or email `jared@themadfseattle.org`.