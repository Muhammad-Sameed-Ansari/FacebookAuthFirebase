# Facebook Sign In Firebase React Native Expo

## app.json
In the **app.json** file under the iOS add the **bundleIdentifier** key for the iOS app. And for the android app add the **package** key under android. The value of the **bundleIdentifier** and **package** should be same.

## Meta For Developers
First of all you have to go to 
```
developers.facebook.com
```

Then go to **My Apps**. If you are not signed in then first of all you have to sign into meta for developers. Then go to **Create App**. 

Then in the **Select an app type** select **Consumer** as we have to use it for customer facbook login. Then hit next.

Then provide the basic information about the app. That is enter the app name and the email address. And then hit create app and the app will be created.

Then under the **Add products to your app** add the Facebook Login product by clicking the **Set up** on it.

#### iOS App
For **Bundle ID**, first go to **app.json** file and get the **bundleIdentifier** value and paste it in Bundle ID. Skip all the other steps. No need to add or change anything else in other steps.

## Firebase
Make a project in Firebase and make the **web app** in it. And make a new file **firebase.js** in the root directory of your project and paste the code of the **SDK setup and configuration** in it.

Now go to Authentication and add the Facebook Sign-in method. Now we have to provide the **App ID** and **App secret**. Both the values will be get from the project we have made in **Meta for Developers**.

For **App ID**. Go to App Dashboard
![](readmeImages/1.png)

Then for the **App secret**. Go to Settings > Basic
![](readmeImages/2.png)

Then copy the **OAuth redirect URI** given under the **App secret**. Then go to **Meta for Developers** Facebook Login > Settings, and add it over there.
![](readmeImages/3.png)