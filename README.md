# Readmefile for moneyfy

#Exploratory Testing Charters


**Testers: SAKET ANAND**
**Date: 25/05/2022**
**Timebox or Duration: 5 Minutes**.
**Target or Scope: Home Page UI and Navigations without clicking any UI element.**
**Priority: High**
			
    Test Steps:
	    -Installing and Launching the app
	    -Skipping the "Claim my offer" page by clicking the cross icon on the top right corner. 
	    -Sliding from the center of the screen without touching the right and left screen borders slides the chart page to the next date.
	    -Issue here is that If Current date is 25th may and user slides to the left side from center then the max date he reaches is 28th May which should have ideally shown at least till the last date of the current month.
	    -Sliding towards right touching the left border opens Time filter (Day, Week, Month, Year, All, Interval Choose Date)
	    -Sliding leftwards closes the Filter options.
	    -Sliding towards the left touching the right border opens the Menu filter (Categories Accounts, Currencies and Settings options )
	    -Sliding rightwards closes the menu options.
	    -Sliding upwards from the "Balance" section slides the page up showing the balance records which initially shows a message 
         "There are no records for this period yet"
        -Sliding down touching the "Balance" display section slides the sections down and is navigated back to the home page containing charts. 
 
**Testers: SAKET ANAND**
**Date: 25/05/2022**
**Timebox or Duration: 5 Minutes.**
**Target or Scope: Exploring by Clicking on UI elements icons of the Home Page.**
**Priority: High**
			
**Test Steps:**
  
     -Clicking on the filter icon on the top left corner navigates to filter options which are Day, Week, Month, Year, All, Interval, Choose date etc.
     -Observation: Camel case could have been followed. 
     -Clicking the Filter icon again to close time filters.
     -Clicking on the filter icon opens the time filter options and clicking on the right half greyed out part of the screen closes the filter.
     -Clicking on the 3-dots menu icon on the top right corner navigates to menu options such as Categories, Accounts, Currencies and Settings.
     -Clicking the Menu 3-dots icon again closes time menu options.
     -Clicking the Menu 3-dots icon opens the menu options and then clicking/touching the left greyed out part of the screen while the menu option is open closes the menu option.
	 -Clicking on the magnifier icon opens the mobile keypad in the bottom half of the screen and text box at the top with title as "Search records" and "Cancel" button which on clicking closes the editable search record text box and UI is back to containing the Magnifier icon along with other icons.
     -Clicking on the left and right directional arrows navigates to the New Account page with the cursor on the Name Text box.
     -Clicking on the left or right Hamburger icon (3 horizontal lines slides up the Balance records section)
     -While the slider is up, clicking on the left Hamburger icon slides down navigating to the home page. 
     -While the slider is up, clicking on the right downward arrow icon changes the part of the icon to $ and Calendar but doesn't slide the page down.
     -On the home page with different expense item icons, clicking on each item 
     a. Highlights the circum-circle in green 
     b. Displays the items name on the center circular area (For eg. Car) with the Font in white
     c. And also displays Currency followed by Value spend on that(For eg. Car and INR0.00) in white font color. Here the decimal value font size is smaller than the whole number on the left of the decimal point.
     d. and then navigates to the New Account Creation page if the account is not created.
 

**Testers: SAKET ANAND**
**Date: 25/05/2022**
**Timebox or Duration: 5 Minutes.**
**Target or Scope: Exploring Categories from the 3-dots icon menu option on the top right corner.**
**Priority: Medium**

