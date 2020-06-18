# Unicorn Zoo Web Application

> This web application, named _Unicorn Zoo_, was developed by me, [Owan Hunte](https://owanhunte.com), as part of my Code Fellows Instructor Technical Qualifying Interview.

## Local Development

**NOTE**: I prefer Yarn over NPM as my package manager of choice so this project uses Yarn.

1. Make sure you have [NodeJS](https://nodejs.org) (>= 12.0.0) and [Yarn](https://yarnpkg.com/en) (>= 1.17.3) installed.
2. Fork and clone this repository to your local environment.
3. Install the dependencies:

   ```
   cd path/to/app
   yarn
   ```

4. Create a file named **.env.local** in the root of the project and add the following local environment variable entries to the file:

   ```
   NEXT_PUBLIC_APP_BUILD_TARGET=local
   NEXT_PUBLIC_GOOGLE_KEY="<a-google-key>"
   ```

   The `NEXT_PUBLIC_APP_BUILD_TARGET` entry should be set to a value other than production, i.e. _local_ or _development_.

   To keep the authentication side of things agile I'm using the [pwa-auth](https://github.com/pwa-builder/pwa-auth) web component. Specifically the app allows anyone to log in to it using their Google account. The `NEXT_PUBLIC_GOOGLE_KEY` entry therefore needs to be set to a valid Google key. Details on creating a Google key can be found [here](https://github.com/pwa-builder/pwa-auth/blob/master/creating-google-key.md).

5. Start the Next.js server in development mode, specifiying the port to run the NodeJS process on. For example, if you want to run the application on port 3002 your command would be:

   ```
   PORT=3002 yarn dev
   ```

**NOTE**: You _MUST_ explicitly pass a port number to Next.js when starting the server in development mode, as shown in the above command. Alternatively you can make the PORT environment variable available to the application any other way you deem fit.

## Credits

- Favicon and site manifest logos by [Gordon Johnson](https://pixabay.com/users/GDJ-1086657/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=5184453) from [Pixabay](https://pixabay.com/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=5184453)
