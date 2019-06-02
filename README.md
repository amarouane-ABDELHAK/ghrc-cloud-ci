# Purpose 
This image is used to run all the tests using gitlab-ci.<br>
When a push is made this image execute `npm run all-tests`

# How to use
Your project should have package.json and an entry on the scripts section `all-tests` <br>
```
"scripts": {
    "all-tests": "npm run test && npm run test-report"
}
```
<br>
Configure .gitlab-ci.yml to run `npm run all-tests`