**Test Steps:**
     -Clicking on the top right 3-dots icon on the home page opens up the menu options (Categories, Accounts, Currencies, Settings)
     -Clicking on the "Categories" shows animation on the Category palate and sliding below the Categories opens EXPENSE & INCOME section with the list of items in EXPENSE and INCOME respectively.
	 -Clicking on the '+' icon on EXPENSE/INCOME probabily adds a user defined personalized EXPENSE item but currently it is available only for subscribed app users so clicking on the cross icon navigates back to "Categories" Section.
	 -Assumption: + icon should 
     -a. navigate to add an item page for EXPENSE/INCOME
     -b. give the user an option to select a display item for the same. 
	 -Clicking on any of the EXPENSE/INCOME items slides the screen towards the left and is navigated to "Edit category" page.
     -Edit category has below ui elements functionalities 
     -Enabled Done button to save the changes and navigate back to categories List page
     -Editable Text box displaying the item name which was selected on the EXPENSE/INCOME Categories page. 
     -And below the editable text box are the different icons that can be selected and set for the selected EXPENSE/INCOME item by clicking the Done button and the same will be updated and will be visible on the home page. 
	 **Renaming a Category item.**
	 -Renaming the Car text to Cars and then clicking Done navigates back to the Home page and the updated name is visible when the Category Expense item is clicked.
	 -Also an update message "Category was updated" is displayed with the "UNDO" button after clicking on the Done for the renamed category and stays for about 10 seconds. 
     -Clicking on UNDO reverts the rename operation and clicking the category item on the home page displays the name of the category before renaming.  
     -If UNDO is not clicked the renamed EXPENSE/INCOME item name is updated and visible on the Category page as well. 
     -While Renaming the Category item from the Edit categories page, there is no length restriction while editing the category name and all characters including smileys are allowed.
     -Renaming any item of EXPENSE/INCOME Category with String length equal to 18 displays the full 18 chars on the homepage when the item is selected.
     -If the EXPENSE/INCOME name is renamed to 18 successfully then full 18 chars are seen on the home page inside the center circle when the expense item is clicked.  
     -If EXPENSE/INCOME name is renamed to greater than 18 chars successfully then full 18 chars are seen followed by max 3 dots if length was 21 or more. 
     -Renaming category name to blank in the Edit category page and then clicking on Done blinks the text box to Red for a moment and an error message is displayed "Name is empty"
	 -Renaming the category to only spaces and then clicking on Done also Highlights the text box to Red for a moment and error message is displayed "Name is empty"
     -Renaming the category item to 21 spaces followed by a valid String and Saving it by clicking done displays only 3 dots on the home page inside the center circle when the expense item is clicked.
     **Deleting a Category Item**
     -On the Edit category page click on the Bin icon which gives a reconfirmation message asking to be sure with the message drafted as "Are you sure? All associated records will be removed . You can merge or disable it instead"
	 -With the above message, cancel and Yes buttons are provided.
	 * Here on the confirmation message, full stop is missing in the text "You can merge or disable it instead"
     **Disabling Any EXPENSE or INCOME item from the Categories section from**  
     -can be disabled by clicking the 3 dots on the top right in the Edit category page and selecting option to "Disable" from the given options - Disable, Merge
     -clicking on the Disable and then clicking on Done 
	     -navigates back to the Home page skipping the category list page 
		 -and that disabled EXPENSE item disappears from the home page.
		 -and also a message is displayed on the home page for exactly 10 seconds stating "Category was updated" along with the "UNDO" button
		 -Clicking the UNDO button reverts the Disable operation and the Category item (eg.Clothes) reappear on the home page instantly.
		 -In the case when UNDO is not clicked, When navigated again to the category Menu it is observed that disabled category item has gone to the last item in the list of EXPENSE/INCOME and the font-color is changed from white to purple.
	  
     **Enabling Any EXPENSE or INCOME  item from the Categories section from **
	 -can be enabled by clicking the 3 dots on the top right in the Edit category page and selecting option to "Enable" from the given options - Enable, Merge
	 -clicking on the Enable and then clicking on Done 
     -navigates back to the Home page skipping the category list page 
     -and that Enabled EXPENSE item appears back on the home page. 
     -and also a message is displayed on the home page for exactly 10 seconds stating "Category was updated" along with the "UNDO" button
	 -Clicking the UNDO button reverts the Enable operation and the Category item (eg.Clothes) again disappears from the home page instantly.		 
     -In the case when UNDO is not clicked, When navigated again to the category Menu it is observed that enabled category item comes back to its original position in the list of EXPENSE/INCOME and the font-color is back to white from purple.	 
     -Menu options on the Edit category changes based on the current status(Enabled/Disabled) of the Category item
	 -If disable is selected for a category in the Edit category page, then before clicking on Done when 3-dots are selected then options changes to Enable & Merge
     - If Enable is selected for a category in the Edit category page, then before clicking on Done when 3-dots are selected then options changes to Disable & Merge
	   
     **"Merge" option on the Edit category page:**
	 *-Selecting merge option for a Category(eg.Clothes) populates Category list on the page as an overlay screen and selecting one of the option (eg. Food) currently gives an error message that back-up file is created with the .bkp extension and navigated back directly to the home page where the Clothes item disappears. *

 
