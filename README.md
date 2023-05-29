# 🥭 Project Mango Thesis Project

<img src="public/assets/logo2.png" alt="Logo" width="40%" height="40%">

A mango grading classification and mango product suggestion app built with TensorflowJS and NextJS.

In Partial Fulfillment of the Requirements for the Degree Bachelor of Science in Computer Science

April 2023

## Table of Contents

<details>
  <summary>Table of Contents</summary>

1. [About this project](#about-this-project)
2. [Contributors](#contributors)
3. [Getting Started](#getting-started)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Frequently asked questions](#frequently-asked-questions)
7. [Known Issues](#known-issues)
8. [Acknowledgements](#acknowledgments)

</details>

## About this Project

### :information_source: General

![Screenshot of homepage](public/screenshots/homepage.png "Screenshot of Homepage")

This project was developed as a requirement for the Thesis subject of the developers. The project is a Mango Classification App, a web-based application that aids consumers, sellers and exporters (especially in Guimaras) to classify mangoes and recommend suitable products based on its classification. The system allows the user to scan and upload mango images using a mobile device or PC. A Convolutional Neural Network (CNN) algorithm was used in the mango classification process.

For the front-end development of the system, ReactJS and Tailwind, while for the back-end, NextJS and TensorflowJS were utilized and the application was deployed using Vercel. Classification history is stored locally on client devices using localStorage API.

### :wrench: Project Architecture

#### :atom_symbol: Front-End

1. <img src="https://simpleicons.org//icons/react.svg" alt="drawing" width="16px"/> React
2. <img src="https://simpleicons.org//icons/tailwindcss.svg" alt="drawing" width="16px"/> Tailwind

#### :card_file_box: Back-End

1. <img src="https://simpleicons.org/icons/nextdotjs.svg" alt="drawing" width="16px"/> NextJS
2. <img src="https://simpleicons.org/icons/tensorflow.svg" alt="drawing" width="16px"/> TensorFlowJS
3. <img src="https://simpleicons.org/icons/vercel.svg" alt="drawing" width="16px"/> Vercel (Deployment)

## Contributors

### :family: Group Members

- Julia S. Carabaño
- Theodore Walter T. Galve
- Jessa Mae F. Nopueto
- Jonah James A. Pormento

Course, Year and Section: BSCS 4A

## Getting Started

### :computer: Prerequisites

- Install [NodeJS](https://nodejs.org/en/) v.16 LTS or higher.
- Clone this repository.
- Make sure you are in the 'src' folder
- This project uses **pnpm** as a package manager.
  To install it on your system, type:

  ```bash
  npm install -g pnpm
  ```

### Installation

- Install required dependencies:

  ```bash
  pnpm install
  ```

- Run the development server:

  ```bash
  pnpm dev
  ```

  or

  ```bash
  npm run dev
  ```

- If you like to build for production:

  ```bash
  pnpm build
  ```

  To start the production server:

  ```bash
  pnpm start
  ```

## Usage

This section explains the step-by-step procedure on how to classify mango images.

- Users can open the web app by typing <https://projectmango.vercel.app> in the address bar of their preferred web browser.

  For those that are running the development version of the app, they can access it locally by typing <http://localhost:3000>.

  <img src="public/screenshots/usage/Picture1.png" height="70%" width="70%">

- Upon opening the link, the user can click the 'Get Started' button to begin.

  <img src="public/screenshots/usage/Picture2.png" height="70%" width="70%">

- The user uploads mango images by clicking the 'Upload File' button. Camera option for desktop and laptops is not supported.

  <img src="public/screenshots/usage/Picture3.png" height="70%" width="70%">

- The user selects an image from their local device.

  <img src="public/screenshots/usage/Picture4.png" height="70%" width="70%">

- Upon uploading/capturing mango image, users can classify and generate results by clicking the 'classify' button.

  <img src="public/screenshots/usage/Picture5.png" height="70%" width="70%">

- After scanning the mango image, the system will display the classification results. Users have option to save them by clicking 'Save Results'.

  <img src="public/screenshots/usage/Picture6.png" height="70%" width="70%">

- The system will also display the product recommendations based on the classification results.

  <img src="public/screenshots/usage/Picture7.png" height="70%" width="70%">

## Frequently Asked Questions

### 1. Can I upload multiple images at the same time?

  No, only one image can be uploaded at a time.

### 2. Does this application collect personal data?

  No, the system will not gather any personal data from the user.

### 3. Can the Web application scan the image in real-time?

  The system does not support real-time image detection. Images must be uploaded manually.

### 4. Where is the data stored?

  The data is stored in the local browser storage of the device.

### 5. Can I take photos from different angles?

  Yes, but because the neural network model was trained in a controlled environment, the system might produce inaccurate results.

### 6. Is the system restricted to ripe mangoes only?

  No. Any kind of mangoes, regardless of its type, appearance, size, and shape can be classified.

## Known Issues

### 1. Issues accessing the app on Samsung Devices

  <img src="public/screenshots/issue1.jpg" height="50%" width="50%">
  
  On some Samsung devices, browsers may flag the app as unsafe. This is due to a false positive detection by Google SafeBrowsing. While this mistake has been reported, rest assured that the app is safe and no data collection is involved.

### 2. Inaccurate Prediction Results

  <img src="public/screenshots/inaccurate_results.png" height="70%" width="70%">

  There is a minor problem in classifying the mango images since there are some issues encountered in the model training process. Rest assured that this is an issue that pertains to the development of the app, so expect bugs and inaccuracies as you use it.

### 3. Classification takes a while on the first attempt

  <img src="public/screenshots/loading.png" height="50%" width="50%">

  The model takes a while to load depending on your network since it needs to be downloaded on the device. However, after the first attempt, succeeding classifications will be fast and smooth.

## Acknowledgments

Our deepest appreciation to:

### Thesis Advisers

Dr. Frank Elijorde and Ms. Nerilou Dela Cruz

### Experts from BPI-GNCRDPSC

- Juvy G. Narte
- Alex A. Tuyo
- Genoveva G. Macahilo
- Ruth F. Jardeleza
- Erlyn N. Billones
- Samuel P. Pielago
- Rhod S. Orquia
- Yondre J. Yonder

### Apps and Services

- [Font Awesome](https://fontawesome.com)
- [React Icons](https://react-icons.github.io/react-icons/search)

### License

MIT
