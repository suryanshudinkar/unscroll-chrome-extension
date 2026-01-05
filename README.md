# unscroll-chrome-extension

Chrome extension for Instagram detox: Block addictive elements for better control.

## Features

- **Block Reels**: Hide Reels tab and block navigation to Reels
- **Block Explore**: Hide Explore page and redirect to home feed
- **Block Feed**: Prevent loading of main feed
- **Block Stalking**: Disable search and profile access
- **Settings UI**: Easy-to-use popup with toggles
- **Reset**: Reset settings to defaults

### Using the Extension

1. Navigate to [Instagram.com](https://www.instagram.com)
2. Click the Unscroll icon in your Chrome toolbar
3. Configure your blocking preferences
4. Settings are automatically saved and applied

### Blocking Options

- **Block Reels**: Hides the Reels tab in navigation and blocks navigation to Reels
- **Block Explore**: Hides the Explore tab and redirects Explore page to home
- **Block Feed**: Prevents the main feed from loading
- **Block Stalking**: Disables search functionality

### Browser Compatibility

- Chrome 88+ (Windows, macOS, Linux)
- Other Chromium-based browsers (Edge, Brave, etc.)

## Privacy
Unscroll does not collect, store, or transmit any personal or sensitive user data.
All preferences are stored locally on the user’s device using Chrome storage APIs.
The extension does not use analytics, tracking, or external servers.

## Support
For issues or feature requests, please open a GitHub issue.

## Limitations & Notes

1. **Instagram UI Changes**: Instagram frequently updates their UI. Selectors may need updates if Instagram changes their DOM structure. The extension uses multiple selector strategies to be more resilient.
2. **Content Script Timing**: Content scripts run at `document_start` to catch navigation early, but some elements may load after the initial injection. The extension uses MutationObserver to handle dynamically loaded content.
