# mastering-python-collections

## Setting up Repository

Here are the instructions to setup the repository.
* Login into Gateway node and open terminal
* Run command `git clone https://github.com/itversity/mastering-python-collections.git`
* It will create a directory by name **mastering-python-collections**. You can validate by running `ls -ltr` command.
* You can view by checking the home directory. You should see the new folder.
* Go into the folder using JupyterHub and see validate the README.md file.

## Using git to add scenarios

We need to use Git CLI to add the scenarios into the GitHub Repository so that we can collaborate. `git clone` will make a initial copy. As you guys collaborate you have to be comfortable with some of the git features.
* Adding branches
* Placing pull requests (it is also called as PR)
* Reviewing the code (by the leads)

Here are the steps with commands.
1. Create a branch for the scenario with name `scenario/<provide scenario specific details>`. In this example, I am adding sample data to repo and hence I named the branch as `data/amazon-bestsellers`.

```
git fetch # Make sure to fetch the changes from the repo to your local copy
git pull # To get the latest changes
git checkout -b data/amazon-bestsellers
```

2. Create required notebook with meaningful name. We can add number later. If you want you can take care of multiple scenarios or notebooks under one branch.
3. Make sure to take care of pushing the branch once in a while. Here are the sequence of commands you can run to push your changes at regular intervals. Make sure to go through the output of each command and understand what is happening.

```
git branch # to confirm the branch. You will see * for the active branch
git status # Check current status of your branch
git add data # You can specify folder name or file or patterns
git status # You will see new and modified files are being tracked
git commit -m "Added Amazon best sellers data set" # Make sure to provide meaningful commit messages

git push origin data/amazon-bestsellers
```

4. Once you are confident that your changes are done and want the lead to review, you need to place the Pull Request (PR). You can do so using GitHub web page of the project.
  * Open repo in the browser.
  * It will automatically start showing your changes and will provide the capability to place the pull request.
  * You can also go to **Pull requests** section and create new pull request using **New pull request** button.
  * Make sure to choose right branch and also provide required title and description.
5. The owner or designated repo admins will be notified about pull request. Now the owner can use the GitHub repo page and review the code before accepting the pull request.


