# Clone your project from Github

The goal here is to migrate the code made available at the [the GitHub Xamarin.DevOps repository](https://github.com/DXPortugal/Xamarin.Devops) into Visual Studio Team Services.
 
 > Note: VSTS supports Github, SVN or external Gits. You can even create your Continous Integration directly from this repos.

1. Open Your Visual Studio and connect to your VSTS repo

2. Clone the repo by clicking the “Clone this repository” link:

3. Open up Command Prompt in the “Changes” window and “Actions:” 

4. Then, add a remote for the GitHub repo. If we ever need to pull down commits from the repo that are located on GitHub, we can do that by pulling from the remote name rather than the long GitHub URL. The command is: 

   `git status`  

   `git remote add Github https://github.com/DXPortugal/Xamarin.Devops.git`  

   >Note: The name Github is case sensitive and is merely a name you can change. 

5. Check your remote configuration 

   `git remote -v`  

6. To pull down your changes from that new remote you just added: 

   `git pull Github master`  

7. And don’t forget to push your changes from your local repo up to the Visual Studio Team Services server (which is origin by default):

   `git push origin master`  

Check out the result of pulling down from GitHub and pushing up to the Visual Studio Team Services repo:

## Next

[Lab 1.3](https://github.com/DXPortugal/Xamarin.Devops/blob/master/lab13.md) - Create your Android Build Definition

