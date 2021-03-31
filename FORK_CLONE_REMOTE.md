# Fork, Clone & Remote


## Fork

<b> Note: </b> <i>This is only needed if you want to contribute to the project.</i>

If you want to contribute to the project you will have to create your own copy of the project on GitHub. You can do this by clicking the <b>Fork</b> button that can be found on the top right corner of the landing page of the repository. 

For example:

![image](https://user-images.githubusercontent.com/25927257/112403868-79d2b080-8ccc-11eb-9212-dbd70cf3326e.png)


## Clone

<b> Note: </b> <i>For this you need to install [git](https://git-scm.com/) on your machine. You can download the git tool from [here](https://git-scm.com/downloads).</i>

* If you have forked the project, run the following command -

```
git clone https://github.com/YOUR_GITHUB_USER_NAME/<Respository_Name> 
```

where ```YOUR_GITHUB_USER_NAME``` is your GitHub handle and ```<Project_Name>``` is name of Project you are trying to Clone.

* If you haven't forked the project, run the following command 

```
git clone https://github.com/anitab-org/<Project_Name>
```

```<Project_Name>``` is name of Project you are trying to Clone, for example, mentorship-backend

## Remote

<b> Note:</b> <i>This is only needed if you want to contribute to the project.</i>

When a repository is cloned, it has a default remote named ```origin``` that points to your fork on GitHub, not the original repository it was forked from. To keep track of the original repository, you should add another remote named upstream. For this project it can be done by running the following command -

```git remote add upstream https://github.com/anitab-org/<Project_Name>```

You can check that the previous command worked by running ```git remote -v``` . You should see the following output:

```
$ git remote -v
origin  https://github.com/YOUR_GITHUB_USER_NAME/<Project_Name> (fetch)
origin  https://github.com/YOUR_GITHUB_USER_NAME/<Project_Name> (push)
upstream        https://github.com/anitab-org/<Project_Name>.git (fetch)
upstream        https://github.com/anitab-org/<Project_Name>.git (push)
```
