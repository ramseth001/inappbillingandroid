# Inappbillingandroid

1. Don't use the default company domain name when creating the project especially the word example. In my case, it's com.image.ram.inappbillingandroid 
2. Download Google Play Billing Library from Android SDK Manager. In IntelliJ, it can be opened from Tools -> Android
3. Once downloaded, you can find the path /android-sdk-macosx/extras/google. Create a new directory named aidl under src/main. Create a package com.android.vending.billing under the aidl folder. Copy the IInAppBillingService.aidl from the above mentioned path and paste it in the com.android.vending.billing package.
4. Build your program
5. Create a package util under src/main/java/com.image.ram.inappbillingandroid. You can find util files under /android-sdk-macosx/extras/google/play_billing/samples/TrivialDrive/src/com/example/android/trivialdrivesample/util. Copy files from that location and paste in the newly created package util.
6. To test the project, if you are using third party emulators, make sure you have google play services in it and you are signed into the google play
7. The aim of the project would be purchase an image. Once an image is purchased, it would be disappeared in 5 seconds. And hence need to purchase again. When an image is purchased, the BuyImage button would be disabled. After 5 seconds, it would be enabled again.
8. The code is given for the inapp billing to work.
9. android.test.purchased is the default SKU. This SKU can be used to test the code. For real SKUs, a different SKU names should be used.
10. A line in security.java file (as commented in the code) should be enabled to allow the android.test.purchased to be tested.
11. A signed APK file should be uploaded to the developer console for the code to be tested. (for actual SKUs)
