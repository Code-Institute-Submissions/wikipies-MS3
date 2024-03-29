# Wikipes
### The simple way to store your recipes, and share it with others.


<hr>

### Index
1. Project Planning.
2. Updates Timeline.
3. Planned Updates.
4. Bugs & Errors.
5. Additional Comments.
6. External Resources.
7. Testing.
8. Conclusion.


## 1. Project Planning.
I wanted to create a recipe database long before I started the Code Institute programme. As a chef there are flaws in keeping things like this on paper or in notes on my phone. So I made a simple and intuitive recipe database for users to store their recipes, either for their own sake or to share it. 
<br>
<br>
Users will be enabled to create accounts to upload, edit, and delete their recipes. 
<br>
<br>
Users that does not log in will still be able to read the recipes but not upload, edit, or delete any recipes on the site. 
<br>
<br>
Wireframe and a user flowchart can be found in /documentation.


## 2. Updates Timeline.
> 0.3 **2021-03-16**
> > Styled webpage globally with button colors, card panels, and label texts.<br>
> > Editing recipes now looks as intended<br>
> > Editing recipes now works as intended<br>
> > Fixed nested IF statements messing with displayin allergn icons only if the previous was checked.
> > Made allergen switches occupy 3 spaces each and center align them on 2 rows<br>
> > Created edit functionality with conditional if statements to declare wether allergens were toggled in the original recipe.<br>
> > Created delete functionality to use .remove() on the ObjectId in the database.<br>

> 0.2 **2021-03-15**
> > Created edit page using the upload inserts<br>
> > Created routing for edit_page<br>
> > Created submit button for upload recipe<br>
> > tested allergens toggle and viewed output<br>
> > Created dictionary to retrieve info from the input fields on upload_page.html<br>
> > Created variables for allergens to utilize toggles (easier to display on the recipes using ***if toggle on*** statement to display icon)<br>
> > Created routing for upload_page and function to use .insertOne into the<br> database using the input values from the page.<br>
> > Created placeholder input field on upload_recipe for testing.<br>
> > Created routing for login with functions to read hashed password and put user in session<br>
> > Starting development of login page/route<br>
> > Finished registration page<br>
> > Registration function works and uses Werkzeug password hashing<br>
> > Built the function for new registrated users to be stored in the database<br>
> > finished registration page layout<br>
> > Updated index to be able to search categories<br>
> > Added routing for register page<br>
> > Added register page<br>
> > Finished working on frontpage<br>
> > reset the search function resets the current index, returning user to view all recipes<br>
> > search function works, filtering the index<br>
> > Created recipe index in MongoDB to use in the search functionality<br>
> > Added search route<br>
> > Added search elements<br>
> > Added comments for base.html<br>
> > Added comments for JQuerys in scripts.js<br>
> > Added ellergens icons with tooltip<br>
> > Formatted Jinja output for recipes.<br>
> > Configured .dockerfile for GitPod functionality


> 0.1 **2021-03-14**
> > Created app on heroku and configured Config Vars<br>
> > Added User Flowchart <br>
> > Added wireframe <br>
> > Added Static and Templates folder <br>
> > Set up app.py with dependencies<br>
> > set up requirements.txt<br>
> > set up env.py<br>
> > added template extentions from base.html<br>
> > extended base.html to front_page.html<br>
> > frontpage now renders current recipes from MongoDB<br>


