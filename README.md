# SkillMart

SkillMart is a single-file, client-side marketplace web app prototype for buying/selling items and offering/hiring skills nearby. It includes:

- Email/password signup + login
- A home feed with search, category filters, and item/skill toggles
- Create listing modal with multi-image upload
- Listing details modal with favorite + chat + offer actions
- chat between users
- Favorites page
- Profile page with basic stats
- Settings modal (dark mode + miles/km + location update)
- Admin dashboard (hardcoded credentials) for managing users, listings, and chat logs

---

Demo / How It Works

This app runs entirely in the browser:

- Users can create accounts, post listings, favorite listings, and chat with other users.
- Admin can log in to view platform stats and moderate users/listings/chats.

---

Features

Marketplace
- Post Items or Skills
- Assign a Category
- Set a Price or Hourly Rate
- Add multiple photos (preview + remove)
- Feed filtering by:
  - Type: All / Items / Skills
  - Category chips
  - Search by title
- Featured/promoted display support (admin-controlled)

Favorites
- Heart icon toggles saved listings

Chat
- 1:1 conversations between buyer and seller
- Unread message badge
- Message read state (simple `read` boolean)
- Delete conversation (user) and delete chat logs (admin)

Offers
- “Make Offer” sends an offer message into the chat thread
- Offer content is formatted into the message text and marked with `isOffer`

Settings
- Dark mode toggle
- Distance unit toggle (km/miles display)
- Update user location text

Admin Dashboard
- Login via hardcoded credentials
- Tabs: Overview / Users / Listings / Chat Logs / Analytics / System
- User actions:
  - Terminate/restore
  - Suspend/unsuspend
  - Reset password (random password shown in toast)
  - View user detail modal
- Listing actions:
  - Edit listing
  - Feature/unfeature
  - Delete listing
- Chat logs:
  - View message history
  - Delete conversation
