# CLI for Code Review AI

## Overview

The `code-review-ai-cli` is a command-line interface tool designed for code review using AI. It leverages the power of Google's Gemini AI model to analyze and provide suggestions on code diffs from Git repositories. This CLI tool helps developers improve their code quality efficiently.

## Features

- **Review Code Diffs**: Analyze and review code changes with AI suggestions.
- **Add API Key**: Configure your Gemini API key for authentication.
- **Easy Setup**: Simple commands to manage your API key and perform code reviews.

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/code-review-ai-cli.git
   cd code-review-ai-cli

2. **Install Dependencies**
   Ensure you have Node.js installed. Then, install the required packages:

   ```bash
   npm install

3. **Build**
   Compile TypeScript code to JavaScript:

   ```bash
   npm run build

## Usage
### Adding Your API Key
To use the Gemini AI model, you need to set up your API key. Follow these steps to add your API key:

1. **Obtain a Gemini API Key**

   - Go to the [Google Cloud Console](https://console.cloud.google.com/).
   - Navigate to the **APIs & Services** section.
   - Select **Credentials** from the menu.
   - Click on **Create Credentials** and choose **API Key**.
   - Copy the generated API key.

2. **Add the API Key to Your Project**

   Use the `add-key` command to save the API key:

   ```bash
   npm run start add-key "your-gemini-api-key"

  This command saves the API key in a .env file. Make sure to replace "your-gemini-api-key" with your actual API key.

### Reviewing Code Diffs

To review code diffs using the AI model, use the review command:

    npm run start review

This command retrieves the code diff from the current Git repository and sends it to the Gemini AI model for analysis. Ensure that your API key is set before running this command.

### Commands

- `add-key <apiKey>`: Add your Gemini API key. Replace <apiKey> with your actual API key.
- `review`: Review the code diff in the current Git repository.

## Configuration
The .env file is used to store the API key. The file will be automatically created or updated when you run the add-key command. Ensure this file is included in your .gitignore to keep your API key secure.

## Troubleshooting
- **Error: API key is not set**: Ensure that you have added the API key using the add-key command and that the .env file is in the project root.
- **Command not found**: Ensure you have built the project using npm run build and that you're running the command from the correct directory.

## Contributing
Contributions are welcome! Please submit a pull request or open an issue if you find bugs or have feature requests.

## License
This project is licensed under the MIT License.

## Support

If you find this project useful and would like to support its development, consider making a donation via Pix. Your support helps cover development costs and keep the project active.

Pix: 98992073959

Thank you for your support! 👍

