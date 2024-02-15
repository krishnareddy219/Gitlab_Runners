## INSTALLATION OF GITLAB_RUNNERS

### GROUP_RUNNERS : Only owner have the access to create Group runners.
* Installation of runner on windows :
 [Refer here](https://docs.gitlab.com/runner/install/windows.html)
 * Create a folder and copy the downloaded amd_64 exe file then open poweshell in Run as admin mode.
![Image](pics/image1.png)
 * We can use the below commands:

 ```
  cd C:\GitLab-Runner(created folder)
.\gitlab-runner.exe install
.\gitlab-runner.exe start
 ```
 ![Image](pics/image2.png)

 ![Image](pics/image7.png)
 
 ![Image](pics/image8.png)

 * Go to gitlab in the particular group with owner access click on the build section in the runners create a new group runner.
 [Refer here](https://docs.gitlab.com/ee/ci/runners/runners_scope.html#group-runners)
 ![Image](pics/image3.png)
 * After creating runner register the runner with below commands:

 ```
.\gitlab-runner.exe register  --url https://gitlab.com  --token glrt-Cjsg9jCrNFHu1Xzp7PAF 
.\gitlab-runner.exe run
 ```
Note: Everytime token generates with new runner creation.
![Image](pics/image4.png)

![Image](pics/image5.png)

![Image](pics/image6.png)

