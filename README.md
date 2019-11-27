# What is Securus?

An open source implementation of a secured methodology to sign-in to any system/website without the need to key in password. Passwords are challenges.

Without the need to be tied down to Google, FB or other social media which becomes a target.

Even if the Securus is comprimised, its' database cannot be used without the Enigma key because the key changes every 12 hours. Or if compromised is known, immediate change to the key is activated.

# Reference design

1. Enigma design
2. OAuth

## Long term goal

Get other websites to implement this feature. This way every website will constantly change password and there'll be no fix password moving forward. Even if the database is hacked, but because the website is constantly changing and the website doesn't have the key to unlock then even if the password got hack but without the key, it's not possible to snatch it.

Another possible goal is to have a "Sign-up with Securus" similar to "Sign-up with Google"
then "Sign-in with Securus"

This will automatically select the most secure manner to sign in without the concern of security.

## Updates
### 27th Nov 2019

After some reviews on existing solutions, OAuth2 does meet all the criterias above. Unfortunately, the adoption of OAuth2 is still picking up. Most existing websites are still using traditional username and static password which is stored in the vendor's database.

After some brainstorming, it's *possible* that this project will change its' direction towards working around the issue on the lack of adoption of OAuth, then again, there's still a possibility to re-design or propose another implementation of open standard for a secured methodology around Authentication.

Possible workaround would be empowering the users the capability to host the OAuth themselves rather than depending on the merchants and vendors that doesn't bother about the security of the users. Users have to be awared and be empowered to take pro-active measures to secure themselves rather than depending on others. Implementation details are still in thought phase.
One way to approach this would be to implement a plugin or software that is able to detect the website's password and provide a dynamic password (token) and each time it changes the password, it'll reset the password for the given website. This approach is rather harsh as it means from the vendor's perspective, this is considered a "Lost your password" or "Forgotten your password" which is a not the desired output.

Reviewing the process and methodology taken by LastPass and DashLane, they seem to implement a method to auto-change password to several websites. Auto-change password. That's another interesting idea.