**Testers: SAKET ANAND**
**Date: 25/05/2022**
**Timebox or Duration: 5 Minutes.**
**Target or Scope: Exploring Accounts from the 3-dots icon menu option on the top right corner.**
**Priority: High**	

**Test Steps:**

     -Clicking on the top right corner on the 3-dots opens the menu with options Category, Accounts, Currencies and Settings. 
     -Clicking on the "Accounts" expands the page below and displays Add text, Bidirectional arrow icon and '+' icon. 
     -Clicking on + icon navigates to "New account" page which contains 
     -Back button : which on clicking navigates back to the account page
     -Editable "Name" Text box that accepts alphanumeric and special characters. 
     -Add button: Which on clicking gives error "Name is empty" if Name text box is blank.
     -This error message appears on the page for 10 seconds even if the account is being entered or has finished entering.(Bug/Usability)   
     -Toggle button for Included in balance. 
     -Currency field which on clicking shows different current options on the page and the user can select  from the same but currently the selection navigates to the annual subscription page. 
     -Exchange rate link which on click navigates to annual subscription page
     -Initial account balance field accepting max 9 digit numbers 
     -Initial balance date field shows current date in dd/mm//yyyy format when user lands on this screen for the first time
     -When user clicks on the Initial balance date it opens up a calendar with CANCEL and OK button and current date highlighted on the calendar. 
     -BUG:On an open Initial balance date calendar, when the user navigates towards the previous months in the calendar then only the Month name slides towards right and dates are constant which is fine, but the month name should appear in the center which is currently towards left from the center. 
	 -*BUG: On an open Initial balance date calendar when the user navigates towards the previous months in the calendar and clicks on the CANCEL button then they are navigated back to the New account page. But now if the user opens the Initial balance date calendar again then the calendar opens to the same previous month where the calendar was closed by clicking cancel. For instance if the current month is May 2022 and the user slides back to May 2019 calendar and then clicks on cancel to close the calendar and then again opens the Initial balance date calendar from the New account page then the May 2019 calendar opens instead of Mar 2022. Same behaviour is seen if the calendar was closed CANCEL or OK button for future months as well. *
     -Usability Issue:Good if Initial balance date was editable as a field as well. 
     -Usability Issue:Good if Initial balance date is restricted to current month only, until we have some explicit business case for enabling future calendar.
     -Account can be created with 0 balance
     -When Account is created with x Initial account balance, then this amount is visible on the home page as well in green text inside the circumcircle. 
     -On Account creation on clicking Add button, an account is created and the page is navigated back to the home page with a message on the screen "New account was created" along with UNDO button. This message remains on the page for about 10 second. If a user clicks on UNDO the account creation actions are undone and the Initial account balance disappears from the circumcircle. When the user navigates again to the account page then this account is no more visible. 
     -When an Account is created with x Initial account balance, then this amount is visible on the home page as well in green text inside the circumcircle. Now the user navigates back to the account Menu then this account name is visible on the account page. 
     -Clicking this existing account navigates to the Edit Account Page where an additional Bin button is visible.
     -Clicking this bin button gives a confirmation message before deleting the account "Are you sure? All associated records will be removed. You can merge or disable it instead" Here when user selects Yes, then account deletion happens instantly navigating the user back to the home page with 0 balance with a message "Account was deleted" and also contains an UNDO button. This message stays for 10 seconds and if the user clicks on the UNDO then account deletion operation is undone instantly and Balance amount appears on the home page.
     -Balance amount shows 2 decimal places on the home page.


