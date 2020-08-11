# googlemaps-react

A Google Maps component that can be used by simply passing your API Key through props or by saving it to an .env file.

## Installation

Install using npm:

```sh
npm install --save googlemaps-react
```

Install using yarn:

```sh
yarn add googlemaps-react
```

## Usage

[React.js](http://facebook.github.io/react/) is a peer dependencies for googlemaps-react. This dependency is not installed along with googlemaps-react automatically, but your project needs to have it installed in order to make the googlemaps-react work. You can then use the googlemaps-react like in the example below.

```js
import React from "react";
import GoogleMapsReact from "googlemaps-react";

...

const App = () => {
return <GoogleMapsReact apiKey={[YOUR_GOOGLE_MAPS_API_KEY]} latLng={[41.093842, -85.139236]}/>
}

export default App;
```

[See this example working](http://codepen.io/simeg/pen/mEmQmP).

## API

| Name           | Type                       | Default                                | Description                                                                             |
| -------------- | -------------------------- | -------------------------------------- | --------------------------------------------------------------------------------------- |
| **apiKey**     | `String`                   | `process.env.REACT_APP_GOOGLE_MAP_API` | Pass the Api Key through props or default to REACT_APP_GOOGLE_MAP_API in you .env file. |
| **latLng**     | `Array`                    | `[41.093842, -85.139236]`              | Center coordinates of map and marker point                                              |
| **mapOptions** | `Object`                   | `{disableDefaultUI: true, zoom: 10}`   | Google Maps Api options.                                                                |
| **className**  | `string` or `string array` | `''`                                   | Extra class name for the map element                                                    |
