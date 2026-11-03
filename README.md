# My board

A personal Kanban board in a single web page: accounts, projects with values, a project × stage matrix, weekly statistics, and confetti when a card reaches Done. It works on phones and desktops.

## Put it on GitHub Pages

1. Create a new repository on GitHub. It can be public or private (private Pages needs a paid GitHub plan).
2. Upload `index.html`, `README.md` and `.nojekyll` to the root of the repository. (`.nojekyll` is hidden on some computers; it's optional.)
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose the `main` branch and the `/ (root)` folder, then **Save**.
5. After a minute or two, the page is live at `https://<your-username>.github.io/<repository-name>/`.

## Accounts

- The first time you open the page, you'll see **Create an account**: your name, a username or email, and a password of at least 8 characters.
- After that, the page opens on **Sign in**. "Don't have an account? Create one" adds another account; each account has its own separate board.
- You stay signed in until you close the tab, choose **Account → Sign out**, or leave the board idle for 15 minutes.
- **Account → Change password** and **Account → Delete this account** are in the menu.

## How your data is stored

The board has no server. Everything runs in your browser:

- Accounts, cards, projects and statistics are saved in that browser on that device only. Nothing is sent to GitHub or anywhere else.
- An account made on your laptop doesn't exist on your phone. To move a board between devices, use **Account → Download a backup** on one, then create an account and use **Account → Restore from a backup** on the other.
- Clearing your browser's site data, or using a private/incognito window, removes accounts and boards. Download a backup regularly.
- Passwords are never stored, only a salted hash (PBKDF2). Even so, treat the sign-in as a privacy screen for a shared device: someone with full access to the browser could still read the saved board data.

## Not included in this version

- **Email reminders** for cards over 14 days in Backlog. They need a connected email account that a plain web page can't use. Stale cards are still marked on the board with an amber "days in backlog" tag.
- **Sync between devices** and **password reset by email.** Both need a server. Use backups to move your board.

## Forgot your password

There's no reset without a server. You can create a new account on the same device and restore a backup into it.