**Testers: SAKET ANAND**
**Date: 25/05/2022**
**Timebox or Duration: 5 Minutes.**
**Target or Scope: Exploring Multiple accounts an Merge Functionalities.** 
**Priority: High**


     -Multiple accounts can be created with an Add account and all the created accounts appear on the Accounts Page. 
     -clicking one of the many created accounts opens its Edit account section where all the fields are editable. 
     -Clicking on the bidirectional arrow button Opens up the New transfer page with Current day and date specified. 
     -This New transfer page contains an unnamed field with currency INR and 0 displayed on the text box. 
     -Below the add note field are the 2 dropdown fields with prepopulated first account created name in 1st Field and second account created name in the 2nd dropdown field. 
     -Below dropdown is the numpad button that populates numpad. 
     -When the user focuses on the amount field to enter the amount then the num pad opens containing a SAVE button which  blinks red if the amount is 0.
     -If amount>0 is entered then the page navigates back directly to the home page.
     -In order to validate the transfer from Account A to B, click on the 3-dot menu followed by selecting account and this account transfer can be seen as updated account balance in the account list view. 
     -BUG: If user has only 1 account then also bidirectional arrow icons are enabled which clicking navigates to New transfer with From and To dropdowns showing this same account name and when user click on amount or numpad button then dropdown highlights in red with error message "Account have to different" 
     -When user clicks inside the field the number pad opens up with +,-,*,/, and = buttons just like calculator which was not required at all. 
     -Clicking on the Notes opens up the Mobile keyboard but at the same time , the number pad of the app remains beneath 1,2,3 and partially visible 4,5,6. Bug added. 
     -Usability Issue:Another feature is that New transfers cannot happen between the same account and blinks read only when the user is trying to fill in the transfer amount.   Ideally the user should be able to select the same account by disabling the From account name in the To account drop down.
     -Usability issue: Whenever any user reaches to transfer page then 

     -Adding multiple accounts sums up their defined Initial account balance and shows up on the home page as account balance. 
     -Deleting 1 of many accounts reduces the account balance on the home page by the Initial account balance of the deleted account. 
     -Undoing the delete operation of an account reverts the Balance amount on the home page i.e. Initial account balance of undone deleted account is added to Balance.
     -When income(eg.500) is added by clicking on + on the homepage and if that  point of time we have 2 account A(balance 1000) and B(Balance 1000) then by default the added income amount (i.e. 500) gets added to the Account A resulting in the balance as 1500. Ideally it should ask which account should the income be added to. bug with description added.
     -BUG: Account A with initial balance 100 and B with initial balance 100. We are able to do an account transfer 500 from A to B despite having a balance of 100. Also the updated balance in A becomes 400 and B becomes 600.  If this is intended then for sure this is ambiguous to the user. 


**Testers: SAKET ANAND**
**Date: 25/05/2022**
**Timebox or Duration: 5 Minutes.**
**Target or Scope: Exploring Settings.**
**Priority: Medium**

     -Reaching settings: Click on the 3-dot menu button from the home page and then select settings. 
     -Clicking on settings expands the settings below listing the options available in settings. 
     -Budget Mode in the settings is not intuitive. If we give an amount as 100 and enable budget mode then on the home screen we see balance as INR 3.33 and when disabled then the home page shows INR 0.00.
     -Clearing data from setting and relaunching the app still persist the data of the budget mode.
     -Enabling Carry over in settings navigates back to the home page showing an additional row of INR balance in green along with Income and expense balance.
     -Dark theme is disabled from non-annual subscriptions.
     -Selecting Language opens a list of language options in the list, and when an option is selected then "You should restart the application in order to apply the changes" and this message is displayed in the language option selected and also the Settings options language changes instantly without restarting the app. 

    
#Bugs/Observations:

**Below are the list of observations found during testing**

1.Low Priority: It looks good to use camel case the texts used in the app Choose date, New expense, Edit category, New account, New transfer.
 
