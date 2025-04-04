# Introduction

This is the public repo for the AI generated anime art site that I've created as practice for front-end web development.

It uses the huggingface api key to use the model.

Initially, this was only a simple vanilla project but I decided to use Webpack due to the fact that I needed some secure ways to store the API key.
The project is a simple web app that allows users to generate anime art using a pre-trained model from Hugging Face. The app takes user input and generates four image based on the input using the model.

## Instructions

### Prerequisites
- Node.js
- npm
- Webpack
- dotenv-webpack
- html-webpack-plugin
- webpack-cli
- VSCode
- Live Server (optional, but recommended)
- Huggingface API key (required for the model to work)

### Make Your Own

1. First `git clone` this repo,
2. Then run `npm init -y`
3. Install these packages:
    - dotenv-webpack
    - html-webpack-plugin
    - webpack
    - webpack-cli
4. Run `npm run build` to build the project.
5. Run `npm run start` to start the project.
6. It is recommended to use "Live Server" extension for VSCode to view the project in your browser.

#### Webpack Stuff
- The `webpack.config.js` file is used to configure Webpack for the project.
- When the `package.json` file is created, you will need to add the following:
    - `build`: This script will build the project using Webpack.
    - `start`: This script will start the project using Webpack Dev Server.
    - The code will look like this:
```json
    "scripts": {
        "build": "webpack",
        "start": "webpack --watch"
    }
```

#### Change Model
- If you want to change the model, you can do so by changing the part in the `/src/script.js` file. Look for the line that contains a link with words "router" and "models".
- The current model in use is this:
https://router.huggingface.co/hf-inference/models/black-forest-labs/FLUX.1-dev



### Visiting the Site

You can directly visit the [site](https://huzbi-animeartai.vercel.app/) to check it out!

#### Please BE PATIENT with generating, sometimes the generation can fail due to unsucessful resource fetch.

For any issues, please create an issue on the GitHub repo. I will try to fix it as soon as possible.