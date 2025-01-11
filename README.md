# Okta SSO and Directory Sync with WorkOs 

This node.js application uses WorkOS's [node-sso example application](https://github.com/workos/node-example-applications/tree/main/node-sso-example) as a starter.  WorkOS is used to configure SSO and Directory Sync connections with Okta. 

## Video Demonstration

This [video walkthrough](https://youtu.be/w8OqwRxk5IM) (no audio) shows successful logins using the Google OAuth option and the Enterprise SAML option with Okta.  It also demonstrates a successful Directory Sync connection by displaying a job title change originating in Okta for user Noah Davis. 

## To Use the Deployed Application

1. Navigate to the [deployed app](https://sso-directory-sync.onrender.com/) .

2. Login using the Google OAuth option. _Note that only users configured in Heather's Okta application will be able to successfully login in through the Enterprise SAML option._ 

3. Use the Directory button to view user details from the Okta Directory Sync.


## To Run Locally

### Prerequisites

- Node.js version 10+
- API key, client id and session secret environment variables are required to run this session locally. Please contact Heather for more information.

### Setup

1. Clone this repo

    ```bash
    # HTTPS
    git clone https://github.com/hfaerber/sso-directory-sync.git
    ```

    or

    ```bash
    # SSH
    git clone git@github.com:hfaerber/sso-directory-sync.git
    ```

2. Install the dependencies.
    ```bash
    npm install
    ```

3. Create .env file at the project root
    ```bash
    touch .env
    ```

4. Contact [Heather](https://www.linkedin.com/in/heather-faerber/) for required environment variables.

5. Store the environment variables in the .env file:

    ```bash
    WORKOS_API_KEY=sk_xxxxxxxxxxxxx
    WORKOS_CLIENT_ID=project_xxxxxxxxxxxx
    SESSION_SECRET=xxxxxxxxxxxx
    ```

### Run the app

6. Start the server
    ```bash
    npm start
    ```

7. Navigate to http://localhost:8000/ in your browser.

8. Login using the Google OAuth option. _Note that only users configured in Heather's Okta application will be able to successfully login in through the Enterprise SAML option._ 

9. Use the Directory button to view user details from the Okta Directory Sync.
