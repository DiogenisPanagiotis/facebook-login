# React Facebook Login

> A React Component for Facebook Login

## Getting Started

- `yarn add react-facebook-login` or `npm install react-facebook-login`

## Development

```shell
git clone https://github.com/diogenispanagiotis/facebook-login.git && cd facebook-login
npm install react react-dom react-facebook-login --save --force
npm start
```
- navigate to [localhost:3000](http://localhost:3000)

## How to use

### Basic button with styling

```js
import React from 'react';
import ReactDOM from 'react-dom';
import FacebookLogin from 'react-facebook-login';

const responseFacebook = (response) => {
  console.log(response);
}

ReactDOM.render(
  <FacebookLogin
    appId="1088597931155576"
    autoLoad={true}
    fields="name,email,picture"
    onClick={componentClicked}
    callback={responseFacebook} />,
  document.getElementById('demo')
);
```