# Email Processor Project

## Overview
This project is a UiPath automation workflow designed to retrieve and process email data, specifically extracting the header (subject) and body of emails. It is built to streamline email handling tasks by logging and organizing key email information.

## Features
- Retrieves email headers (subjects) and bodies from a configured email account.
- Logs the extracted data for review and further processing.
- Supports iteration through multiple emails using a "For Each" loop.
- Saves email attachments (optional configuration).

## Prerequisites
- **UiPath Studio**: Ensure you have the latest version installed.
- **UiPath.Mail.Activities**: Install this package via the Manage Packages option.
- **Outlook Account**: A configured Outlook account is required for email access.
- **Permissions**: Ensure the account has appropriate access to read emails.

## Setup Instructions
1. **Clone the Repository**:
   - Clone this repository to your local machine using Git:
2. **Open in UiPath Studio**:
- Open the project folder in UiPath Studio.
3. **Configure Outlook Scope**:
- Add an "Outlook Application Scope" activity and connect it to your Outlook account.
4. **Adjust Variables**:
- Ensure the `currentMailMessage` variable is correctly scoped within the "For Each" loop.
5. **Run the Workflow**:
- Execute the workflow in debug mode to test email retrieval.

## Usage
- The workflow iterates through emails, logging the subject and body using "Log Message" activities.
- Attachments can be saved if the "Save Email Attachments" activity is configured with a valid folder path.
## Output
Below is a screenshot of the workflow output:

![Workflow Output](https://github.com/rewaaalaa7/EmailAutomation-RPA/blob/main/output.jpg)
## Contributing
Feel free to fork this repository and submit pull requests for improvements. Please ensure any changes are tested before submission.

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
