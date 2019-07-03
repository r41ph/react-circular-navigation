# react-circular-navigation

React circular navigation component.
Uses MaterialUI icons.

## Usage

```
$ npm i @r4lfl4b/react-circular-navigation
```

```jsx
import React from "react";
import ReactDOM from "react-dom";
import CircularNavigation from "@r4lfl4b/react-circular-navigation";
import HomeIcon from "@material-ui/icons/Home";
import AnnouncementIcon from "@material-ui/icons/Announcement";
import AssignmentIcon from "@material-ui/icons/Assignment";
import BuildIcon from "@material-ui/icons/Build";
import EmailIcon from "@material-ui/icons/Email";

function App() {
  return (
    <CircularNavigation overlay={true}>
      <CircularNavigation.item href={"#"} icon={<HomeIcon />}>
        Home
      </CircularNavigation.item>
      <CircularNavigation.item href={"#"} icon={<AnnouncementIcon />}>
        About
      </CircularNavigation.item>
      <CircularNavigation.item href={"#"} icon={<AssignmentIcon />}>
        Projects
      </CircularNavigation.item>
      <CircularNavigation.item href={"#"} icon={<BuildIcon />}>
        Labs
      </CircularNavigation.item>
      <CircularNavigation.item href={"#"} icon={<EmailIcon />}>
        Contact
      </CircularNavigation.item>
    </CircularNavigation>
  );
}

export default App;
```

## Development

To start the development server (with entry point `src/index.js`), run

```
$ npm start
```

## Storybook

To start the components explorer

```
$ npm run storybook
```

## Publish to npm

To transpile `src/lib` and create a build in the `dist` folder, run:

```
$ npm run build
```

To publish it to npm using:

```
$ npm publish
```

- Note that only README.md and the dist folders are published to npm.
