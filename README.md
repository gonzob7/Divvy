# Divvy

## Steps for Local Setup #Team 
1. Fork the project & clone locally
<pre><code>git clone git@github.com:ellojess/Divvy.git</code></pre>

2. Create an upstream remote and sync your local copy before you branch
- cd into the local project directory 
Then: 
<pre><code>git remote add upstream git@github.com:ellojess/Divvy.git</code></pre>

**NOTE:** 
You now have two remotes for this project on disk:

- origin which points to your GitHub fork of the project. You can read and write to this remote.
- upstream which points to the main project’s GitHub repository. You can only read from this remote

3. Create branch for each separate piece of work

*BUT FIRST* Ensure you're on the master branch and up to date 

Sync your local copy with the upstream project <pre><code>git pull</code></pre>
Syncs it to your forked Github project <pre><code>git push</code></pre>

Now you're ready to: <pre><code>$ git checkout master
$ git pull upstream master && git push origin master
$ git checkout -b fullname/LoginViewControllerUpdate
</code></pre>

4. Do the work, write good commit messages
<pre><code>git commit -m "Your-Full-Name/Feature_Description"</code></pre>

5. Push to your origin repository

Example: <pre><code> git push -u origin fullname/LoginViewControllerUpdate</code></pre>
This will create the branch on your GitHub project
The -u flag links this branch with the remote one, so that in the future, you can simply type *git push origin*

**Double Check** Swap back to the browser and navigate to your fork of the project 
You’ll see that your new branch is listed at the top with a handy “Compare & pull request” button


6. Create a new PR in GitHub
If you scroll down a bit, you’ll see a diff of your changes. Double check that it contains what you expect.

Once you are happy, press the “Create pull request” button

**Update the Trello board to let other members know you're ready for review**

7. Respond to any code review feedback and keep up the good work(: 
