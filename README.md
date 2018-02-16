# KaoWallSdk is the simple library for KickAssOffers Wall

## Getting started

#### Gradle Dependency 

Google documentation for importing external libraries to your project: [here](https://developer.android.com/studio/projects/android-library.html#AddDependency)

Download [KickAssWallSdk](https://github.com/kickassoffers/offerwall/raw/master/library/kaowallsdk-r-v0.1.0.aar) and add to your project. After that modify your `build.gradle` file

```gradle
dependencies {
    implementation 'com.android.support:design:26.1.0'
    implementation files('libs/kaowallsdk-r-v0.1.0.aar')
}
```

### How to use
KickAssWallSdk provides a couple of ways to show the wall.

#### Method 1:
You may init the library in your main activity or applications in the following way:

```java
KaoWall.init(context, new KaoParamsBuilder(YOUR_AFFILIATE_ID).userId(YOUR_USER_ID).build());
```

and call the method 'show' there in a place where you want to open KickAssWall:

```java
KaoWall.show();
```

#### Method 2
You can init the library and show where you want to open KickAssWall

```java
KaoWall.show(context, new KaoParamsBuilder(YOUR_AFFILIATE_ID).userId(YOUR_USER_ID).build());
```

#### Params
YOUR_AFFILIATE_ID - Long

YOUR_USER_ID - String

context - also, may be an application context

To retrieve your affiiate ID, simply follow the below instructions:
1) Login to your affiliate account - http://partners.kickassoffers.com
2) Click "Offers"
3) Click "Offer Wall"
4) Under SDK Integration, you will see your affiliate ID


## Support
If you experience any issues with integration, please reach out to your affiliate manager or alternatively, you can email support@kickassoffers.com
