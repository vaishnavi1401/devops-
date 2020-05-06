**How to setup a Jenkins production and testing pipeline using docker?**

Assumptions: Jenkins And Docker are installed in RHEL OS

Jenkins is added in sudoers file.

User has a Github Profile and Git Bash is Installed

1\. Create a folder on your preferred place

2.Create a index.html file and write something it .

![](./media/image1.png)

4\. create a dev1 branch by Git branch dev1 and move to dev1 branch by
using git checkout dev1

![](./media/image2.png)6.

5.Edit the code in this branch

![](./media/image3.png). Add 6.and commit the code

Git add.

Git commit -m “message“

Git checkout master

![](./media/image4.png)

PART 2

Now we need to setup Jenkins for the job

Fire up Jenkins

Step 1:

Create Job1 for production server with following configuration

![](./media/image5.png)

![](./media/image6.png)

Save the job

STEP 2:

Create another job for development server ![](./media/image7.png)

![](./media/image8.png)

Save the job

Step 3

Create a job QAtesting

Don’t forget to give your credentials here

![](./media/image9.png)

\# go to advanced post build section

![](./media/image10.png)

THE TASK HAS BEEN COMPLETED

This is how the index page in branch looks

![C:\\Users\\HP\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\11.png](./media/image11.png)

This is what development server looks like

![C:\\Users\\HP\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\12.png](./media/image12.png)

Once the QA team test the code they will start the QATESTING

![C:\\Users\\HP\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\12.png](./media/image12.png)

This is what Docker looks like after this process

![C:\\Users\\HP\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\Capture.png](./media/image13.png)
