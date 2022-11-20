# Continuous Integration and Continuous Delivery

## Purpose 

CI allows automation of code integration from other branches to main branch. It can also help in automating tests before mergining code to the main branch and even before deploying the app. 
CD allows automation of application deployment process.

## Process 

- CI/CD on Github can be acheived via Github actions. This is acheived by using tools from GitHub marketplace in conjuction with YAML scripting.
YAML scripts are created and stored in the following path `./github/workflows/`.

- YAML scripts decribe the workflow for CI/CD.

- It uses different verbs like on (to indicate when to run the workflow) and jobs (to list the tasks that need to be performed)

- In the `on` part of script we can identify the branch that the CI/CD script needs to run and when it needs to run example push or pull. 

- The `jobs` section identifies the actions that needs to take place. Example of certain actions that can take place are - build, test and deploy. 

- Each job has steps mentioned that identifes the sequence of tasks to be prformed for that job. Each task is represented by the key-word `uses`. Task names can also be assigned by using the keyword `name`. `run` keyword is used to run commands. 

- Once the script has been genrated it needs to be commited and pushed. Based on the actions mentioned in the YAML script whenevr there is a push/pull in mentioned branch in script the workflow starts to execute.

- The workflow execution can be checked at Actions tab on Github