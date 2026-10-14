# Video player

A React page called VIDEO HUB. The routes are `/`, `/videos`, `/upload`, `/login`, and `/signup`. Login, signup, and upload are forms with no submit handler. The fields are required, and a filled-in submit reloads the page. The footer email box has no form around it, so the send button does nothing.

A round button at the top left opens a drawer. The links are Home, Videos, Free Videos, and Upload Video, with Log In and Sign Up at the bottom. Free Videos goes to `/videos?category=free`. The videos page never reads that query, so it shows the same list. The button at the top right switches light and dark.

Home is a full-screen carousel that advances every second, loops, and hides the arrows, thumbs, and status. The slides read Watch The Future, Future is Gaming, Gaming on Console, and Night life is cool. Under that, a Services block shows one image and a placeholder paragraph.

Videos plays one of seven mp4 files kept in `src/components/Videos.jsx`. Lecture 1 through Lecture 7 swap the `src` on the player. The download control is turned off. The heading stays Sample Video 1, and the description stays the sample sentence, whichever lecture is selected.

Upload is a file input and an Upload button. Login asks for an email and a password. Forget Password goes to `/forgetpassword`, and that path has no page. Sign Up asks for a name, an email, and a password, and shows an empty avatar. The two pages link to each other.

The footer is a subscribe line, the words VIDEO HUB and "All rights received", and buttons labeled Youtube, Instagram, and Github. Those buttons open the public homepages of those sites. The subscribe button does not send the email.

## Run

From this folder:

```bash
npm install
npm start
```

Open [http://localhost:3000](http://localhost:3000).

`npm test` starts the test watcher. `npm run build` writes the production build. `npm run eject` copies the build config into the project, and that copy cannot be undone.

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app). The references from that README:

- [Running tests](https://facebook.github.io/create-react-app/docs/running-tests)
- [Deployment](https://facebook.github.io/create-react-app/docs/deployment)
- [Getting started](https://facebook.github.io/create-react-app/docs/getting-started)
- [React](https://reactjs.org/)
- [Code splitting](https://facebook.github.io/create-react-app/docs/code-splitting)
- [Analyzing the bundle size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)
- [Making a progressive web app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)
- [Advanced configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)
- [npm run build fails to minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
