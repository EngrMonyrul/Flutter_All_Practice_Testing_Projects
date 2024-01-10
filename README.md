# Firebase setup in project

- Setup firebase project from
  console ([Firebase](https://firebase.google.com/?gad_source=1&gclid=Cj0KCQiAnfmsBhDfARIsAM7MKi2dd6gEoZruJD8zCmwAo2BnN5AB8XpPMO_bMXppcbnii3QkVMxRn_waAvysEALw_wcB&gclsrc=aw.ds))
    1. Active project authentication using google
        ![Google Image](https://play-lh.googleusercontent.com/1-hPxafOxdYpYZEOKzNIkSP43HXCNftVJVttoo4ucl7rsMASXW3Xr6GlXURCubE1tA=w3840-h2160-rw)

- Setup firebase into flutter project

    1. Install firebase in app
       1. Firebase login
        ```Terminal
         firebase login
        ```
       2. Active cli
        ```Terminal
         dart pub global activate flutterfire_cli
        ```
       3. Firebase config
        ```Terminal
         flutterfire configure
        ```
       4. Select database
       5. Select platform