# Node.js Gmail Auto-Reply Application

![Node.js Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/1280px-Node.js_logo.svg.png)

This Node.js application allows you to automatically reply to emails in your Gmail account with a specific reply message and categorize those emails under a new label. The application uses the Gmail API to access your Gmail account and send automated responses.

## Prerequisites

Before running the application, ensure you have the following prerequisites installed:

1. Node.js: Make sure you have Node.js installed on your system. You can download it from the official Node.js website: https://nodejs.org/

2. Gmail API Access: Obtain API access credentials from the Google Developer Console to authenticate your application. Instructions on how to set up the Gmail API can be found in the [Google Developers Guide](https://developers.google.com/gmail/api/quickstart).

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/your-nodejs-gmail-auto-reply.git
cd your-nodejs-gmail-auto-reply
```

2. Install dependencies:

```bash
npm install
```

3. Set up your Gmail API credentials:

   - Follow the instructions in the Google Developers Guide (link above) to create a project and enable the Gmail API.
   - Download the `credentials.json` file and save it in the root directory of the application.

## Usage

Run the application using the following command:

```bash
node index.js
```

When you run the application for the first time, it will prompt you to authorize access to your Gmail account. Follow the provided URL, grant access, and copy the authorization code back into the terminal.

The application will start listening for new emails in your Gmail inbox. When it finds a new email, it will automatically reply to the sender with a default auto-reply message and add the email to a new label named "Auto-Replied."

You can modify the auto-reply message and label name directly in the `index.js` file if needed:

```javascript
const replyMessage = 'Your auto-reply message goes here.';
const labelName = 'Auto-Replied';
```

## Limitations and Considerations

- This application may not work as expected if you have complex Gmail filters or forwarding rules already set up. Ensure to test it in a controlled environment to avoid unexpected behaviors.

- Be cautious with the auto-reply message content to avoid sending unwanted or spammy replies.

- Make sure to handle exceptions and errors properly, especially when dealing with third-party APIs like the Gmail API.

- The Gmail API usage may be subject to rate limits and restrictions. Refer to the Gmail API documentation for more information.

## Contributing

Contributions to the project are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

This Node.js Gmail Auto-Reply Application is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).

## Disclaimer

This application is provided as-is and without warranty. Use it at your own risk. The author and contributors are not responsible for any damages or misuse of this application.

Happy auto-replying! 📧🚀
