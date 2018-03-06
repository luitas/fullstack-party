# Load projects
App consist of 2 projects `front` and `api`
This project has 2 submodules to get all of them run commands

`git submodule init`

`git submodule update`

# Init
1. Init API Run `composer install -d components/api`
2. Init Front(Angular) Run `cd components/front && npm install && cd ..\..` or just run tow commands:
`cd components/front` and `npm install`

# Config  
1. In **components/api/.env** file change `CLIENT_ID` and `CLIENT_SECRET` to your own. 
Authorization callback URL set to `http://127.0.0.1:4200`

2. Change main parameters in file: **components/front/src/environment.ts**
   
   `clientId` - gitHub CLIENT_ID 
   
   `apiUrl` - API full URL
   
   `fromLoginUrl` - There github return user baseUrl + /login
 
 # Run
 1. Run API `php components/api/bin/console server:run`
 2. Run Front(Angular) `cd components/front && ng serve --open && cd ..\..`
 
 
 