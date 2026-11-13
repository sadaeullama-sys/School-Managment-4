School Management System — ZIP update notes (2026-11-13)

Changes made in this package:
1. Added School Management System launcher artwork at assets/school_management_launcher.png.
2. Added flutter_launcher_icons configuration and a GitHub Actions step to generate Android launcher icons during the build.
3. Incremented Android build version to 1.0.0+2 for the next Play upload.
4. Added the student's saved photo to the Fee Voucher PDF layout.
5. Added the student's saved photo to the DMC PDF layout. Both layouts show a PHOTO placeholder if no student photo is saved on this device.

Not completed in this package (requires further implementation and testing):
- Google Play reviewer/demo license bypass. No universal or hard-coded bypass key was added. A secure review-access flow must be designed and tested against the app's actual licensing model.
- Full enforcement of Staff View/Add/Edit/Delete permissions across all modules and cross-device Firebase synchronization. The existing README_UPDATE_STATUS_UR.txt already notes that permissions are stored/displayed but not connected to every module action. This limitation remains.

Important: This package has not been compiled in this environment because Flutter/Dart SDK is unavailable. Run the included GitHub Actions workflow and test the resulting APK/AAB on Android before uploading to Play Console. Keep the existing signing keystore/secrets unchanged so updates can be signed with the same upload key.
