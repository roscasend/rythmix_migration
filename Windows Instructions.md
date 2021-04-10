# Build Windows App

## Preparation

### Prepare the app

1. 

   ``` shell
   sudo npm install -g electron
   npm install
   ```
   
2. Open **package.json** you can change certain information below
   ![image-20200804215257595](./Windows_Instructions.assets/image-20200804215257595.png)

3. Change **appId** on widget element match with **app code** in **licences manager**, 
   ![image-20200801143437358](./Windows_Instructions.assets/image-20200801143437358.png)

3. Change the **version** to higher than uploaded app version

4. Change **productName** if it's different product

6. Open **index.js** inside **/assets** Folder

7. change **appName** to match with **appCode**

   ![image-20200804215817634](./Windows_Instructions.assets/image-20200804215817634.png)


### Prepare content

1. Copy your **contents** folder 
   ![image-20200804215951880](./Windows_Instructions.assets/image-20200804215951880.png)
2. Adjust font size, list height etc inside settings.json

## Build

1. Run this command :

   ```shell
   yarn dist
   ```

2. Location of the **exe** which you can install to windows computer
   ![image-20200804220106995](./Windows_Instructions.assets/image-20200804220106995.png)
