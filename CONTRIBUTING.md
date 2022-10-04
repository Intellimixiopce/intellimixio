## Contributing to intellimixio

First off, thanks for taking the time to contribute! ❤️

- [ ] [Live Preview](https://intellimixio.in/)
- [ ] [Contribution Guidelines](https://training.galaxyproject.org/training-material/topics/contributing/tutorials/github-command-line-contribution/tutorial.html)

All types of contributions are encouraged and valued. Please make sure to read the relevant section before making your contribution. It will make it a lot easier for us maintainers and smooth out the experience for all involved. The community looks forward to your contributions. 🎉

> And if you like the project, but just don’t have time to contribute, that’s fine. There are other easy ways to support the project and show your appreciation, which we would also be very happy about:
>
> - Star the project
> - Tweet about it
> - Mention the project at local meetups and tell your friends/colleagues

## I Have a Question  
  
> If you want to ask a question, we assume that you will mail here  [intellimixio.pce19@gmail.com](mailto:intellimixio.pce19@gmail.com).

### How to contribute

 1. Create a fork of this repository on GitHub
 2. Clone the GitHub repository on your computer
 3. Create a new branch
 4. Make your changes on this branch
 5. Stage and commit those changes
 6. Push your branch on your GitHub repository
 7. Open a pull request
 8. That's it after merging/approving 😍your changes you are done.
 9. Stay up to date

### EXPLAINED CONTRIBUTION GUIDE

This project aims to simplify and guide the way beginners make their first contribution. If you are looking to make your first contribution, follow the steps below

\


<img align="right" width="300" src="https://user-images.githubusercontent.com/79048275/193631517-6264abc8-9c63-460e-8325-9987f1ad3cfc.jpg" alt="fork this repository" />

#### If you don't have git on your machine, [install it](https://help.github.com/articles/set-up-git/).

## Fork this repository

Fork this repository by clicking on the fork button on the top of this page.
This will create a copy of this repository in your account.

## Clone the fork from your repository

<img align="right" width="300" src="https://user-images.githubusercontent.com/79048275/193632205-b048edea-5b43-41e0-bb41-6d56dc325bef.jpg" alt="clone this repository" />

Go to your GitHub account, open the forked repository, click on the code button and then click the _copy to clipboard_ icon.
Now clone the forked repository to your LocalHost.

Open a terminal and run the following git command:

```
git clone "URL of forked repository"
```

(without the quotation marks)
(your fork of this project)


## Create a branch

Change to the repository directory on your computer (if you are not already there):

```
cd intellimixio
```

Now create a branch using the `git checkout` command:

```
git checkout -b your-new-branch-name
```

For example:

```
git checkout -b hacktober2022
```

## Make necessary changes and commit those changes

If you go to the project directory and execute the command 

`git status`, 
you'll see there are changes.

#### The Red there is to be commited / that are the changes which are not pulled to main/master or any other branch.

So Lets add those changes with these command lines:
`git add` 
or 
`git add -A`

Now commit those changes using the `git commit` command:

```
git commit -m "<Your commmit message>"
```
## Push changes to GitHub

Push your changes using the command `git push`:

```
git push origin -u <add-your-branch-name>
```

replacing `<add-your-branch-name>` with the name of the branch you created earlier.

<details>
<summary> <strong>If you get any errors while pushing, click here:</strong> </summary>

- ### Authentication Error
     <pre>remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
  remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
  fatal: Authentication failed for 'https://github.com/<your-username>/first-contributions.git/'</pre>
  Go to [GitHub's tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) on generating and configuring an SSH key to your account.

</details>

## Submit your changes for review

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

<img align="right;" src="https://user-images.githubusercontent.com/79048275/193634497-6efe62ab-c929-4cd1-9bd8-19baf235b95f.png" alt="create a pull request" />

Now submit the pull request.

<img align="right;" src="https://user-images.githubusercontent.com/79048275/193635119-06dd2024-5c3f-4977-9576-3e76f87e268f.png" alt="submit pull request" />

Soon Our team will be merging all your changes into the master/main branch of this project. You will get a notification email once the changes have been merged.


*Thank You*