## 3. Planned Updates.
> ~~Create cancel button on edit recipe page to redirect user to frontpage<br>~~
> ~~Create If statement on edit page to render all the allergens toggles was on or off before editing<br>~~
> ~~Create function to display users recipes on profile page<br>~~
> ~~Revamp how recipes display on frontpage and profilepage(Add steps)<br>~~
> ~~Implement Search Function~~<br>
> ~~Move flash messages to modal<br>~~(focusing on styling instead, if there is time I will try this)
> ~~Implement User auth<br>~~<br>
> ~~Add more Allergen icons (on frontpage/view all recipes using ***if x on then***<br>~~
> ~~Implement Allergen functions in update/edit recipe to be toggles<br>~~
> ~~Implement Creating of Recipes<br>~~
> ~~Implement Updating Recipes<br>~~
> ~~Implement Deleting Recipes<br>~~
> ~~Implement Functional Registration~~<br>
> Update Project Planning<br>
> ~~style buttons to all look the same<br>~~
> ~~Style nav<br>~~
> ~~Style text content<br>~~
> ~~Style brand logo<br>~~
> ~~Style Flash Messages<br>~~

## 4. Bugs & Errors.

1. 2021-03-14
> **Expected Result:**
> > Applying a Jinja for loop in front_page.html would render on screen in the preview.

> **Actual Result:**
> > The Jinja for loop renders the HTML element to store the database data from MongoDB but renders the elements empty, regardless of the database thats injected

> **Resolved Y/N:**
> > ***Y 2021-03-14***

2. 2021-03-15
> **Expected Result:**
> > using the correct column size would display the search elements and the collapsible element as the same width

> **Actual Result:**
> > the search and collapsible elements does not align

> **Resolved Y/N:**
> > ***Y 2021-03-15***

3. 2021-03-15
> **Expected Result:**
> > Using the implemented python function should render a fully functional and rendered login_page.html, that retrieves data from database to match<br>
> > user credentials. 
> 
> **Actual Result:**
> > Page does not load and [TO_MANY_REDIRECTS], and heroku returns a HTTP code of 302.

> **Resolved Y/N:**
> > ***Y 2021-03-15*** - The 302 code indicates redirecting, but the log does not show an endpoint, leading to a probable error in the routing for the page.
> resolved by editing the /login function with correct indentation.

4. 2021-03-16
> **Expected Result:**
> > creating CSS code targeting elements in the html should change the appearance of the output

> **Actual Result:**
> > The CSS code does not change the appearance of the html, it does work with in-line customization however.

> **Resolved Y/N:**
> > ***Y 2021-03-16*** - Due to not having an online preview that could read jinja I had to push the css changes to main to display them on the live page.(not best practice)

## 5. Additional Comments.
The commits are somewhat inconsistent, the later ones will use the description to specify the changes in the files. 
I am using GitHub Desktop and it was simply more effective for me to write in the description.
<hr>
I have not found a way to visualize functional previews of jinja code on VsCode, thus the large ammount of commits to the main branch.<br>
I pushed commits for testing to push changes to heroku and to display the changes made in the code. This did force me to push multiple commits with the same
description to declare what I was working on, more like workin on a separate branch, but instead doing testing on main. I appologize for the large ammounts of commits.

## 6. External Resources.
[MaterializeCSS Documentation](https://materializecss.com/)<br>
[StackOverflow]([www.stackoverflow.com](https://stackoverflow.com/))<br>
CI Data Centric Modules (MongoDB / Mini Project)


## 7. Testing.
Accepted state would be if user is redirected to the correct link or if a message is displayed if credentials are not met. If measures are met answer will be "works".

| links | registrating | login | upload recipe | profile | log out | search | edit recipe | delete |  |
|-|-|-|-|-|-|-|-|-|-|
| all works | works | works | works | works | works | works | works | works |  |
<hr>




 


## 8. Conclusions.
Due to some extensive computer issues this project has ben put under intense time restraints, once again I would like to reach out and thank CI Student Counceling for their understanding and very helpful ways.
<hr>
Even with the time restrictions I actually enjoyed this project very much. This is probobly because I actually had extended ammounts of time instead having to go away and focus on people thats sick (that does need my help), this helped me massively with focus and dedication.
I very much enjoy working with Back-End intergration and I have learned massively from this.
<hr>

Some jinja rendering is basic, and the output for recipes from the database could have been "prettier", but to me it does its job and works.
<hr>
While this project is heavily influenced by the mini-project, I only reasearched the source code when there were issues I did not know how to fix and I implemented it myself. 
<hr>
While I believe this could have been made much flashier, (as always) I wanted to focus my time where I felt it needed, with the timelimit I had I chose to not do extensive styling or use crazy images, the goal I had was a simple database collection thats intergrated on the page to be displayed and accessed by users. 
<hr>
MS2 was quite horrible for me, as there were too many things pulling me away from my studies, and this time around I had some really bad PC issues with bluescreens and having to run the computer in safemode without network to try to fix it. Eventually I fixed the issue and here we are. This project actually made me prove to myself that this is something I actually enjoy and are capable of completing, and I am so happy I pulled through and completed it. 