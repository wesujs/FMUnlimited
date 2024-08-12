This README will guide users through setting up and using your FM-Unlimited application, providing them with clear instructions and resources.


Here's an updated version of the README file with adjustments reflecting that MongoDB setup and command-line actions won't be needed by the end users, since you'll be providing the database support and the application will be distributed as an `.exe` file.

```markdown
# FM-Unlimited

FM-Unlimited is a desktop application that allows you to scrobble tracks to your Last.fm account. The application features customizable scrobble settings and connects to a shared MongoDB database to store your API credentials and scrobble limits.

## Features

- **Scrobbling**: Easily scrobble your favorite tracks to Last.fm.
- **API Integration**: Save and reuse your Last.fm API credentials for seamless scrobbling.
- **Scrobble Limits**: Manage the number of scrobbles allowed in the free version.
- **Dangerous Scrobbles**: Enable faster scrobbling with reduced delays, with a warning about potential account risks.
- **Paywall Unlock**: Unlock the full version to remove scrobble limits.
- **User-Friendly GUI**: Simple and intuitive interface for all users.

## Requirements

- Windows 7 or later
- Python 3.x installed ([Download Python](https://www.python.org/downloads/)) if you plan to run the source code.
- No need to set up MongoDB or perform command-line actions. Just download and run the `.exe` file.

## Installation

### Download the Executable

1. **Download the Executable**:
   - [Download FM-Unlimited.exe](https://github.com/wesujs/FMUnlimited/releases) (Replace this with the actual link to your executable once available)

2. **Run the Executable**:
   - After downloading, simply run the `FM-Unlimited.exe` file to start the application.

### Option 2: Download via Zip (For Developers)

1. **Download the Zip File**:
   [Download FM-Unlimited](https://github.com/wesujs/FMUnlimited/archive/refs/heads/main.zip)

2. **Extract the Files**:
   Unzip the downloaded file to a directory on your computer.

3. **Run the Application**:
   Start the application by running the `fmspam.py` script in a Python environment:
   ```bash
   python fmspam.py
   ```

## Getting Your Last.fm API Key, API Secret, and Session Key

To use FM-Unlimited, you need to obtain your Last.fm API credentials. Follow these steps:

1. **Create a Last.fm API Account**:
   Visit the [Last.fm API Authentication Page](https://www.last.fm/api/authentication) and sign in with your Last.fm account.

2. **Create an API Application**:
   - Once signed in, create a new API application to get your API Key and API Secret.
   - You will need to provide some basic information about your application.

## Getting Your Last.fm Session Key Using the GUI

FM-Unlimited includes a handy GUI tool to help you quickly generate your Last.fm session key. Follow these steps:

1. **Run the Session Key Generator**:
   - Download and run the `getSeshKey.exe` file.
   - Enter your Last.fm API Key and API Secret in the provided fields.

2. **Authorize Your Token**:
   - Click "Get Session Key". This will generate a token and open a web browser prompting you to authorize it with Last.fm.
   - After authorizing, return to the application.

3. **Retrieve Your Session Key**:
   - Click the "I've authorized the token" button.
   - Your session key will be displayed in the window. Copy it and keep it safe for future use.

4. **Input Your Credentials**:
   - Once you have your API Key, API Secret, and Session Key, input them into FM-Unlimited's GUI and click "Submit" to validate and save them.

## Usage

1. **Run the Application**:
   Start the application by running the `FM-Unlimited.exe` file.

2. **Enter API Credentials**:
   - Input your Last.fm API Key, API Secret, and Session Key.
   - Click "Submit" to validate and save these credentials.
   - The credentials will be stored in a shared MongoDB database, so you won't need to re-enter them each time.

3. **Scrobble Tracks**:
   - Enter the Artist name, Song title, and the number of scrobbles you want to submit.
   - Click "Start Scrobbling" for standard scrobbling intervals.
   - Click "Dangerous Scrobbles" for faster scrobbling with a 10-second delay between submissions. Note the warning about potential account risks.

4. **Unlock Full Version**:
   - If you have a paywall unlock code, enter it in the "Paywall Code" field and click "Unlock Full Version."
   - This will remove the scrobble limits for your account.

5. **Contact Support**:
   - If you run out of scrobbles or need support, click the "Contact Support (Discord)" button to reach the developer.

## Troubleshooting

- **Invalid API Credentials**: If your credentials are not validated, ensure they are correctly copied from your Last.fm account.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.

## Contact

For support, contact me via Discord: `amgk` ([Discord Profile](https://discordapp.com/users/703112459313217556/)).
```
