
# Salesforce Connector for Claude Desktop

[](https://www.google.com/search?q=https://securityscorecards.dev/viewer/%3Furi%3Dgithub.com/KiranWelisa/claude-desktop-extension-salesforce)

This is a Claude Desktop Extension that integrates with Salesforce, enabling natural language interactions with your Salesforce data and metadata. This extension allows Claude to query, modify, and manage your Salesforce objects and records using everyday language.

## Features

  * **Object and Field Management**: Create and modify custom objects and fields using natural language.
  * **Smart Object Search**: Find Salesforce objects using partial name matches.
  * **Detailed Schema Information**: Get comprehensive field and relationship details for any object.
  * **Flexible Data Queries**: Query records with relationship support and complex filters.
  * **Data Manipulation**: Insert, update, delete, and upsert records with ease.
  * **Cross-Object Search**: Search across multiple objects using SOSL.
  * **Apex Code Management**: Read, create, and update Apex classes and triggers.
  * **Intuitive Error Handling**: Clear feedback with Salesforce-specific error details.

## Installation and Setup

Installing the Salesforce Connector is a simple, one-click process.

### 1\. Download the Extension

Download the latest release file, which will be named `salesforce-connector-extension-x.x.x.dxt`, from the [releases page of this repository](https://www.google.com/search?q=https://github.com/KiranWelisa/claude-desktop-extension-salesforce/releases).

### 2\. Install the Extension

Simply **double-click** the downloaded `.dxt` file. Claude Desktop will automatically open and handle the installation.

Alternatively, you can drag and drop the `.dxt` file into the **Settings \> Extensions** page in Claude Desktop.

### 3\. Configure Your Credentials

After installation, you must configure your Salesforce credentials:

1.  Go to **Settings \> Extensions** in Claude Desktop.
2.  Find the "Salesforce Connector" extension and click the **settings icon (⚙️)**.
3.  Fill in the required fields based on your chosen authentication method.

#### Authentication Method: User/Password

  * **Connection Type**: `User_Password`
  * **Salesforce Instance URL**:
      * For production/developer orgs, use: `https://login.salesforce.com`
      * For sandbox orgs, use: `https://test.salesforce.com`
  * **Salesforce Username**: Your Salesforce username.
  * **Salesforce Password**: Your Salesforce password.
  * **Salesforce Security Token**: Your security token (deze kunt u resetten via uw Salesforce-instellingen).

#### Authentication Method: OAuth 2.0 Client Credentials

  * **Connection Type**: `OAuth_2.0_Client_Credentials`
  * **Salesforce Client ID**: The Client ID from your Salesforce Connected App.
  * **Salesforce Client Secret**: The Client Secret from your Salesforce Connected App.
  * **Salesforce Instance URL**: Your organization's specific "My Domain" URL (e.g., `https://welisa.my.salesforce.com`).

Once configured, the extension is ready to use\!

## Tools

This extension provides a comprehensive set of tools to interact with Salesforce:

  * **salesforce\_search\_objects**: Search for standard and custom objects.
  * **salesforce\_describe\_object**: Get detailed schema information for any object.
  * **salesforce\_query\_records**: Query records with support for relationship queries.
  * **salesforce\_aggregate\_query**: Execute aggregate queries with `GROUP BY`.
  * **salesforce\_dml\_records**: Perform data operations (insert, update, delete, upsert).
  * **salesforce\_manage\_object**: Create and modify custom objects.
  * **salesforce\_manage\_field**: Manage object fields and create relationships.
  * **salesforce\_manage\_field\_permissions**: Manage Field Level Security for profiles.
  * **salesforce\_search\_all**: Search for text across multiple objects using SOSL.
  * **salesforce\_read\_apex**: Read Apex classes.
  * **salesforce\_write\_apex**: Create and update Apex classes.
  * **salesforce\_read\_apex\_trigger**: Read Apex triggers.
  * **salesforce\_write\_apex\_trigger**: Create and update Apex triggers.
  * **salesforce\_execute\_anonymous**: Execute anonymous Apex code.
  * **salesforce\_manage\_debug\_logs**: Manage debug logs for users.

## Development

### Building from source

```bash
# Clone the repository
git clone https://github.com/KiranWelisa/claude-desktop-extension-salesforce.git

# Navigate to directory
cd claude-desktop-extension-salesforce

# Install dependencies
npm install

# Build the project
npm run build
```

### Packaging the Extension

To create the `.dxt` file for distribution:

```bash
# Install the DXT command-line tool
npm install -g @anthropic-ai/dxt

# Package the extension
dxt pack .
```

## Contributing

Contributions are welcome\! Feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](https://www.google.com/search?q=LICENSE) file for details.
