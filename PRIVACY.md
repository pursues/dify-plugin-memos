## Privacy Policy for MemOS Plugin

The purpose of this plugin is to serve as a client for a user-provided MemOS instance. MemOS is an open-source project that supports self-hosting.

**Data Collection:**

To function, this plugin requires the following credentials provided by the user during setup in Dify, corresponding to *their* MemOS instance (self-hosted or otherwise):
*   `MemOS_url`: The URL of the user's MemOS instance.
*   `MemOS_api_key`: The API key for authenticating with the user's MemOS instance.

When using the plugin's tools, the following data might be processed and sent to the specified MemOS instance:
*   `user_id`
    Description: The unique identifier for the end-user within the MemOS system.
    Required for: Both the add and search tools.
*   `query`
    Description: The content or question the user wants to inquire about.
    Required for: The search tool.
*   `messages`
    Description: The conversation content that the user wants to memorize. MemOS will analyze this input to extract mentioned events and personal preferences, form them into memory content, and store it in the MemOS memory management system.
    Required for: The add tool.

**Data Usage:**

*   The collected credentials (`MemOS_url`, `MemOS_api_key`) are used solely to establish a connection and authenticate with the user's designated MemOS instance.
*   This plugin itself does not persistently store any user data or credentials beyond the necessary runtime context for executing the requested tool function. Data is passed through to the MemOS API.

**Third-Party Services / Self-Hosting:**

*   This plugin relies entirely on the user-provided MemOS instance. All data processed by the tools is sent to this instance.
*   Since [MemOS](https://github.com/MemTensor/MemOS) is open-source , users typically deploy and manage their own instances.
*   Users are responsible for the privacy and security practices of their own MemOS instance. They should review the MemOS documentation and their specific deployment configuration to understand how data is handled.

**Contact:**

For questions regarding this plugin's privacy practices (specifically how it interacts with MemOS), please contact the author: [MemTensor](https://github.com/MemTensor). For questions about MemOS itself, please refer to the MemOS project resources.