# trc-campersguide
Static Vue site for displaying TRC Camper's Guide info in a user-friendly format.

## Visit Live Site
Site is deployed at [trianglehat.org](https://trianglehat)

## How to Contribute

Attention computer people! Want to contribute to this project? Yes you can. Here's a simple guide to get you started, even if you're new to GitHub. 

### Contributing Directly on GitHub

1. **Create a GitHub Account**: If you don't have one, sign up at [GitHub](https://github.com/).
2. **Fork the Repository**: Click the "Fork" button in the top right corner of our repository. This creates a copy in your account.
3. **Make Your Changes**: Navigate to the file you want to update, click edit, and make your changes. For an image, you can upload a new file directly.
4. **Commit Your Changes**: Add a meaningful commit message and commit directly to the `main` branch.
5. **Create a Pull Request**: Head over to the "Pull requests" tab in our repo, click "New pull request," and select your fork as the source. Fill in the details and submit!

### Using GitHub Desktop and NPM

1. **Install GitHub Desktop and NPM**: Download [GitHub Desktop](https://desktop.github.com/), and install [Node.js and npm](https://nodejs.org/en/).
2. **Clone the Repository**: Use GitHub Desktop to clone the forked repository to your machine.
3. **Install Dependencies**: In your project folder, run `npm install`.
4. **Run the Dev Environment**: Start the server with `npm run dev` and see your version in action in the browser.
5. **Make Local Changes**: Update the files as needed and view your changes in the browser.
6. **Commit and Push**: Use GitHub Desktop to commit and push your changes.
7. **Create a Pull Request**: Just like before, create a PR for your updates.

**Pro Tips**:
- Read the Commit history for more Update examples.
- Keep your fork updated with the latest changes from our repository.

Once you submit a PR, we'll review it and provide feedback. If everything looks good, we'll merge your changes into the project. Happy coding, and thanks for your input!

## Steps for Creating This Website from Scratch:

1. Open command prompt, cd to this directory. Run `npm create vue@latest` to use the Vue project scaffolding tool.
2. Use the default vue-project name. Choose yes for the Pinia option, no to all other options.
3. cd into vue-project. run `npm install` and then `npm run dev` to run the dev server.
4. Modify source code, view changes in dev server.
5. Push updates to GitHub.
6. Deploy on Azure as a static site.
7. Repeat steps 4 and 5 ad infinitum.

## Update example 1: Integrate Tailwind CSS

1. Follow Vue installation instructions on [Tailwind Docs](https://tailwindcss.com/docs/guides/vite#vue).
2. Create tailwind.css style sheet, import and add tailwind directives.
3. Update main.js, import tailwind style sheet.
4. Run `npm run dev` to interact with site in dev server. Update HelloWorld.vue component, add Tailwind CSS component classes to test and demonstrate its use.
5. Pushing this updated code will automatically update the deployed site, according to the Azure Static Web Apps GitHub workflow file. It takes about 2 minutes to see the updates go live. You can check on the status of the deployment from GitHub Actions.

