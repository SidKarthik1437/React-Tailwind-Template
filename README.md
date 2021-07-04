# CRA-template for React-Tailwind by SidKarthik

This ia a template with a robust file structure, tailwind, routing system, lazy-loading and skeleton-loading Pre-configured.
You can jump right into development!

## Setup
**Run the following command in the terminal to use template**
```
npx create-react-app <app-name> --template sidkarthik
npm run setup
```

## Using the Router
### `Step 1`
```
Create a New <filename>.js in Pages folder
```

### `Step 2`
-> Create a new variable in constants/routes.js and specify route in the format:
```
export const <routename> = '<path>'
```

### `Step 3`
-> Import the page in App.js using the following format in-order to use lazy-loading :
```
const <pagename> = lazy(() => import(<path>));
```

### `Step 4`
-> Add Route tag in the provided region and set the following props:
```
path={ROUTES.<routename>}
component={<pagename>}
```
### `Note`

-> React works on basis of rendering in layers hence the stack should be in descending order i.e., 
the bottom-most layer is rendered first

## Learn more 
[create-react-app](https://github.com/facebook/create-react-app)
[Tailwind](https://tailwindcss.com/)
[Lazy-loading](https://blog.bitsrc.io/lazy-loading-react-components-with-react-lazy-and-suspense-f05c4cfde10c)
[React-loading-skeleton](https://www.npmjs.com/package/react-loading-skeleton)

