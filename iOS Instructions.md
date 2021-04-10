# Build And Deploy IOS App

## Preparation

### if ionic app not configured

1. download the source from : https://github.com/mbash12/reverse/
   ![image-20200801141904494](iOS Instructions.assets/image-20200801141904494.png)

2. Extract downloaded ZIP file

3. Open Visual Studio Code

4. Open menu file, then click **Open Folder...** or **Open...**

5. Open folder from extracted zip file

6. Open embedded shell / terminal by pressing **CTRL** + **`** *(backtick)* key

7. Run this command : 

   ``` shell
   sudo npm install -g @ionic/cli
   sudo npm install -g @angular/cli
   npm install
   ```
   
### Prepare app

1. Open **config.xml**
   ![image-20200801143728719](iOS Instructions.assets/image-20200801143728719.png)

2. Change **id** on widget element match with **app code** in **licences manager**, 
   ![image-20200801143437358](iOS Instructions.assets/image-20200801143437358.png)

3. Change the **version** to higher than uploaded app version

4. Change **name** of the app inside <name> element

5. You can change other things, like **description**, author's **email**, author's **href** and **name** inside <author> element

6. Open **home.page.ts** inside **/src/app/home folder** 

7. change **appName** to match with **appCode**

   ![image-20200801144237501](iOS Instructions.assets/image-20200801144237501.png)

8. Run this commands :

   ```shell
   ionic cordova platform rm ios
   ionic cordova platform add ios
   ```

### Prepare content

1. Copy your **contents** folder to folder **assets** inside the **src** folder in the application folder
   ![image-20200801143035983](iOS Instructions.assets/image-20200801143035983.png)

   
   
## Build

### Ionic

1. Run this command :

   ```shell
   ionic cordova prepare ios
   ```

### XCode

1. Open xcode

2. Open menu file, click open

3. Find the **ios** folder inside **/platforms** folder
   ![image-20200801145430944](iOS Instructions.assets/image-20200801145430944.png)

4. Click open
   ![image-20200801145458123](iOS Instructions.assets/image-20200801145458123.png)

5. Click show the project navigator

6. Click the app 
   ![image-20200801145635057](iOS Instructions.assets/image-20200801145635057.png)

7. Select the app inside **TARGETS**
   ![image-20200801145833372](iOS Instructions.assets/image-20200801145833372.png)

8. In **General** tab you can change these information if there are some correction
   ![image-20200801145914373](iOS Instructions.assets/image-20200801145914373.png)

9. Click **Build Settings** tab

10. Find for **Signing** section, change the release to **iOS Developer**
      ![image-20200801150105075](iOS Instructions.assets/image-20200801150105075.png)

11. Click **Signing & Capabilities** tab and select the **Team**
      ![image-20200801150418928](iOS Instructions.assets/image-20200801150418928.png)

12. You can test the app first before uploading the app to the store

    1. change the simulator to any device you want to test, or you can plug the real device and select it
       ![image-20200801150604570](iOS Instructions.assets/image-20200801150604570.png)

    2. Click play icon to start simulation
       ![image-20200801150651583](iOS Instructions.assets/image-20200801150651583.png)

    3. And click stop to end the simulation
       ![image-20200801150727894](iOS Instructions.assets/image-20200801150727894.png)

13. If everything is ok, you can change the device to **Generic iOS Device**
      ![image-20200801150604570](iOS Instructions.assets/image-20200801150604570-1596269819266.png)

## Distribution

1. Open menu **Product** then click **Archive**
      ![image-20200801150902397](iOS Instructions.assets/image-20200801150902397.png)
      ![image-20200801151010194](iOS Instructions.assets/image-20200801151010194.png)

2. Click **Distribute App**

3. Select **App Store Connect**, then click **Next**
    ![image-20200801151147007](iOS Instructions.assets/image-20200801151147007.png)

4. Select **Upload** then click **Next**
    ![image-20200801151235839](iOS Instructions.assets/image-20200801151235839.png)

5. Click **Next**
    ![image-20200801151309924](iOS Instructions.assets/image-20200801151309924.png)

6. Select **Automatically manage signing**, then click next
    ![image-20200801151345914](iOS Instructions.assets/image-20200801151345914.png)

7. Click **Upload**
    ![image-20200801151451060](iOS Instructions.assets/image-20200801151451060.png)


