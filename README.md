#Vue with AWS Serverless Full Stack implementation

##Pre requirements 
### NPM & NODE
https://nodejs.org/en/download/

If you run into a Windows issue similar to `npm does not support Node.js v12.18.3` go to the following link
https://stackoverflow.com/questions/63196042/npm-does-not-support-node-js-v12-18-3

### Install Serverless CLI 
https://www.serverless.com/framework/docs/getting-started/

### Create AWS Account  Free Tier
https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=*all&awsf.Free%20Tier%20Categories=*all

### AWS  CLI
### Create a CLI User to use Serverless requests
https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html

## Examples in this Repo:
`backend` folder:
* Navigate to this folder and run `npm install` to downlowd the dependencies
* Run `serverless deploy` to deploy your serverless implementation

`frontend` folder:

There are 3 examples in this folder. All can be ran by simply opening the HTML in a browser :

`vue-coindesk/coindesk.html` - The goal of this example is to demonstrate a simple Vue front end performing and internet call.

This Contains a very simple Vue frontend implementation with Axios webclient
integrated with Axios webclient to perform a simple REST call to a coin base endpoint

`vue-todo/todo.html` - The goal of this example is to demonstrate local storage and the usage of Vue directives.

This contains various directives and logic to determine what to show to the user. 
Local storage usage can be seen by doing the following :

Using the Chrome browser
1. Open the Developer Tools
2. Click `Application`
3. Click `Local Storage`
4. You can see the used storage after entering Todo's in the appication

`vue-todo-aws/todo.html` - The goal of this example is to demonstrate a front end application and how we can use it 
to make back end calls
#### Note: If you run into CORS issues, you can use [this application](https://chrome.google.com/webstore/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf) to get past it
#### Note: In order to ge this application working properly, you must deploy the back-end application and set the URL's on the various `AMAZON_ENDPOINT*` endpoints on the vue.js frontend application
#### Note: Any backend sync will over write the local storage

This version of the application allows you to create Todo's and get a list of Todo's from the backend server (using the `sync with server` button). 

Cool things to take this further.
1. Enable validation on the front end
2. Add the code to update a Todo on the backend application 
3. Add the code to remove a todo from the backend service


## Other cool stuff 
### .gitignore builder
https://www.toptal.com/developers/gitignore
