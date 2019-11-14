# groupproject
# README Template

Your [design product spec](https://hackmd.io/s/H1wGpVUh7) (described in that link) will look like the following in your README:

## 1. User Stories (Required and Optional)

**Required Must-have Stories**

~~ * User need the ability to login ~~
~~ * User need the ability to create account.~~
 * User need the ability to search resturant.
 * User need the ability to edit account settings.
 * User need the ability to search deals.
 * User need the ability to select food deliver service.
 * User need the ability to map direction.
 * User need the ability to browse resturant.
 *  User need the ability to (Favorite) push notification.

**Optional Nice-to-have Stories**

 * User can add push notification.
 * User can add Yelp API.
 

## 2. Screen Archetypes

 * [Login Screen]
   * User can login
   
 * [Registration Screen]
   * User can create new account
   
 * [listView Screen]
   * User can view list of resturant
   
 * [MapView Screen]
   * User can find exactly location of resturant and get direction
   
 * [Detail Screen]
   * User can scroll 
   * User can click on to Yelp to add review
   * User can click hover over deals, resturant, and address
  
* [Profile Screen]
  * User can view saved bookmark.
  * User can edit Profile information
  
* [Setting Screen]
   * User can edit home and work address
   User can choose what data privacy to share
   User can edit email
   User can edit phone number
   User can view legal document
   User can logout app

 
## 3. Navigation
**Tab Navigation** (Tab to Screen)

 * Search
 * Map
 * Account Settings
 * Favorites

**Flow Navigation** (Screen to Screen)

 * Forced Login -> Account creation/registration if no login available
  
 * Search -> Opens listview of restaurants and deals
   
 * Map -> gives mapview of restaurants
   
 * Profile -> gives favorites, allows profile to be edited
  
 * Settings -> toggle settings
  
<img src="https://github.com/thatsadeal/groupproject/blob/master/LowFiWireframe.jpg"/>
<img src="https://github.com/thatsadeal/groupproject/blob/master/login.png"/>
<img src="https://github.com/thatsadeal/groupproject/blob/master/Screen%20Shot%202019-11-06%20at%206.21.38%20PM.png"/>
<img src="https://github.com/thatsadeal/groupproject/blob/master/Screen%20Shot%202019-11-06%20at%206.21.00%20PM.png"/>
<img src="https://github.com/thatsadeal/groupproject/blob/master/Screen%20Shot%202019-11-06%20at%206.21.10%20PM.png"/>
<img src="https://github.com/thatsadeal/groupproject/blob/master/Screen%20Shot%202019-11-06%20at%206.21.19%20PM.png"/>
<img src="https://github.com/thatsadeal/groupproject/blob/master/Screen%20Shot%202019-11-06%20at%206.21.26%20PM.png"/>

User

|Property|Type|Description|
|---------|------|----------------|
|fName|String|User first name| 
|lName|String|User last name|
|bDay|String|User birthday|
|phoneNum|String|User phone number|
|email|String|User email|
|unameID|String|Unique id for user| 
|password|String|User password| 

Restaurant 

|Property|Type|Description|
|---------|---------|-------------------------|
|rName|String|Name of restaurant| 
|rAddress|String|Restaurant address|
|rHours|DateTime|Business Hours|
|rID|String|Unique id for restaurant| 

Deals

|Property|Type|Description|
|---------|---------|------------------------------------|
|dealID|String|Unique id for deal|
|dealName|String|Name of deal| 
|dealStart|DateTime|Deal start time| 
|dealEnd|DateTime|Deal end time| 
|rID|Pointer to another parse object|Foreign key of restaurant id|

Saved Deal 

|Property|Type|Description|
|---------|---------|-------------------------------------|
|unameID|Pointer to another Parse object|Username saved deal (Foreign key)|
|dealID|Pointer to another Parse object|Saved deal (Foreign key)|

* Login View Screen
  * (Read/GET)
* Registration View Screen
  * (Create/POST)
* Favorite View
  * (Read/GET)
* Restaurant View
  * (Read/GET) 
* Setting View  
  * (Update/POST)
