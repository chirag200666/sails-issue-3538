# sails-issue-3538

This branch is to replicate a bug in sails #3538 .
The issue comes up with node version 4.2.6 & sails version 0.12.0-rc6

To replicate the bug install node using `sudo n 4.2.6`
if you don't have n you can install using `curl -L http://git.io/n-install | bash  `

clone this repo `https://github.com/chirag200666/sails-issue-3538`
Install dependencies `npm install`
To use node-inspector as debugger `npm install node-inspector`

start app in debug mode in one shell `node --debug app.js`
and node-inspector in another shell `node-inspector`

open the link which comes in node-inspector in chrome browser and see the app crashing with segmentation fault.

## Update
The issue has been resolved with the new version of node version 5.6.0. 

## Fix
Use node version 4.2.4 `sudo n 4.2.4`
