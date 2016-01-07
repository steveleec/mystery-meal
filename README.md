# Mystery Meal - A new way of discovering food
Thesis project at MKS-20 implemented by using React, React-Native and Relay.

##When instaling Camera Roll Feature (needed for both cameraroll and live features)
1. In XCode, go to your `Project` ➜ `Libraries` ➜ `React.xcodeproj` ➜ `React` ➜ `Base`
2. Right click on `Base` and select `New File...`
3. Select `Objective-C File` and click `Next`
4. Name the file **RCTCustom.m** and click `Next`
5. Change the file contents to [this file](https://raw.githubusercontent.com/scottdixon/react-native-upload-from-camera-roll/master/RCTCustom.m)
6. Press `Enter` after @end to create a newline (XCode specific syntax rule)
7. `Save`

##After doing an npm install, In react-native-fbsdk-cor/js-modules/FBSDKGraphRequest.ios.js:
Change line 121 to be FBSDKGraphRequestManager.batchRequests([this], function(){}, timeout)

##When using the app font system
###San Francisco Display
- fontFamily: 'SanFranciscoDisplay-Light'
- fontFamily: 'SanFranciscoDisplay-Regular'
- fontFamily: 'SanFranciscoDisplay-Semibold'

###San Francisco Text
- fontFamily: 'SanFranciscoText-Regular'
- fontFamily: 'SanFranciscoText-RegularItalic'
- fontFamily: 'SanFranciscoText-Medium'
- fontFamily: 'SanFranciscoText-Semibold'

##Color Guide
These are located within the globalVariables.js file at the root of the directory. Just require either the whole set or choose which ones...

![Colorguide](https://s3-us-west-2.amazonaws.com/mystery-meal/color-guide.png)

##Icon Guide
The available icons are located [here](http://ionicons.com/). To see the name you use, just click on one and it's the words after the 'ion'.

```
var { Icon, } = require('react-native-icons');

<Icon
  name='ion|beer'
  size={30}
  color='#887700'
  style={styles.beer}
/>
```

Do note, you must explicitly include the width and height in the styles for the icon. so for this instance it would be...

```
styles = StyleSheet.create({
  beer: {
    width: 30,
    height: 30
  }
});
```

Screen Images
-------------
<p align="center">

  <img src='https://s3-us-west-1.amazonaws.com/portfoliostevem/mystery-screen-1.png?X-Amz-Date=20160107T190158Z&X-Amz-Expires=300&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Signature=95a392d5c851d2ae5a20dbda81268d1ad03b0d99ee8951c0a1e7e4ae61a144c7&X-Amz-Credential=ASIAIQVHZF5I2CP4SDTQ/20160107/us-west-1/s3/aws4_request&X-Amz-SignedHeaders=Host&x-amz-security-token=AQoDYXdzEJT//////////wEakAKD5N15U7V08n1tDVwBxTqQ07T%2Bz3F3FkyWAFu7Tn2j1gHwThk7snjkVDfyDpHFC/tJIL7sRkifoPP//u20uAqCoISo9j9F57JK7/WGkkXDYYKXoarFZvhn17Em%2BESzkO25wZhDb6pDt1WVv9dm5vuyj3j7XTPWj3CgcCExo6K3p%2B3iHbDXeuBCjrQGPF1stP%2Bb51P3pnsyQRTHU4z/ODradjDmn1M80idLkYZQrGb3Nk2uJwQ%2BDCoRXB9s6K0sdq1VKugjULjWjcqW1zQPuGeVFOfgR//Hnql7424x5iy8cnhUBDe2zdDhJrudpBR7aSJfby0K7dFxArOFZUxaN30FQuaguzV1jBI8j3wkEnWCKSD33rq0BQ%3D%3D' width='250'>

  <img src='https://s3-us-west-1.amazonaws.com/portfoliostevem/mystery-screen-2.png?X-Amz-Date=20160107T190218Z&X-Amz-Expires=300&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Signature=91b16beead507e571b120c54130931e925c8bc21b628297c7e21916b316d6d43&X-Amz-Credential=ASIAIQVHZF5I2CP4SDTQ/20160107/us-west-1/s3/aws4_request&X-Amz-SignedHeaders=Host&x-amz-security-token=AQoDYXdzEJT//////////wEakAKD5N15U7V08n1tDVwBxTqQ07T%2Bz3F3FkyWAFu7Tn2j1gHwThk7snjkVDfyDpHFC/tJIL7sRkifoPP//u20uAqCoISo9j9F57JK7/WGkkXDYYKXoarFZvhn17Em%2BESzkO25wZhDb6pDt1WVv9dm5vuyj3j7XTPWj3CgcCExo6K3p%2B3iHbDXeuBCjrQGPF1stP%2Bb51P3pnsyQRTHU4z/ODradjDmn1M80idLkYZQrGb3Nk2uJwQ%2BDCoRXB9s6K0sdq1VKugjULjWjcqW1zQPuGeVFOfgR//Hnql7424x5iy8cnhUBDe2zdDhJrudpBR7aSJfby0K7dFxArOFZUxaN30FQuaguzV1jBI8j3wkEnWCKSD33rq0BQ%3D%3D' width='250'>

  <img src='https://s3-us-west-1.amazonaws.com/portfoliostevem/mystery-screen-3.png?X-Amz-Date=20160107T190237Z&X-Amz-Expires=300&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Signature=9df141f2f29de731867366f104b7223817926bb3d22ae89319f3d9f932834fec&X-Amz-Credential=ASIAIQVHZF5I2CP4SDTQ/20160107/us-west-1/s3/aws4_request&X-Amz-SignedHeaders=Host&x-amz-security-token=AQoDYXdzEJT//////////wEakAKD5N15U7V08n1tDVwBxTqQ07T%2Bz3F3FkyWAFu7Tn2j1gHwThk7snjkVDfyDpHFC/tJIL7sRkifoPP//u20uAqCoISo9j9F57JK7/WGkkXDYYKXoarFZvhn17Em%2BESzkO25wZhDb6pDt1WVv9dm5vuyj3j7XTPWj3CgcCExo6K3p%2B3iHbDXeuBCjrQGPF1stP%2Bb51P3pnsyQRTHU4z/ODradjDmn1M80idLkYZQrGb3Nk2uJwQ%2BDCoRXB9s6K0sdq1VKugjULjWjcqW1zQPuGeVFOfgR//Hnql7424x5iy8cnhUBDe2zdDhJrudpBR7aSJfby0K7dFxArOFZUxaN30FQuaguzV1jBI8j3wkEnWCKSD33rq0BQ%3D%3D' width='250'>

  <img src='https://s3-us-west-1.amazonaws.com/portfoliostevem/mystery-screen-4.png?X-Amz-Date=20160107T190245Z&X-Amz-Expires=300&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Signature=ecd1922cf8c3d9a594fc7406a15ea99e21fcf21bd3c6ddc4d843dfc9510ea7e6&X-Amz-Credential=ASIAIQVHZF5I2CP4SDTQ/20160107/us-west-1/s3/aws4_request&X-Amz-SignedHeaders=Host&x-amz-security-token=AQoDYXdzEJT//////////wEakAKD5N15U7V08n1tDVwBxTqQ07T%2Bz3F3FkyWAFu7Tn2j1gHwThk7snjkVDfyDpHFC/tJIL7sRkifoPP//u20uAqCoISo9j9F57JK7/WGkkXDYYKXoarFZvhn17Em%2BESzkO25wZhDb6pDt1WVv9dm5vuyj3j7XTPWj3CgcCExo6K3p%2B3iHbDXeuBCjrQGPF1stP%2Bb51P3pnsyQRTHU4z/ODradjDmn1M80idLkYZQrGb3Nk2uJwQ%2BDCoRXB9s6K0sdq1VKugjULjWjcqW1zQPuGeVFOfgR//Hnql7424x5iy8cnhUBDe2zdDhJrudpBR7aSJfby0K7dFxArOFZUxaN30FQuaguzV1jBI8j3wkEnWCKSD33rq0BQ%3D%3D' width='250'>

  <img src='https://s3-us-west-1.amazonaws.com/portfoliostevem/mystery-screen-5.png?X-Amz-Date=20160107T190252Z&X-Amz-Expires=300&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Signature=b092c3a678d0e5a3feb6b1347b3faa59970de6eee067f93c1e534518b77f1109&X-Amz-Credential=ASIAIQVHZF5I2CP4SDTQ/20160107/us-west-1/s3/aws4_request&X-Amz-SignedHeaders=Host&x-amz-security-token=AQoDYXdzEJT//////////wEakAKD5N15U7V08n1tDVwBxTqQ07T%2Bz3F3FkyWAFu7Tn2j1gHwThk7snjkVDfyDpHFC/tJIL7sRkifoPP//u20uAqCoISo9j9F57JK7/WGkkXDYYKXoarFZvhn17Em%2BESzkO25wZhDb6pDt1WVv9dm5vuyj3j7XTPWj3CgcCExo6K3p%2B3iHbDXeuBCjrQGPF1stP%2Bb51P3pnsyQRTHU4z/ODradjDmn1M80idLkYZQrGb3Nk2uJwQ%2BDCoRXB9s6K0sdq1VKugjULjWjcqW1zQPuGeVFOfgR//Hnql7424x5iy8cnhUBDe2zdDhJrudpBR7aSJfby0K7dFxArOFZUxaN30FQuaguzV1jBI8j3wkEnWCKSD33rq0BQ%3D%3D' width='250'>

  <img src='https://s3-us-west-1.amazonaws.com/portfoliostevem/mystery-screen-8.png?X-Amz-Date=20160107T190354Z&X-Amz-Expires=300&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Signature=a87401ca8005b4f63024576b05bd9758f6f7e6728de36da73af2da835c4a02e2&X-Amz-Credential=ASIAIQVHZF5I2CP4SDTQ/20160107/us-west-1/s3/aws4_request&X-Amz-SignedHeaders=Host&x-amz-security-token=AQoDYXdzEJT//////////wEakAKD5N15U7V08n1tDVwBxTqQ07T%2Bz3F3FkyWAFu7Tn2j1gHwThk7snjkVDfyDpHFC/tJIL7sRkifoPP//u20uAqCoISo9j9F57JK7/WGkkXDYYKXoarFZvhn17Em%2BESzkO25wZhDb6pDt1WVv9dm5vuyj3j7XTPWj3CgcCExo6K3p%2B3iHbDXeuBCjrQGPF1stP%2Bb51P3pnsyQRTHU4z/ODradjDmn1M80idLkYZQrGb3Nk2uJwQ%2BDCoRXB9s6K0sdq1VKugjULjWjcqW1zQPuGeVFOfgR//Hnql7424x5iy8cnhUBDe2zdDhJrudpBR7aSJfby0K7dFxArOFZUxaN30FQuaguzV1jBI8j3wkEnWCKSD33rq0BQ%3D%3D' width='250'>

</p>

License
-------

MIT, see LICENSE.
