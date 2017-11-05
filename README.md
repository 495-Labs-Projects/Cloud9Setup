# Cloud 9 Setup
Setup instructions for using Cloud 9 for 67-272 Application Design and Development at Carnegie Mellon University.

This semester in 272, we will be using a new, online, platform called [Cloud 9](https://c9.io/) to build and run our web applications. This allows people on Windows, Mac, or Linux to run code in the same environment which will dramatically reduce time and frustrations on installing different pieces of software. Also, because of a standardized environment, the TAs can be more helpful in issues that may arise in building code.

## Step 0: Registration
You should have already received an email to join the 67-272 labs and 67-272 projects teams on Cloud 9. If this is not the case, please post on Piazza!

Once you do get these emails, please create an account on Cloud 9 if you have not done so by following the link in the email.

**NOTE THAT AFTER JOINING A TEAM, YOU WILL GET AN EMAIL TO SET YOUR PASSWORD, PLEASE DO SO!**

## Step 1: Creating a New Workspace

After registering or signing in, you should notice a home dashboard which looks like the following:
![Cloud 9 Home Dashboard](https://i.imgur.com/iZ6KVMq.png)

**Click on the *Create a new Workspace* panel** to start creating a new workspace. You should now see a screen similar to this one:
![Cloud 9 New Workspace Form](https://i.imgur.com/UZY99ST.png)

Here is a bit more about each setion of the form:

1. Adding a project name and description. Note that the project name can only have lowercase letters, numbers, underscores and dashes.

2. Choose a team for this project. If it is a lab assignment, please choose 67-272 Labs, otherwise choose 67-272 Projects.

3. **Please make sure the workspace is private! If it is not you are in danger of violating Academic Integrity**

4. One nice feature of Cloud 9 is to be able to import straight from a remote git repository. USe the HTTPS link from the Github repository you wish to start from if you wish to start from some starter code (recommended).

5. Make sure you are using the Ruby template.

You can now click the Create Workspace button to create the workspace.

## Step 2: Within the IDE

Now that the workspace has been created, you should see the Cloud 9 IDE, similar to below:

![Cloud 9 IDE](https://i.imgur.com/J1HCrqF.png)

On the left, you can view the directory for your files. On the bottom is a live linux terminal connected to your workspace.

Now there are a few small things that must be done within the IDE before we can continue coding.

1. As of now, Cloud 9 uses a default Ruby version of 2.3.4, but for 272 we will be using 2.4.1. **From the terminal, run** `rvm install 2.4.1`, **and then** `rvm use 2.4.1` **to switch Ruby versions to 2.4.1**. This should take about 1-2 minutes at most.

2. Once that is complete, **run** `gem install rails` **from the terminal** to get Rails.

3. After Rails is installed, **click on Cloud 9 in the top-left corner and select *restart workspace*** to restart the workspace. This cleans out any dependencies to Ruby 2.3.4.

Now we are ready to start working on our Rails project in Cloud 9!

## Step 3: Starting the Server
Once you are ready to run the rails server, note that in Cloud 9, **do not simply type** `rails server` **into the terminal** (since the container will not route the application as expected). Instead, **select the *Run Project* button on the top bar of the IDE** to run your project. A new terminal tab will open and display the URL to visit to view your application!

Now you are ready to develop in the cloud with Cloud 9! Please contact a professor or TA if there are further issues with using Cloud 9 in 272!
