# persona-pwa

A simple progressive web app for matching personas and conversing with AI assistants.

**Starting a chat session**

After selecting or creating an assistant you must first run the **Improve** or **Get video suggestions** action. These actions start the conversation and create a single chat thread shared by all personas. Once a thread exists you can freely exchange messages in the chat box. Attempting to chat before running either action will show a "No active chat session" warning.

The conversation and thread IDs remain the same no matter which persona you talk to. Both values are stored in `localStorage` so the chat can continue after a refresh. Switching personas only changes the persona ID that is passed with each message; the backend resolves the corresponding assistant automatically.