2.Low Priority: When we are on the day filter, the next date slides upto 3 days only. It should have been more. 

3.Low Priority: While Renaming the Category item from the Edit categories page, there is no length restriction while editing the category name.

4.Low Priority: Renaming the category item to 21 spaces followed by a valid String and saving it by clicking Done displays only 3 dots on the home page inside the center circle when the expense item is clicked on the home page.

5.Low Priority: When a category item is selected and delete/bin icon is clicked on the edit category page then on the confirmation message, a full stop is missing in the text "You can merge or disable it instead"

6.Low Priority: The delete category confirmation message should have been in Text matching to the app. Currently it is displayed in white which looks like an error message of the mobile/cell phone being used. 

7.Medium Priority: Selecting Merge option for a Category(eg.Clothes) populates Category list on the page as an overlay screen and selecting one of the option (eg. Food) currently gives an error message that back-up file is created with the .bkp extension and navigates back directly to the home page where the Clothes item disappears. Even after re-launch of the app, Clothes options do not appear on the home page. 

8.Low Priority: On the accounts page, clicking + button opens up the New account page but the Add text also gives a feeling of the same functionality of New account. Therefore the normal text and '+' button could have been a bit different. 

9.Medium Priority: When we click on '+' reaching to the New account creation page and then click Add button on the top right again without giving the Account name then we get an error message "Name is empty" which remains for 10 seconds. But the issue here is that if the user has started entering/typing or has completed entering the account name, then also the blank validation error message does not disappear until it has completed its 10 seconds. Expected Solution: The blank error validation message should disappear as soon as users start typing/entering/filling the text box. 

10.Medium Priority: On an open Initial balance date calendar when the user navigates towards the previous months in the calendar and clicks on CANCEL button then they are navigated back to the New account page. But now if the user opens the Initial balance date calendar again then the calendar opens to the same previous month where the calendar was closed by clicking cancel. For instance if the current month is May 2022 and the user slides back to May 2019 calendar and then clicks on cancel to close the calendar and then again opens the Initial balance date calendar from the New account page then the May 2019 calendar opens instead of May 2022. Same behaviour is seen if the calendar was closed CANCEL or OK button for future months as well. Expected Solution: Whenever an open calendar is closed with whatever open calendar of Past or future date then reopening again should open the current month Calendar only. 

11.Medium Priority: New transfer page opens a calculator screen when the user intends to enter an amount value. Other than number options, it looks odd and misleading. 

12.High Priority: While the calculator like screen is open while editing the amount on the New transfer page and then if user is done entering the amount and moved to next editable text box of writing notes then the mobile keyboard opens up but the previously open number pad does not disappear at this point of time as well which should disappear. Expected Fix: When user is entering numbers/amount on New transfer then Num pad of the app should appear and once the focus is shifted to entering notes then Numpad should close and Mobile Keyboard should appear instantly.

13.Medium Priority: Due to issue 14, the number pad as well as mobile keypad is active at the same time. That means we see 2 active cursors on the same page which are on the Amount field and Notes field and both are editable at the same time. Part of the number pad(1,2,3 and partial 4,5,6) is visible below the mobile keyboard.

14.High Priority: When income(eg.500) is added by clicking on + for income on the homepage and if at that point of time we have 2 accounts A(with initial balance 1000) and B(with initial Balance 1000) then by default the added income amount from homepage (i.e. 500) gets added to the Account A resulting in the balance as 1500. Issue here is that this 1500 for account A is only visible on the Account list page (where we reach by clicking on the 3-dot menu option followed by clicking on account menu) where we can see a list of accounts and their balance. Now if we click on Account A reaching to the Edit account page of Account A then here the initial account balance shows 1000 which is confusing.  Ideally it should ask which account should the income be added if at all needs to be added instead of adding to the first created account. 

15.Low Priority: Usability Issue:Another feature is that New transfer cannot happen between the same account and blinks red only when the user is trying to fill in the transfer amount. Ideally the user should not be able to select the same account and this can be achieved by disabling the selected From account name in the To account drop down and vice versa.

