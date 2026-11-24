# uBlock Origin Filter list for Reddit

Restores the logged-out Reddit experience for privacy-conscious users. Tested in Firefox desktop and mobile.

## Features

- Access to age-restricted non-NSFW posts
- Automatically reveals blurred media
- NSFW search results
- Fixes embedded players (usability + frame resizing after unblur)
- Restores the burger menu on desktop (quick access to recently visited subreddits)
- Removes the big login banner on desktop
- Removes "Log in / Sign up" (desktop) and "Open App" (mobile) buttons
- Removes unclosable popups and overlays on mobile

Closable popups and the cookie consent popup are intentionally kept functional.

## Installation

This list uses trusted filter rules, so you need to allow it before importing.

1. Open the uBlock Origin dashboard → **Settings** tab and enable **I am an advanced user**.
2. Expand the *advanced settings*, find the entry called `trustedListPrefixes`, and add the URL of this filter list **after the existing value**. The entries are separated by a space. It should look like this:
   ```
   trustedListPrefixes ublock- https://raw.githubusercontent.com/stolen-retile9/ubo-filter-reddit/refs/heads/main/filterlist.txt
   ```
3. Go to the **Filter lists** tab → **Import…**, paste the URL below, and click **Apply changes**:
   ```
   https://raw.githubusercontent.com/stolen-retile9/ubo-filter-reddit/refs/heads/main/filterlist.txt
   ```
4. If you change the `trustedListPrefixes` setting *after* importing, reload the list afterwards using the **watch icon** — the trusted filter rules won't take effect until you do.

## Note

Reddit is gradually restricting logged-out access. An alternative is creating an account via a VPN (e.g., Switzerland, where no ID verification is forced) to keep full access.

## Credits

Based on [andradeatdev's Reddit-NSFW-Unblur](https://github.com/andradeatdev/Reddit-NSFW-Unblur/blob/main/filters/ublock.txt).

## License

MIT
