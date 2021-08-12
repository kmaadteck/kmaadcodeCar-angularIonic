## Build an Ionic angular App with multi-parts using cordova

# 1st Part => implementation of the Navigation with Login, Guards & Tabs Area

> # 1| Manage my authentication state (and API calls)

    ionic g service services/authentication

> # 2| Additional Pages

    ionic g pages pages/intro
    ionic g pages pages/login

> # 3| Secure inside area

    ionic g guard guards/auth --implements CanLoad

> # 4| Show intro automatically once

    ionic g guard guards/intro --implements CanLoad

> # 5| Automatically log in users

    ionic g guard guards/autoLogin --implements CanLoad
