# Clerk Social SignIn Issue

## Reproduce Steps

1 Installation

```shell
git clone git@github.com:asika32764/clerk-social-signin-issue.git
cd clerk-social-signin-issue
yarn install
yarn dev
```

2 Open `http://localhost:5173/` in your browser.

3 Click on the "Sign in with Google" button or any other social sign-in button.

4 You will be redirected to the social sign-in process and redirect back to `http://localhost:5173/#sso-callback` page.

5 After a few seconds, you will be redirected to the account portal login page and stop at here, no any other actions will be performed.

6 Back to localhost, there will be an error shows `The External Account was not found.`. (Sometimes this message will shows at account portal.)

7 This behavior will happen on all social sign-in buttons.

## The Expected Behavior

Should auto create a new user account if is a new user.