16.High Priority:If user has only 1 account then also bidirectional arrow icons are enabled which clicking navigates to New transfer with From and To dropdowns showing this same account name and when user click on amount or numpad button then dropdown highlights in red with error message "Account have to different". Expected solution: Users should have the choice to go to the Transfer page if they have only 1 account. 

17.High Priority: Account A with initial balance 100 and B with initial balance 100. We are able to do an account transfer of 500 from A to B despite having a balance of 100. Also the updated balance in A becomes 400 and B becomes 600.  If this is intended then for sure this is ambiguous to the user.

18.Low Priority: Budget Mode in the settings is not intuitive. If we give an amount as 100 and enable budget mode then on the home screen we see balance as INR 3.33 and when disabled then the home page shows INR 0.00.

19.Low Priority: Clearing data from setting and relaunching the app still persist the data of the budget mode. 

20.Low Priority: Selecting Language opens list of language options in the list, and when an option is selected then message is displayed "You should restart the application in order to apply the changes" and this message is displayed in the language option selected but the Settings options language changes instantly without restarting the app. As per message, this change should happen post restarting the app.

21.High Priority: When expense is added for few items then it is seen that the links on the home page are not created sporadically and when number of links increases the links are visible and disappear sporadically. (Link is the lin created between the category element to the circle on the home page) 



#Which area of the app or testing should be explored first and why?


As we know that we are dealing with an app first, the below areas of the app should be tested first.

a.Since it is an app we can start testing with the basic navigations from the page covered in chapter 1 where the user is just playing around with the app to see that features are present.
b.Any clickable button or icons or links should be tested and made sure that there is no lag and that it is working as per functionality. 
c.Once the above are checked for sometime, then comes the functionalities that a money app provides as mentioned below. 
d.Make sure there is not data loss due to low/no network or sudden switching of mobile to due battery drain.
e.Check if the UI is not breaking in dark mode and panoramic mode and UI elements align themselves accordingly.
f.Make sure there is no random or sporadic flickering of the screen.
g.App needs to be tested on the supported platforms.
h.Globalization/Localization Testing will take on priority id apps that need to be newly launched in specific language.

#Coming to Monefy APP 

**High Priority**

1.Adding of Income and Expenses and seeing the updated UI and calculations on the home page. 
2.Making sure that the calculations are working fine are updated at every intended page on the app. 
3.Making sure all the given filters are working as expected and the applicable changes can be seen. 
4.Making sure the addition of accounts and merging are happening properly. 
5.Making sure all the UNDO buttons at most of the basic functionalities are working fine then we can go deeper into testing the UNDO button at low priority areas. 
6.Make sure adding of expense and incomes category works fine as these might be common areas where users will first try to set/add them according to their needs. 
7.Account addition and deletion and UNDO button specific to them.
8.Transfer of money from one account to another and verifying the credit and debit balances
9.Change in the balance figures during Currencies transitions and the conversion rates applicable are perfect or not.
10.Search functionality on the homepage should be tested with Exact match, partial match and no match.  
11.Budget mode which is currently not intuitive enough
 

**Medium Priority**

1.Addition of multiple accounts and their intended effects on the Balance on the UI
2.Deletion of Multiple accounts and their intended effects on the Balance on the UI
3.Merging accounts
4.Testing date filters with boundary value partitioning Technique.
5.Transfer of money from one to many and from many to one accounts and verifying the credit and debit balances.

**Low Priority**

1.Cosmetic changes
2.Error message refinement. 
3.Confirmation messages.
4.Changing button backgrounds to show when it is enabled and when disabled. 


#Risks that need to be mitigated for this type of application:

1. Authorization and authentication
2. Data Security, Data Leakage - Basically Privacy Management
3. Weak security Encryptions
4. Currencies exchanges and conversion 
5. Malware attacks
6. Usage on Public Networks, wifi
7. Protections again duplicate fake apps  
8. Data Privacy/Protection after theft like Mobile stolen. 









 
  