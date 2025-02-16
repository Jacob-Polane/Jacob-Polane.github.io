# Hosted JSON files

We are going to use this repo to talk to our json file for long term persistance.

I have sent everyone a github.js script, which we are going to use to communicate with our hosted json files.

how to use the script files

## Steps to make use of github.js

* step 1 : npm i axios
* step 2 : import the function into your js files
* step 3 : call functions with correct parameters

<b>each one is allocated two json files</b>

- users.json
- messages.json

<b>if there is any additional files needed please do advise.</b>

## Updating files 

--------------------------------------------
call function writeToJsonFile(jsondata,type)
--------------------------------------------
--------------------------------------------

----------------------------------------------------------------------------------------------------------------------------------------
jsondata : this is data that you would like to update in json format. This function appends the data by spreading and replacing old data. Please ask facilitors if you don't understand.

----------------------------------------------------------------------------------------------------------------------------------------
type: this is the type of json you are trying to update, possible values "users' or "messages"


---------------------------------------------------
Reading json files
---------------------------------------------------
---------------------------------------------------

readJsonFile(type)

----------------------------------------------------------------------------------------------------------------------------------------
type: this is the type of json you are trying to update, possible values "users' or "messages"


## Examples

import { writeToJsonFile,readJsonFile } from "./github.js";


//reading data from users
readJsonFile("users");


// write new users
let users = [{
    username : "user1",
    password : "password",
    email : "email@gmail.com"
   },
   {
    username : "user2",
    password : "password",
    email : "email@gmail.com"
   }
];

writeToJsonFile(users,"users")

