# 🚀 ATLAN SQL Editor

This is a ATLAN SQL Editor built using ReactJs and TailwindCSS.

![Homepage](src/assets/screenshots/screenshot-one.png)

## 👨‍💻 Demo

<a href="https://github.com/rishipurwar1/coding-space" target="blank">
<img src="https://img.shields.io/website?url=https://www.codingspace.codes&logo=github&style=flat-square" />
</a>

Try out the website : [ATLAN SQL Editor](https://atlan-react-sql-editor.netlify.app/)

## 👨‍🔧 Tech Stack

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)

## 👨‍💻 Features

- [x] User can get data of any of the below SQL queries either by using Text Editor or Sidebar Menu.
- [x] User can filter data directly by clicking the Table Headers title.
- [x] User can search for a particular data using the search bar.
- [x] User can navigate to different pages using pagination.
- [x] User can download the data in both CSV and JSON Format in just one click.
- [x] User can see query runtime in milliseconds(ms).

## ✍️ Predefined SQL Queries

- `select * from customers`
- `select * from categories`
- `select * from employee_territories`
- `select * from order_details`
- `select * from orders`
- `select * from products`
- `select * from regions`
- `select * from shippers`
- `select * from suppliers`
- `select * from territories`

## ⏱ Page Load Time

Load time of this website is between 0.4 s to 0.6s.

I tested the performance and load time of this website using these two tools Lighthouse Chrome DevTools and BrowserStack SpeedLab.

### [Lighthouse Chrome DevTools Report](https://developers.google.com/web/tools/lighthouse#devtools) (got a perfect 💯)

![lighthouse report](src/assets/screenshots/screenshot-two.png)

- **First Contentful Paint** marks the time at which the first text or image is painted
- **Time to interactive** is the amount of time it takes for the page to become fully interactive.
- **Speed Index** shows how quickly the contents of a page are visibly populated.
- **Total Blocking Time** is the sum of all time periods between FCP and Time to Interactive, when task length exceeded 50ms, expressed in milliseconds.
- **Largest Contentful Paint** marks the time at which the largest text or image is painted.
- **Cumulative Layout Shift** measures the movement of visible elements within the viewport.

### [BrowserStack Report](https://www.browserstack.com/speedlab)

![browserstack report](src/assets/screenshots/screenshot-three.png)

## 🪜 Steps I took to optimize the page load time

- Used `React.Lazy()` to lazy load the component and reduce the bundle size for faster load.
- Used `React.Memo()` to optimize the render performance of functional components.
- Used JIT and PurgeCSS to remove unused CSS.
- Used Lighthouse DevTools Extension to find the performance issues.
- Used vercel to leverage its Vercel Edge Network compression that results in the better performance.

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.
