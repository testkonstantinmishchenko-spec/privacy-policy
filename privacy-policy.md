# Privacy Policy for SupportUp Extension

## Data we collect

1. **Authentication tokens** – when you interact with `chat-api.moneyman.ru`, the extension reads the `Authorization` and `ApiKey` headers from outgoing requests. These tokens are temporarily stored in `chrome.storage.local` **only** to authenticate subsequent API calls (e.g., fetching `visitor_id` or CRM data). They never leave your device.

2. **Extension preferences** – your on/off choices for each feature (e.g., "Fix messages", "Collapse system messages") are stored in `chrome.storage.sync`. This allows your settings to be available across devices if you are signed into Chrome.

3. **UI state** – some temporary selections (like radio button choices in the chat interface) are saved in `localStorage` to persist across page reloads. This data is not synced and is purely for convenience.

4. **Email and visitor identifiers** – when you view a chat, the extension may extract the visitor's email from the page and send it (via the background script) to the `search_visitors` API to retrieve `visitor_id` values. These IDs are displayed in the chat header and are **not stored** permanently. The email is only used for that single lookup.

## How we use data

- Tokens are used **only** to make authenticated requests to `chat-api.moneyman.ru` and `admin.moneyman.ru` as part of the extension's core features (showing visitor IDs, opening CRM links).
- Preferences are used to enable/disable specific modules according to your choice.
- No data is used for analytics, profiling, marketing, or any purpose other than providing the described functionality.

## Data storage and retention

- **`chrome.storage.local`** (tokens): stored locally, cleared when you uninstall the extension.
- **`chrome.storage.sync`** (preferences): stored in your Google account (if sync is enabled) and can be managed via Chrome's settings.
- **`localStorage`** (UI state): stored locally; you can clear it via browser developer tools or by uninstalling the extension.

## Data sharing

We **do not** sell, rent, or share any user data with third parties. All data is processed locally or within the `moneyman.ru` domain in accordance with your authentication.

## User rights

You may delete all extension data at any time:
- Uninstall the extension – all data (tokens, preferences, UI state) will be automatically removed.
- Alternatively, you can manually clear `chrome.storage.local`, `chrome.storage.sync`, and `localStorage` via Chrome's developer tools (F12 → Application tab).

## Updates to this policy

If the extension's functionality changes, we will update this policy and notify users via the Chrome Web Store update description.

## Contact

For any privacy-related questions, please contact us at: test.konstantin.mishchenko@gmail.com
