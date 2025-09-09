# V3
<img width="1918" height="902" alt="image" src="https://github.com/user-attachments/assets/a373bc8a-a631-4dfe-ae4c-3832abd08684" />

✅ Implemented Features:

1. Settings Modal
 - Complete UI-based configuration for API endpoint, API key, model name, system prompt, temperature, and max tokens
 - No more JavaScript editing required Settings persist in localStorage
2. Stop Generation Button
 - Appears during streaming responses
 - Uses AbortController to properly cancel API requests
3. Export Conversations
 - Export as JSON, Markdown, or Plain Text
 - Option to export current chat or all chats
4. Code Syntax Highlighting
 - Integrated Prism.js with support for JavaScript, Python, JSON, Bash, SQL, and YAML
 - Automatic language detection from markdown code blocks
5. Copy Code Button
 - Added to every code block
 - Shows language type for each code block
6. Collapsible Sidebar
 - Toggle button to hide/show sidebar
7. Additional Themes
 - Matrix - Green on black with subtle scan lines effect
 - Neon - Cyberpunk-inspired magenta and cyan
 - Commodore 64 - Retro computing with classic C64 colors and monospace font
 - Plus the original themes (Light, Dark, Night Blue, Sepia)
8. Debug Console
 - Shows API requests/responses
 - Timestamps and color-coded entries
 - Toggleable panel at bottom right
 - Helps troubleshoot API issues
9. Smaller Stuff Implemented:
 - Timestamps on all messages
 - Character count in input field
 - Fullscreen mode toggle button
 - Delete individual chats with confirmation
 - Auto-scroll toggle (appears when scrolled up)
 - Keyboard shortcuts:
 -- Ctrl/Cmd + Enter - Send message
 -- Ctrl/Cmd + N - New chat
 -- Ctrl/Cmd + / - Toggle sidebar
 -- Ctrl/Cmd + S - Open settings
 - Model info display below input
 - Markdown table support

V1 and V2 still here if you would rather poke at those.


# LocalLLMChat V2!
![LocalLLMv2.png](https://github.com/dmeldrum6/LocalLLMChat/blob/main/LocalLLMv2.png?raw=true)

Since people are actually using this I have added a v2 - it features updated UI / Themes / Local Storage. I left the original as they're just single pages.


# LocalLLMChat
Single HTML Page access to an OpenAI API compatible Local LLM
![local_chat](https://github.com/dmeldrum6/LocalLLMChat/assets/38048135/9b8d2ca2-afe7-4fbf-9e30-0f65ca7665d1)

I have enjoyed running local LLMs using LM Studio, but wanted a simple way to be able to access them running on one computer at home from other machines without having to put up some kind of server framework.

This is a single webpage that uses JavaScript for the interaction with the OpenAI compatible API. Just edit the file and change the IP address from "Localhost" to whatever makes sense for you.

It implements streaming replies from the API so you don't need to wait for the entire answer to be rendered. As it is meant to be run serverless it does not have a lot of native features.

Generate - Passes prompt to the API endpoint and begins displaying response. <br/>
Stop - Cancels request and clears context <br/>
Clear Context - clears context and starts a new conversation. <br/>
