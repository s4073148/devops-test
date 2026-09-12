# COSC2759 Assignment 1
## Notes App - CI Pipeline
- Full Name/Names:
  - Marcell Joe Sugianto
  - Arman Gholami
- Student ID/IDs:
  - s4073148
  - s4039910

## 1. Explanation

### 1.1 How the Pipeline is Run
The pipeline is run when a code change is pushed to the Git Repository.
The workflow file is located in the .github/workflow/ directory, which has code that listens for events (e.g. on push) and defines jobs (e.g. set of steps to test, build, or deploy scripts)
Once the workflow is triggered (such as by a push to the repository), GitHub provisions a dedicated VM (as defined in the workflow file) to run the jobs defined in the workflow.

### 1.2 Required Commands to Run Properly
Simply run `git push` on a branch that's defined in the .yaml file which will have the workflow run

### 1.3 Expected Output
The expected output will be the results of all tests ran, and a deployable artefact of the app if all tests are passed

