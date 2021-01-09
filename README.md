# An Introduction to Redux-Logic

<p>Redux is a popular predictable state container for JavaScript applications.<br /><br />
Redux-Thunk is a popular choice for Redux middleware that also allows you to support asynchronous (एसिंगक्रनस) behaviour.<br /><br />
Another popular Redux middleware is Redux-Saga.  I think that if they are not well managed, then sagas can create complicated-looking code compared to the Logic you create with redux-logic. This can impact development speed and code maintainability.</p>

## How to interact with the Redux store in a React app  
<ul>
<li>Connect individual react component to the redux store</li>
<li>Interact with the redux store</li>
<li>Retrieve information from the store</li>
</ul>  

### Connect individual react component to the redux store
First we must install the react-redux npm package if you don’t have it installed in your react app:  
`npm install react-redux`

Import a function called connect from this package: (Please check spelling it is <b>'connect'</b> not 'Connect' because it is a function and not a component.)  
`import { connect } from "react-redux";`

Once connect imported on your file then wrap your component with the connect function.The connect function can take two arguments. 


    import React, {Component} from "react";
    import { connect } from "react-redux";
	
	class MyClassComponent extends Component{
	... ... ...
	... ... ...
	}
	export default connect()(MyClassComponent);
### Interacting with the redux store  
<b>Redux flow</b>  
1. A react <b>component</b> dispatching an <b>action</b><br/>  
2. The dispatched-<b>action</b> gets to the <b>store</b>, which then passes it to the <b>reducer</b><br/>
3. depending on the type of dispatched-<b>action</b>, the reducer will update the <b>state</b> and pass the <b>new state</b> to the store.<br/>
4. the <b>store</b> will then pass the <b>new state</b> received from the <b>reducer</b> to the <b>component</b>.<br/>
 

### Interacting with the redux store  







https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#lists
## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
