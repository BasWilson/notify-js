### Notify-JS
A lightweight and easy to use Notification class to use on your next website.  
Sweet **vanilla** JS 🍦

<img src="https://raw.githubusercontent.com/BasWilson/notify-js/master/examples/preview.png" width="auto" height="300" />

#### Setup
Simply download and add the notify-js.js file to you html file. 
`<script src="notify-js.js"></script>`

#### Example usage
```js
// User has logged in
function onLogin (username) {
    // Create a new notification
    new NotifyJS(
        {
            duration: 3, // Display for 3 seconds
            message: `Welcome back ${username}!` // Message
        },
        {
            color: '#42f477' // Set the box color
            textColor: 'black' // Set the text color
        }
    )
}
```
See the examples directory for more examples.

#### Options

The NotifyJS class takes two parameters:

**settings**

| Variable       | Description   | Type  | Example  |
| :-------------|:------------- | :-----| :-----|
| duration      | Time in ms that the notification will show for. | int | `3000` |
| message       | Message you want to show to the user.| string | `"Hello"` |
| timer         | Show countdown | boolean | `true` |

**style**

| Variable       | Description   | Type  | Example |
| :-------------|:------------- | :-----| :-----|
| backgroundColor| Color of notifcation | string | `"rgb(255,0,0)"`|
| color  | Text color | string | `"white"`|
| fontFamily  | Sets the font | string | `"Verdana"` |
| customCSSBox  | Change CSS properties of the notification box | string | `"border-radius: 5px;"` |
