# MirrarSdk

Jewellery try-on Mirrar Module by StyleDotMe

## Integration

Follow these steps-

1. Install mirrar-sdk from npm registry 
   ```npm i mirrar-sdk```

2.Run ```npm install```

3. Must provide camera permssion. Add this line in your Manifest.xml in android

   ```<uses-permission android:name="android.permission.CAMERA" />```

4. Add this line in your page   
```
<dev-custom-sdk
    username="" 
    password="" 
    jsonString=''>
  </dev-custom-sdk>
```

5. Import mirrar-sdk in page.module.ts and add this inside ngModule
  ```import { MirrarSdkModule } from 'mirrar-sdk';```

6. Allow camera permission by following these steps
https://ionicframework.com/docs/native/android-permissions

7. Mirrar-sdk requires two provider so import InAppBrowser and AndroidPermission inside app.module.ts
   ```import { InAppBrowser } from '@ionic-native/in-app-browser/ngx';```
    ```import { AndroidPermissions } from '@ionic-native/android-permissions/ngx'; ```
   and add these two inside providers.

8. Add these two tags in config.xml
    ```<allow-navigation href="*" />```
   ``` <allow-intent href="*" />```

