#This files describes the repo importance

# The repo is created for Zedrix software organization for the gitflow workflow.

#gitflow Workflow:
#remote master -> remote release -> remote feature/defect -> local dev work on feature/defect
#       -> from local push back to remote feature/defect -> merge remote feature/defect to release
#               -> release the remote release branch to PROD -> merge release branch to master.

#STEPS FOLLOWED: (local: git and remote: github.com)
#1.(master branch)
#created master on local after cloning with repo-url and push from local to remote.==> will create master on local then push to remote
#create README file while creating repo itself to create master branch on remote itself directly ==>  will create master on remote

#2.(remote release branch)
#on remote create a release branch from master.(This is used for releasing defect fix or features to PROD env)

#3.(remote feature/defect branch)
#If any feature requirement/defect fix came up, will have to "create branch/use the already existing branch" from release branch say remote feature/defect branch, Developers will clone this remote feature/defect branch to local and work on this code and push to the same remote feature/defect branch.
#NOTE: before pushing code to remote feature/defect branch, first developers need to pull from remote feature/defect branch and resolve if any conflict arise--by keeping/removing/adding new code to include as per requirement.

#4.(merge remote feature/defect branch to remote release branch)
#Once remote feature/defect branch is updated by developers with the defect/feature requirements, we will merge the remote feature/defect branch to remote release branch then via remote release branch we will release code to PROD Environment.

#5.(merge remote release branch to master/main branch)
#Once confirmed PROD Environment is fine after the release, merge remote release branch to master/main branch.

#6.(hotfix branch)
#IF any critical issue occurs and need a fix immediately, then via main/master branch we will create a branch named hotfix branch and ask developers to work on the issue and push code back to hotfix branch and finally merge the code to remote master/main branch.
