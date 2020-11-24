## CASE1: Change the button of the page link to a picture
`Background`: A large grocery chain company's goal is to drive more customers to download their APP and registered the loyalty program. One way of driving customers to download the APP, is via a link on the company website. Page viewing statistics shows that only 10% people who visit the main page, are clicking through to visit the page that describes the app and loyalty program

`Question`: whether changing the button of the page link to a picture would improve the click through rates of visitors who visit the page that describe the app and loyalty program.

### Set up a `Randomized Design`:

`Target variable`——whether or not an individual clicked on the link to visit the APP and loyalty information page.

`Control variable`:
* Type of people (whether or not they would click the link)
  * socioeconomic standing, demographic profile,etc
* Site visit (Ensure we only count each people once regardless how many they click)
  * How frequency they visit the site
* Membership
  * If they already have a card or not

`Sample size`:
* Unit of Diversion = IP addrss
* Population = visitors without an account
* Duration = 1week
* Size = 1/3 treatment and 2/3 control

![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case1.png)

### Analyzing Result
using Test of Means tool

![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case1-1.png)

P-value= 1.78169681561049e-32 (which means the two means are not the same, then we could do next step:calculate the difference)

![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case1-2.png)

The percentage of user who clicked on the link 
Control group: 18.59%
Treatment group: 23.25%
(a 4.66% jump)

##Result
This company can drive 4~5% more users to click on the link to learn more about the loyalty program if they change the button on the website to a picture of the app.
