# Ryanair
To start the project you must run the file "__Ryanair_FINISHED_01.side" in selenium IDE from your browser.

First you need to instal Selenium IDE plugin. There  is an extension for Firefox and Chrome.
Launch Firefox and navigate to https://addons.mozilla.org/en-US/firefox/addon/selenium-ide/
or use this link if you are using  Chrome
 https://chrome.google.com/webstore/detail/selenium-ide/mooikfkahbdckldjjndioackbalphokd

Click the Selenium IDE icon on the right corner of your browser.
Start Seleniun IDE
Choose Open an existing project from the dialog  window.
Browse the file "__Ryanair_FINISHED_01.side" and  click run.
The automated  record for booking up a flight at http//rayanair.com/us will play.

Here is a recording of the script in action:

https://www.youtube.com/watch?v=hlxWJU7PwYI

Here is a sample Gherkin example:

Feature: Fail payment

# Meaningful comment
Scenario: Open ryanair website
Given Logout
And Fill in flight details
And Click Next to payment screen
And Log in with test account
When Input wrong credit card details
Then Check for error message



Rule: Start Fresh
Example: You are logged in
Given The user is logged in
Then Log out

Example: You are not logged in
Given The user is not logged in

P.S. I have used a temporary email to set up an account for testing.




 
