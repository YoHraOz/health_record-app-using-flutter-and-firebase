To use Firebase Storage ....go to firebase and register your app name by giving name same as applicationId under app-level/build.gradle delete the google-services.jason file which is already their in android/app/google-services.jason and replace it with the one you download from firebase while registering your app In firebase Storage change rules to :

rules_version = '2'; service firebase.storage { match /b/{bucket}/o { match /{allPaths=**} { allow read, write; } } }

And you are good to go