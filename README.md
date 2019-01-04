### Intro
The purpose of this project is to get some experience building real life functionality. This is a practice that would be given to you by a prospective employer before an interview. The intent would be to see if you have the skills necessary to build something realistic that would actually be used in business software. They want to see your ability to code before they spend time interviewing you. There are no brain teasers or algorithms but it does require a small amount of math and logic thinking.

### Setup
Use any approach you want to build this project. An online editor, create-react-app or raw React.
Use React but do not include jQuery in your project.

### Instructions

Create a currency converter that converts a user’s selected base currency and outputs the equivalent money value of the exchange currency using the current day’s rate.

Include two select inputs, one for base currency and second for equivalent currency, which make use of the json found at:
https://gist.githubusercontent.com/mddenton/062fa4caf150bdf845994fc7a3533f74/raw/27beff3509eff0d2690e593336179d4ccda530c2/Common-Currency.json

For the base currency, create a masked currency input that:
* Shows the symbol of the selected base currency
* Is formatted to two decimal places
* On focus sets the cursor to the rightmost decimal position
* Only allows numbers
* When a new number is inserted shifts the decimal right one place,
* When deleted shifts the decimal left one place

Currency rates are available from http://data.fixer.io/api/latest?access_key=d0f3b7da0757140a192df5c5ee3fd3cf

Use the money.js library (see this jsfiddle's External Resources) to convert the selected base currency to its chosen equivalent money value. 
For more details: http://openexchangerates.github.io/money.js/

Best practice would be to inform the user if their selected currency is not available from fixer.io using inline validation. 
In order to more easily test error handling, allow the user to select a currency not available from fixer.io and present the error returned.
 
Show the equivalent money value's currency symbol which is included in the above Common-Currency.json endpoint.



[Example](https://plnkr.co/edit/Ap0oLDcb3vt1eLAnEUxe?p=preview)
