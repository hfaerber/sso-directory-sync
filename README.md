# Node.js Application Using WorkOS to configure SSO and Directory Sync with Okta 

An example application demonstrating how to use the [WorkOS Node.js SDK](https://github.com/workos/workos-node) to authenticate users via SSO.

This application uses WorkOS's [node-sso example application](https://github.com/workos/node-example-applications/tree/main/node-sso-example) as a starter.  WorkOS is used to configure SSO and Directory Sync connections with Okta. 

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

4. Contact [https://www.linkedin.com/in/heather-faerber/](Heather) for required environment variables.

5. Store the environment variables like so:

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

7. Navigate to 'http://localhost:8000/' in your browser.

8. Login with Google, Microsoft or Okta


