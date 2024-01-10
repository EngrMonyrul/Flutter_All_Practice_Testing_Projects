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

- If you face any problem to setup firebase in your project like below, then -

```Terminal
firebase : File C:\Users\dell\AppData\Roaming\npm\firebase.ps1 cannot be loaded because running scripts is disabled on this system. For more information, see about_Execution_Policies 
at https:/go.microsoft.com/fwlink/?LinkID=135170.
At line:1 char:1                                 
+ firebase login                                 
+ ~~~~~~~~                                       
    + CategoryInfo          : SecurityError: (:) [], PSSecurityException
    + FullyQualifiedErrorId : UnauthorizedAccess
```

- Then,
    1. Check current execution policy
        ```Powershell
       Get-ExecutionPolicy
       ```
    2. If it's not remote then change
        ```Powershell
       Set-ExecutionPolicy RemoteSigned
       ```
    3. After sign in make it restriction
        ```Powershell
       Set-ExecutionPolicy Restricted
       ```