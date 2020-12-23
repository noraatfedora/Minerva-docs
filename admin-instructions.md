# Minerva Documentation (admin accounts)
Minerva is a website that allows for food banks to automatically calculate routes for delivery. It keeps a database of clients and allows for either volunteer logins or spreadsheet exports. You can access it at https://minervagroceries.org .

# Managing clients

## File upload
![](https://i.imgur.com/U7Qssli.png)

- The easiest way to add many clients at once is to upload a spreadsheet.
- Make sure that your spreasheet contains the following columns on each page:
    - Email
    - First Name
    - Last Name
    - Addresss
    - Apt
    - City
    - State
    - Zip
    - Phone
    - Notes
### Upload options
- If you're uploading a spreadsheet that contains every client, then you can check the box to delete any extra users that might be in the database. **Be careful!**
- The "header" is the row number of your spreadsheet that contains the column names. If your spreadsheet has the words "Email," "First Name," etc. on row 1, then set your header to 1. If you have a title at the top of your spreadsheet, your header is 1. If you don't have a title row, your header is 0.

### Master List
- This is just a normal spreadsheet of clients. It should only have one page on it. If you hit "Download as spreadsheet" on the "all users" page, it's that same format.

### Routes list
- If you've exported your routes into a spreadsheet before, added or removed a few people, and want to update these clients, you can select this option. Each route is on a different page of the spreadsheet. 
- This is the same formatting that you'd get if you hit "Download routes as spreadsheet" on the "Manage Routes" page.

### Troubleshooting
- If your spreadsheet isn't exactly right, you'll probably get a nasty error message.
- Ensure that your column names are exactly correct, and that you're not missing anything (including capitalization). If you don't have certain info about your clients, you can create those columns and just leave the data there empty.
- Ensure that your header is correct. Play around with a couple values until it works.

## Manual entry
- On the "Upload Users" page, you can also create clients by manually entering their data into the website. This is useful if you only want to add a few people.
![](https://i.imgur.com/7el748E.png)


When you're done adding new clients, it's best to calculate new routes as soon as possible. Then, you can download your list of clients from the "all users" page. **Make sure to back this up regularly!**
# Route planning
![](https://i.imgur.com/cTIZZOC.png)


- On the "routes" tab, you can see a list of calculated routes. 
- You'll want to hit 'generate new routes' every time you change the list of clients.
- You can either download these routes as a spreadsheet, or your volunteers can view them from their account.
- Each route has a "priority score." If your volunteers have accounts and are marking when they deliver to each client, then routes with high priority scores will mean that the route should be done sooner. When a volunteer claims a new route in their account, they get one with the highest priority score.
- If you want to combine routes, you can use the "move all to route" feature. Enter the ID of the route that you want to move to.
- You can also move individual clients to another route. Click on "show __ stops", click on the address of the client you want to move, and you should see the option.

## Advanced route options
![](https://i.imgur.com/tcYrpzF.png)


- If you hit "advanced options," you can fine tune the route planning algorithm. If you want good routes that are an hour-ish, you can ignore these options.
- **Maximum number of routes** is an overestimate. If it's taking more than an hour, try increasing this number.
- **Each delivery is equivalent to driving ___ meters:** Because it takes a few minutes to physically step out of the car, locate  a house, etc., increase this number the longer it takes your volunteers.
- **Global Span Cost:** Increasing the Global Span Cost creates shorter routes. It also creates more routes. If you increase the Global Span Cost and it's taking a lot of time to calculate, increase the maximum number of routes.
- **Solution limit:** When routes are calculated, the algorithm generates a number of solutions and picks the best one. You can change the maximum number of solutions it generates to speed it up. Usually, you should use this by setting it to "1" if you want to generate bad routes really quickly (to check if it's solvable).
- Note that all length calculations are done with Euclidian distance. It takes each address, gets the longitutde and lagnitude coordinates, and measures the distance between those two coordinates. It does not factor in the different speeds on roads or highways, or the angles of any roads. Keep this in mind when looking at route lengths.


# Driver management
![](https://i.imgur.com/FfJsmK3.png)

- Volunteers can create new accounts at https://minervagroceries.org/volunteerregister .
- When they have created an account, you can approve them by going to your "volunteer settings" page and selecting them from the dropdown list.
- When a volunteer is approved, they can login and view their dashboard.

