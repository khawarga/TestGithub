# Github Action and SmartMerge (Unityyamlmerge)

## How to use Unity Smart Merge

1. Download git for windows (https://gitforwindows.org/)
   
2. Right Click on the unity project directory and select Git Bash Here

![Screenshot 2023-12-01 165257](https://github.com/khawarga/TestGithub/assets/51886512/6ea1f222-f80f-41bf-b7b8-52964aa45edc)

3. Enter this command (check https://docs.unity3d.com/Manual/SmartMerge.html and search for the git section)
   For the path to unityyamlmerge you can search on your unity editor file (Unity Editor > your unity editor version > Editor > Data > Tools)
   
![Screenshot 2023-12-01 164923](https://github.com/khawarga/TestGithub/assets/51886512/60b9cca7-2e8d-402c-96ca-75f673c3e226)

4. Install tortoiseGit (https://tortoisegit.org/)

5. Change the setting of tortoise git (Right Click > Tortoise Git > Setting) to add .unity file extension
   Check the unity smart merge page and go to the tortoise git section
   
![image](https://github.com/khawarga/TestGithub/assets/51886512/f1fd6265-0bfd-4b39-adca-2752f5326f21)

6. Ready to use. To use it Git Bash on the unity project directory and write "git mergetool" and where there are a scene or prefab conflict the tortoise git will appear like the following image
   
   ![image](https://github.com/khawarga/TestGithub/assets/51886512/4eae99f3-7705-4042-b075-af59e680d680)

    You just need to choose which line to use and save the change.

if you are still confused please check the following tutorial (this guide is based on these)

https://youtu.be/ZI7Uz-VnO8U?si=4t07W4WmmxT4x33q
https://www.andreasjakl.com/resoving-unity-scene-merge-conflicts-unityyamlmerge-tortoisegit/

## How To activate github action

### 1. Activation

a.	Make and run the acquire activation license on github action
    you can get the activation action code on https://game.ci/docs/3/github/activation

b.	Download the artifact after the action completed

![image](https://github.com/khawarga/TestGithub/assets/51886512/79687a61-c4d1-49fc-b06f-3a61067e94ff)

c.	Go to https://license.unity3d.com/manual and enter your .alf file

d.	On activate your license step, inspect the page and delte the style = “display : none,” so the personal license option appear

![image](https://github.com/khawarga/TestGithub/assets/51886512/520d3222-9872-4213-9ec3-073595c1a187)

![image](https://github.com/khawarga/TestGithub/assets/51886512/ce0d28eb-d723-4acb-8a8c-f055fc45f523)
 
e.	Then download the license file

![image](https://github.com/khawarga/TestGithub/assets/51886512/fe55b890-fcfa-4f6b-b5e5-9a9800c9619d)
 
f.	Go to your project on Github then go to Setting > Secret

![image](https://github.com/khawarga/TestGithub/assets/51886512/fb45b9c6-3c92-494f-b001-49e3e4059fb8)

And make the following secret

-	UNITY_LICENSE - (Copy the contents of your license file (.ulf file) into here)
-	UNITY_EMAIL - (Add the email address that you use to login to Unity)
-	UNITY_PASSWORD - (Add the password that you use to login to Unity)

### 2. Build Automation

a.	Make and run the build action on github action
    you can get the build action code on https://game.ci/docs/github/builder

b.	The Action must be in queue and working after you push the change, if doesn’t work check your secret and make sure you already push the latest change to your github

c.	After the action finish you can download the build on artifact section

![image](https://github.com/khawarga/TestGithub/assets/51886512/678d1995-8f35-4062-8647-a273a29d77c0)

