# codepath-prework
# IOS101 Pre-work: Introducing Xcode

Welcome to the prework for **IOS101: Intro to iOS Development**! This pre-work task will guide you through building a simple app using Xcode and Swift. If you are applying for a different course, please refer to its respective prework.

This task aims to introduce you to key components of CodePath's course and iOS development. Firstly, we'll download Xcode, become familiar with the Xcode IDE, and build a simple app. Following that, you'll brainstorm some app ideas for your personal project in the second half of the course. Finally, you'll submit your completed work to CodePath.

By completing this task, you'll gain an understanding of building and running native iOS apps on simulators or your own iPhone. You'll also identify and resolve any issues with creating gif submissions and submitting assignments.

1. [Setup Xcode](#heading-1-setup-xcode)
2. [Familiarize yourself with Swift](#heading-2-familiarize-yourself-with-swift)
3. [Build Application](#heading-3-building-application)
4. [Planning ](#heading-4-planning)





## 1. Setup Xcode

<a href="https://itunes.apple.com/us/app/xcode/id497799835?mt=12#" alt="**Download Xcode from the Mac App Store**" title="**Download Xcode from the Mac App Store**" target="_blank">**Download Xcode from the Mac App Store**</a>

**NOTE:** Membership in the iOS Developer Program is **not** required. This program costs $99 a year and is only required if you want to distribute your apps in the App Store and have access to beta iOS releases.

## 2. Familiarize yourself with Swift

Learning Swift is essential to iOS development, but learning the nuances of its syntax will come with time and practice! There are many resources out there to learn Swift. We recommend taking a look at the following resources and bookmarking the Swift guides:


* Apple's <a href="https://docs.swift.org/swift-book/GuidedTour/GuidedTour.html" alt="**Official Swift Guide**" title="**Official Swift Guide**" target="_blank">**Official Swift Guide**</a>.
* CodePath's <a href="https://guides.codepath.com/ios/Understanding-Swift" alt="**Understanding Swift**" title="**Understanding Swift**" target="_blank">**Understanding Swift**</a>
* Download the <a href="https://www.apple.com/swift/playgrounds/" alt=" **Swift 5 Playground** " title=" **Swift 5 Playground** " target="_blank"> **Swift 5 Playground** </a> to experiment with the Swift 5 syntax.
* You can also find more resources <a href="https://developer.apple.com/swift/resources/" alt=" **here** " title=" **here** " target="_blank"> **here** </a>.


## 3. Building Application


### Let's begin developing!

:::info
**🙋 What if I need help!?**

Help is here!  If you encounter any issues while completing your prework, please join our [🚀 **prework Support Workspace**](http://www.codepath.org/preworkslack).<br/>

Advantages:
- Created to support applicants with prework completion difficulties.
- Help out your peers and learn from both peers and tech experts!
- Put your head together with other students encountering the same issue!

To join, just click the [🔗 **link**](http://www.codepath.org/preworkslack) and sign up with the same email you applied with.
:::

:::info
Expand the triangles below to collapse the tabs.
:::


<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 0: Setting up the Project 🏗 </summary>

- [x] Open Xcode and click "Create a new Xcode project"
- [x] Under the **"iOS"** Tab, click on **"App"**, then click "Next"
- [x] Name your project
- [x] Set the Interface to "Storyboard" and Language to "Swift"
- [x] Do not Use Core Data or Include Tests
- [x] Choose a location to save the project. *We recommend saving the project on your Desktop*

:::success
^^^
**Checkpoint #0**
^^^
<a href="/course_images/ios101/unit_0/Step0Setup.gif" target="_blank"><img src='/course_images/ios101/unit_0/Step0Setup.gif' title='Walkthrough of creating new project' width='' alt='Walkthrough of creating new project' /></a>
^^^
:::
</details>

<br>

<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 1: Exploring Xcode 🏗 </summary>

Now that we have our project set up, let's take a look at the Xcode IDE.

<a href="/course_images/ios101/unit_0/XcodeOverview.png" target="_blank"><img src='/course_images/ios101/unit_0/XcodeOverview.png' title='Xcode IDE' width='' alt='Xcode IDE' /></a>

There are primarily 5 sections of Xcode that we will be working with. All five are in the the screenshot. All of the areas the editor can be toggled hidden, so your view might initial appear differently.

1. **Project Navigator** - This is where you can see all the files in your project. You can also create new files and folders here. Additionally, you can find information about your project here such as the name of the app, the bundle identifier, and the version number.
2. **View Controller Scene**- This where you can see the UI elements that you have added to your app. As you add things to your "view controller" aka the screen you're looking at, you will see them appear here. They can be investigated further by clicking on them either in the view controller or the View Controller Scene. Play around with the menu options and explore the dropdown menus.
3. **Editor**- This is where you will be writing your code. By clicking on the file in the Project Navigator, you will see the editor change deepending on which file is clicked. The `AppDelegate`, `ViewController`, and `SceneDelegate` are Swift files, and as you create more of them later, they will have the same Swift/bird logo. If you see something like, `ViewController.swift`, that is the same as `ViewController` withot the `.swift` extension.  The `Main` file is where you will be adding UI elements to your app. The `LaunchScreen` is where you will be adding a launch screen to your app. The `Assets` is where you will be adding images to your app. As we build today's app, we'll primarily work in the `Main` file, and we'll also edit the `ViewController` file later.
4. **Utilities** - When you want to inspect how you can edit UI elements, you can click around the utilies panel to do things like, change your font, size of image views, etc. You can also change the constraints of your UI elements here. We will be using this later to change the constraints of our UI elements.
5. **Debug Area**- This is where you will see the output of your app. If you have any errors, they will appear here. If you want to print something to the console, you can do that here as well. We will be using this later to debug our app. This region is not pictured but appears from the bottom side when you run your app.




</details>

<br>

<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 2: Setting up the  UI 📱 </summary>

Now that we know where some important parts of Xcode resides, let's build our first simple app. We want to create a button that changes the background of our app to a random color.

- [x] Go to `Main` file and on the top right click the `+` to access the library of UI elements accessible to you.
- [x] Add three `Labels` and one `Button` anywhere on the screen
- [x] In the labels write your name, your university name, and either your current job or aspirational job.

^^^
**Adding UI Elements**
^^^
<a href="/course_images/ios101/unit_0/Step1UISetUp.gif" target="_blank"><img src='/course_images/ios101/unit_0/Step1UISetUp.gif' title='Adding four elements to our screen' width='' alt='Adding four elements to our screen' /></a>
^^^

As you can see, this is a very simple UI and we aren't doing anything fancy. The goal here is to introduce you to some UI elements and show you how simple it is to add things to our screen.

Now is a good time to run our app on a simulator. Although we get a preview on the `Main` file, it is always a good idea to run your app to see a more accurate depiction of how your layout looks.

- [x] At the top of Xcode, click on the right of your project name
- [x] Select any simulator and run your app

^^^
**Where?**
^^^
<a href="/course_images/ios101/unit_0/Step1Simulator.png" target="_blank"><img src='/course_images/ios101/unit_0/Step1Simulator.png' title='Selecting a simulator' width='' alt='Selecting a simulator' /></a>
^^^

After running your app you probably noticed it looks pretty plain. Let's make the button stand out a little bit more.

- [x] Select the button on `Main` and go to the Attributes Inspector (three horizontal lines) on the right hand side.
- [x] Change Background Configuration from `Default` to `Custom` and then change the fill to any color you would like.
- [x] Optionally, change the Foreground color as well.
- [x] Lastly, change the name to something else. Remember, this button will change our background color to a random color.

^^^
**Modifying Button**
^^^
<a href="/course_images/ios101/unit_0/Step1ButtonChanges.gif" target="_blank"><img src='/course_images/ios101/unit_0/Step1ButtonChanges.gif' title='Modifying button' width='' alt='Modifying button' /></a>
^^^

After running our app again we should have some color in our button.

:::success
^^^
**Checkpoint #1**
^^^
<a href="/course_images/ios101/unit_0/Step1Check.png" target="_blank"><img src='/course_images/ios101/unit_0/Step1Check.png' title='Running the app after step 1' width='' alt='Running the app after step 1' /></a>
You'll notice these messages appear on the leftside of Xcode. These messages are saying that your views will appear differently on different sized devices. We address this problem using auto-layout, but for now we ignore this warning and work on the functionality of our app. Warnings do not prevent your app from running, errors do.
^^^
:::


:::info
^^^
**What's this?**
^^^
<a href="/course_images/ios101/unit_0/Views.png" target="_blank"><img src='/course_images/ios101/unit_0/Views.png' title='Layout warning' width='' alt='Layout warning' /></a>
^^^
:::



</details>

<br>


<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 3: Connecting UI to Logic 🚠</summary>

The labels we created will hold static information about us, however, we want our button to change our background when we tap it. To do this, we need to write the logic in our `ViewController` Swift file. Then, we need to connect our logic to our UI so that the button acts as a gesture recognizer that triggers the logic.

- [x] Open the `Storyboard` file
- [x] Click on the `Adjust Editor Options` button on the top right of Xcode
- [x] Click on the `Assistant` in the drop down
- [x] `Control` + Drag from the button on storyboard to somewhere inside of the `ViewController` class
- [x] Name your IBAction `changeBackgroundColor`
- [x] Change the type form `Any` to `UIButton`

^^^
**Connecting Button to Logic**
^^^
<a href="/course_images/ios101/unit_0/Step2ConnectingButton.gif" target="_blank"><img src='/course_images/ios101/unit_0/Step2ConnectingButton.gif' title='Connecting the button' width='' alt='Connecting the button' /></a>
^^^

Note: If you need to edit the name of your `IBAction`, or set it again, you have to check your `Connections Inspector` on the right hand side of Xcode. You can't erase the code and retype it or else you will lose the connection.

^^^
**Where?**
^^^
<a href="/course_images/ios101/unit_0/Step2ConnectionsInspector.png" target="_blank"><img src='/course_images/ios101/unit_0/Step2ConnectionsInspector.png' title='Connections Inspector' width='' alt='Connections Inspector' /></a>
^^^

Now that we have connected our button to our logic, we can write the logic to change the background color.

- [x] Open the `ViewController.swift` file and under the `IBAction` you just created, write the following code:

```swift
    func changeColor() -> UIColor{

        let red = CGFloat.random(in: 0...1)
        let green = CGFloat.random(in: 0...1)
        let blue = CGFloat.random(in: 0...1)

        return UIColor(red: red, green: green, blue: blue, alpha: 0.5)
    }
```

Let's explore what is happening here here as we learn Swift syntax for the first time. We are creating a function, `changeColor()`, the empty parentheses indicate that this function does not take any parameters. The `-> UIColor` indicates that this function returns a `UIColor` object.

Inside of the function we are creating three variables, `red`, `green`, and `blue`. These variables are of type `CGFloat` which is a type of number that is used to represent colors. Think of RGB 0 to 255, but CGFloat normalizes this to 1. We are using the `random(in: 0...1)` function to generate a random number between 0 and 1. We are doing this for each of the three colors.

Lastly, we return a a UIColor where these three random numbers are used to create a color. The `alpha` parameter is used to indicate the opacity of the color. 1 is fully opaque, 0 is fully transparent.

Lastly, if we run our app now, nothing will happen. We need to call this function when the button is tapped.

- [x] Go back to the changeBackgroundColor IBAction and add the following two lines:

```swift
    let randomColor = changeColor()
    view.backgroundColor = randomColor
```


:::info
Why do we assign the function to a variable? Why not just call the function directly in the second line?

Three reasons:
1. **Readeability**; it is easier to read the code when you assign the function to a variable, especially as our code can become more complex.
2. **Reusability**: We can pass the variable into other functions if we need to.
3. **Debugging**: By storing the variable, we can print it out to the console to see what the value is or use the debugger to inspect its value and troubleshoot if the result appears diferent than intended.

For this particular use case, the approach is all that relevant since our app is simple, but it is good practice to practice good habits early on.
:::
</details>

<br>

<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 4: Summary 🧠 </summary>

<br>

^^^<span style="font-size:1.5em; font-weight: medium">📱 Final Product</span>^^^

<a href="/course_images/ios101/unit_0/FinalStep.gif" target="_blank"><img src='/course_images/ios101/unit_0/FinalStep.gif' title='Final Product' width='400' alt='Final Product' /></a>

^^^

Congrats! You have just finished building your first iOS app. You have learned how to create a new project, add UI elements, connect UI elements to logic, and run your app.

This is a great starting point to further out iOS development journey.


Copy and paste the following [README](readme_templates/project0_readme_template.md?raw=true) into your GitHub README and update with features you have implemeneted. 


###### Some ideas to improve the app are:

    - Improve the UI by using different fonts/colors/background
    - Feel free to play around with other elements, such as image views, textfields, etc.
    - Iplement a way to change the color of the text as well



</details>

<br>

## 4. Planning

At the bottom of your README, add a section called **App Brainstorming**. In this section, you will add the following:

- [x] Make a list of your favorite 3-5 applications and identify 2-3 features that make them your favorite app. Its okay if features repeat on different apps
  - Example App: **Instagram**
    - Changing the background color of the messages screen
    - Deleting old messages
- [x] Think of an app idea that you would like to build. It can be a new idea or an improvement on an existing app. Write a short paragraph describing the app and the features you would like to implement. You are not commiting to this idea, but it helps to start brain storming early on and get feedback from your peers and instructors.



## 5. Submit on the application dashboard

<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 1: Submission Checklist ✅ </summary>

The preworked is considered complete when:

- [x] User can run application showing a screen with a button and at least a couple of labels
- [x] The screen has a background color that can changes when the button is tapped


</details>

<br>

<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 2: Create a GitHub Repository 📕 </summary>

1. If you are unfamiliar with GitHub, watch this short introduction video -> <a href="https://www.youtube.com/watch?v=w3jLJU7DT5E" alt="**What is GitHub?**" title="**What is GitHub?**" target="_blank">**What is GitHub?**</a> *(3:32)*
2. Create Repository, Commit, and Push using GitHub Desktop (10min)
        <iframe width="560" height="315" src="https://www.youtube.com/embed/PvUexC0-D2s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    - ⚠️ **IMPORTANT:** You will now have to **re-open** your XCode project in the new repository folder location your moved it to to continue working on it!
    - **Want to learn more about GitHub?** Understanding GitHub is **a must** for tech professionals. Although we will be learning it more in class, we highly recommend to start getting familiarized with it :)

3. If you are comfortable working with the command line, follow the steps on **Linking to a Remote Repository** to push your project to GitHub.<a href="https://guides.codepath.com/ios/Using-Git-with-Terminal" alt="**Git + Terminal**" title="**Git + Terminal**" target="_blank">**Git + Terminal**</a>

</details>

<br>


<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 3: Submit through the application portal 🙌 </summary>

1. Head to the <a href="https://apply.codepath.org/dashboard" alt="**application dashboard**" title="**application dashboard**" target="_blank">**application dashboard**</a> and click the **SUBMIT** button in the *Pre-work Status* section.
<img src="https://i.imgur.com/WzXvbgU.png" height=400 /><br>

**NOTE:** If you can't find this section, try to log out of your GitHub, refresh the page, and then log back in.

1. Complete the submission form

- **Field 1:** Enter your app's GitHub repo URL
- **Field 2:** Enter the URL of your App walkthrough gif
  - Example: `https://i.imgur.com/my_walkthrough.gif`
      ^ Make sure your GIF link ends with `.gif`, otherwise it won't work!
        ^ You can test it in an *incognito/private mode* in your browser as well
- **Field 3:** Enter about how many hours you spent on the pre-work. (There is no right or wrong answer here)
- **Field 4:** Enter any additional info (optional).

1. Click the **Submit** button to submit your pre-work 👍

:::success
**🎉 Congratulations, you finished your first app! 🎉**
:::

When you've completed this, you'll hear from us soon with more information about the rest of the selection process. In the meantime, you can focus on **improving the functionality and user interface** of your app as outlined under **Bonuses!** section. While these remaining steps are optional, completing them will help you familiarize yourself with the coding environment, increasing your chances of thriving in the course. *However, the completion of these additional steps does not guarantee admission.*

</details>

<br>

## 6. Common Errors

<details>
<summary style="font-size:1.25em; font-weight: 600"> Error 1: GIF Not Showing 🙀</summary>

For the GIF to show, make sure that your link **contains** the file extension at the end (.gif)

Here is an example URL of how it should look:
`https://i.imgur.com/JL1snRo.gif`

^^ *Notice* the ***.gif*** extension at the end

On your readme md file, the markdown should look like this:
`![](https://i.imgur.com/JL1snRo.gif)`

We recommend using these tools to help you record GIFs on your computer:

:::warning

**GIF Recording Tools**

- <a href="https://getkap.co/" alt="**Kap**" title="**Kap**" target="_blank">**Kap**</a>
- <a href="https://gfycat.com/gifbrewery" alt="**GifBrewy**" title="**GifBrewy**" target="_blank">**GifBrewy**</a>

:::

</details>

<br>


<details>
<summary style="font-size:1.25em; font-weight: 600"> Error 2: GitHub Reference Error 🐙 </summary>

**ERROR: GitHub reference 'refs/heads/master' not found (-9)**

This problem has many solutions to it. Here a few links to help you fix it:

SOLUTIONS

1. https://stackoverflow.com/questions/30809205/couldnt-set-refs-heads-master-when-commit
2. https://stackoverflow.com/questions/33262304/cannot-resolve-git-xcode-7-repository-issue-commit-fails-error-building-trees
3. https://github.com/desktop/desktop/issues/3838#issuecomment-359297523

If those solutions don't work, you can create another GitHub repo and simply copy/paste your project in that repo folder.

</details>

<br>



<details>
<summary style="font-size:1.25em; font-weight: 600"> Error 3: Any issue with Outlets 🔌</summary>

If you removed/renamed and added new outlets, it is possible you're having errors. When removing old outlets you need to remove them entirely. Go to the outlets menu on the storyboard and verify that your outlets are connected correctly.

This can be caused when you create and delete a current outlet and create a new one.

The image below shows how an outlet is made correctly:

![](https://raw.githubusercontent.com/jonkykong/SideMenu/master/etc/Screenshot3.png)

The second image shows an outlet that was broken (first row with warning sign):

<a href="/course_images/ios101/unit_0/outleterror.png" target="_blank"><img src='/course_images/ios101/unit_0/outleterror.png' title='Oulets with a warning sign.' width='300' alt='Oulets with a warning sign.' /></a>

</details>

<br>


:::success
🎉 Congratulations, you've completed the prework! 🎉 <br/><br/>

You'll hear from us soon with more information about the rest of the selection process. In the meantime, feel free to explore further with Xcode and further familiarize yourself with the coding environment!
:::



**************


Name: Brenda Li
Email: brendali366@gmail.com

Description: This is the Prework for instroducing to the Codepath course.
Objective: To familiarize with some functions of Swift.

App Brainstorming: Favorite Apps

1. Instagram
    a. Able to see clips of all my interests.
    b. Communicating with friends and sharing clips.
    c. Easy to use and convenient. Does not require much focus.
2. Discord
    a. Get to join communities with similar interest.
    b. Simple way to communicate and interact with friends.
    c. A variety stickers to express mood and emotions.
3. Spotify
    a. Easy to navigate and group music.
    b. Convenient to use to listen to music.
    
App Idea:
    As a student, I get overwhelmed with assignments. It would be nice to have a easy to use app that shows all my assignments and things I need to do. Similar to a planner/agenda that is simple enough that it does not get cluttered and easy to use. You can create a checklist that lists all your assignments or tasks  that needs to be completed. You can move the items to put them in a order or importance. 
    
GIF:

[x](https://i.imgur.com/NqBAJDL.gif)
