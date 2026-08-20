# Consu Privacy Policy

**Last updated: 20 August 2026**

This Privacy Policy explains how Consu ("the app", "we", "our") collects, uses, and protects personal data when you use the Consu mobile application.

## 1. Who we are (data controller)

Consu is developed and operated by:

**Karl Holmes**, sole developer (personal capacity). Based in Ireland. Contact: **privacy@getconsu.com**

For the purposes of the EU General Data Protection Regulation (GDPR) and the Irish Data Protection Act 2018, Karl Holmes is the data controller for the personal data processed through Consu.

## 2. What we collect

Consu is designed to minimise data collection. The following is the full list of information we or our sub-processors handle:

### 2.1 Information you provide directly

- **Media library data** — the films, TV shows, games, books and music you add to your library, along with any ratings, notes, tags, pinned items, custom lists, completion dates and parental-control settings you create.
- **Imported library data** (optional) — if you choose to use one of the importers, Consu reads the file or account you point it at and turns it into library items. This covers the TV Time data export, a Letterboxd CSV export, a Goodreads CSV export, the Spotify listening-history export, a previous Consu JSON backup, a Steam profile you identify by its Steam ID or vanity URL, and a ListenBrainz username you connect (ListenBrainz can itself mirror Last.fm scrobbles, in which case Consu reads them from ListenBrainz and never contacts Last.fm). Consu imports only titles, dates, ratings and play counts; from a connected Steam profile it also reads that profile's public game library and wishlist, your playtimes, and — for the games you have played most — your unlocked achievement counts. Any file you import is read on your device and the file itself is never uploaded to us. You can remove imported items like any other item.
- **Tracked time** — where a title has a known runtime, length or playtime, Consu derives an estimate of the time you have spent on your library and shows it back to you as totals and estimates. This is calculated from the items you have logged; we do not measure your actual usage of other apps or services.
- **Profile information** — a display name, friend code, and optional custom avatar image you choose yourself.
- **Social data** — the friend codes of other Consu users you connect with, the people you follow, the recommendations you send or receive, and the reactions you leave on other people's activity. You control how much of your profile is visible to other people through the Public / Mutuals / Private setting (see section 10).
- **Shared lists and Together queues** (optional) — Consu has two kinds of list, and they are not stored the same way. **Custom Lists** (Settings → Custom Lists) are personal: they live with your own library and nobody else can join them. **Shared Lists** and **Together queues** (Social → Shared Lists & Together) are deliberately multi-person: they are stored in our database with a member list, and every member can see the list's name, its members, the titles added to it, your display name against the titles you added, and everyone's up/down votes. Creating a shared list adds your mutuals as members. Anything you add to one of these is visible to its other members regardless of your profile-visibility setting — see section 10.
- **Account linking data** (optional) — if you choose to link your account to a Google or Apple sign-in provider, we receive the email address associated with that provider to identify your account across devices. If you use Sign in with Apple and choose "Hide My Email," we receive only Apple's anonymised relay address, not your real email.

### 2.2 Information created automatically

- **Anonymous user ID (UID)** — when you first open the app, Firebase Authentication assigns you a random anonymous UID. This UID is used to associate your cloud-synced data with your device. It is not linked to any personally identifying information unless you choose to link a Google or Apple account.
- **Device-local preferences** — theme, accent colour, zoom settings, completed tutorials and similar UI state are stored on your device.
- **Release reminders** (optional, off by default) — if you turn on **Settings → Notifications**, Consu asks your operating system for permission to show notifications and then schedules reminders for episodes and releases that are already in your library. These are ordinary device alarms set by the app: the schedule is calculated on your device, nothing is sent to us or to any push service, and Consu has no push-notification server. Turning the setting off, or revoking the permission in your device settings, cancels them.
- **Last-active timestamp** — the time your library was last synced to the cloud is recorded on your profile. If your profile is visible to other people (see section 10) it can be shown to them as an approximate "last active" time. It is not a precise log of when you opened the app.
- **App-integrity checks** — on Android, Consu uses Firebase App Check with Google Play Integrity to confirm that requests come from a genuine, untampered copy of the app. This produces a short-lived device-integrity token used only to protect the service from abuse; it does not identify you personally. App Check is not currently active on iOS.
- **Crash diagnostics** — when the app crashes, Firebase Crashlytics records the crash stack trace, the operating system version, the device model, the app version, and the breadcrumbs of the most recent in-app actions. This data is automatically generated and does not include the contents of your library or personal messages. You can opt out under **Settings → Diagnostics → Send crash reports**.
- **Usage analytics** — Firebase Analytics records events from a closed, hard-coded list: a signup funnel (first app open, onboarding completion, first item added, first rating, Pro purchase, account deletion), which locked feature opened the Pro upgrade screen, and which recommendation and discovery surfaces you were shown and acted on. These record the *kind* of thing shown, never the thing itself — no title, search term, service name or free text — and are described in full in section 4.1b. Firebase also automatically logs technical events such as screen views and an approximate country derived from your IP address. You can opt out under **Settings → Diagnostics**.

### 2.3 Information we do NOT collect

- We do not use third-party analytics SDKs such as Mixpanel, Segment, Amplitude or advertising-attribution SDKs. The only analytics layer in Consu is the minimal Firebase Analytics funnel described in section 2.2.
- We do not use advertising networks or serve ads, and we do not use the Advertising Identifier (IDFA/AAID).
- We do not collect location data.
- We do not access your contacts, phone, camera roll (except when you explicitly pick an image for your custom avatar), SMS, call log or microphone.
- We do not sell data to third parties. We do not share data with advertisers.

## 3. Why we process your data (purposes and legal basis)

| Purpose | Legal basis (GDPR Article 6) |
|---------|-----|
| Provide the core app functionality (library, stats, social) | Contract (6(1)(b)) |
| Cloud backup and cross-device sync via Firebase | Contract (6(1)(b)) |
| Connect you with friends you choose to add | Contract (6(1)(b)) |
| Process one-time Pro upgrade payments | Contract (6(1)(b)) |
| Diagnose crashes and improve app stability | Legitimate interest (6(1)(f)) |
| Measure aggregate product usage to prioritise improvements | Legitimate interest (6(1)(f)) |
| Verify app integrity and prevent abuse and fraud | Legitimate interest (6(1)(f)) |
| Comply with legal obligations (e.g. tax records for sales) | Legal obligation (6(1)(c)) |

We do not rely on consent as the primary legal basis for the processing above, because the processing is necessary to provide the service you requested or is based on our legitimate interests where the data is minimised and the impact on you is low. You can stop all processing at any time by deleting your account (see section 8). You can opt out of crash diagnostics and analytics under **Settings → Diagnostics**.

## 4. Third-party services and data transfers

Consu uses the following sub-processors. Each has their own privacy policy governing how they handle data.

### 4.1 Firebase (Google Ireland Limited / Google LLC)

Used for:

- **Firebase Authentication** — anonymous UIDs and, if you link your account, Google or Apple sign-in.
- **Firestore** — cloud backup of your library and profile, the friend and follow graph, your activity feed, notifications and reactions, and any shared lists or Together queues you are a member of.
- **Firebase Storage** — custom avatar images (Pro feature).

Data is processed in Google's data centres. Consu's Firestore instance is hosted in the **`europe-west2` (London, United Kingdom)** region. Some core Firebase Authentication services are operated from Google's global infrastructure, including servers in the United States; transfers outside the European Economic Area (EEA) are covered by the EU Standard Contractual Clauses in Google's Data Processing Addendum.

Policy: https://firebase.google.com/support/privacy

### 4.1a Firebase Crashlytics (Google Ireland Limited / Google LLC)

Used to capture crash reports. Crashlytics receives:

- The crash stack trace and exception type.
- Device model, operating-system version, app version and build identifier.
- A breadcrumb log of the most recent app interactions (which screen was open, button taps, etc.) **excluding** the content of any library item, friend message, or profile data.
- Your Firebase UID, used solely to deduplicate crash reports per user.

Crashlytics does not receive your name, email, library contents, or friend codes. Crash data is retained by Google for up to 90 days and then deleted.

You can opt out of crash reporting under **Settings → Diagnostics**. When disabled, no further crash reports are sent.

Policy: https://firebase.google.com/support/privacy

### 4.1b Firebase Analytics (Google Ireland Limited / Google LLC)

Used to measure a minimal funnel of usage signals. Analytics receives:

- **Product events** drawn from a closed, hard-coded list of event names (currently around ninety). These cover a small signup funnel (`install`, `onboarding_complete`, `first_add`, `first_rate`, `pro_purchase`, `account_deletion`), which locked feature opened the Pro upgrade screen, and which recommendation, "Fits tonight", availability and Steam surfaces were shown, opened, added, started or dismissed. The names describe the *kind* of thing shown, never the thing itself: they contain no title, no search term, no service or store name, no Steam ID and no free text. An event name that is not on the list is discarded rather than sent.
- **A small set of event parameters**, each restricted to a fixed list of permitted values: the media category (movies, TV, games, books or music), a position label, how an item was opened, which kind of surface it came from, and a few numeric buckets. A value outside the permitted list is dropped before the event is sent, so these parameters cannot carry library content.
- Auto-collected events such as `screen_view`, `app_open`, and `first_open`.
- An approximate country derived from your IP address. The IP itself is not retained.
- A randomly generated app-instance identifier used to deduplicate sessions.

Analytics does not receive your library contents, friend codes, display name, email, or any in-app messages. Analytics data is retained by Google for up to 14 months (Firebase's default retention) and then deleted. You can opt out under **Settings → Diagnostics**.

Policy: https://firebase.google.com/support/privacy

### 4.2 Cloudflare Worker (Cloudflare, Inc.) — metadata proxy

Consu fetches most media metadata (descriptions, ratings, release dates) through a Cloudflare Worker that proxies requests to the third-party APIs listed in 4.3 below. The Worker:

- Does not receive your Firebase UID, email, display name, or library contents.
- Receives only the media title, ID, or search term you are looking up, plus standard HTTP request metadata (your IP address, user-agent, `Accept` headers) that Cloudflare requires to route the request.
- Uses your IP address solely for short-term rate limiting (a rolling 60-second window, currently 100 requests) to prevent abuse. IP addresses are not persisted to long-term storage by the Worker itself.
- Caches responses at Cloudflare's edge to reduce load on the upstream APIs. How long depends on how fast the data changes — from a few hours for film and TV details up to 7 days for reference data such as Open Library and Wikidata.
- Holds the API keys for those providers that require one, so that no key ever ships inside the app. For IGDB this includes obtaining the access token from **Twitch**, which operates IGDB's authentication: that exchange happens between the Worker and Twitch, so Twitch never sees your device or anything about you.
- Also relays cover images in one specific case: when you generate a shareable image of an item, the artwork is fetched through the Worker so it can be drawn onto the picture. Ordinary browsing does not use this path — see 4.3b.

Cloudflare, acting as an independent processor, may log request metadata in accordance with its own privacy policy.

Policy: https://www.cloudflare.com/privacypolicy/

### 4.3 Third-party metadata providers

Consu displays metadata sourced from the following services. Each receives only the query (e.g. a film title or ISBN) necessary to return a result. None of them receive your Firebase UID, email, or library contents. Section 4.3a explains which of them see your IP address and which do not.

| Service | Purpose | Privacy policy |
|---------|---------|---|
| **TMDB** (The Movie Database) | Film and TV metadata, posters | https://www.themoviedb.org/privacy-policy |
| **OMDB** | Supplementary film metadata (IMDb ratings, runtimes) | https://www.omdbapi.com/ |
| **IGDB** (Twitch / Amazon) | Video-game metadata, cover art, screenshots, release dates and ratings — Consu's primary games source | https://www.twitch.tv/p/legal/privacy-notice/ |
| **RAWG** | Supplementary video-game metadata and screenshots | https://rawg.io/privacy_policy |
| **Steam** (Valve) | Video-game store data, and — only if you connect a Steam profile — that profile's public game library, wishlist, playtimes and achievement counts | https://store.steampowered.com/privacy_agreement/ |
| **Nintendo** (Nintendo of Europe) | Nintendo Switch game listings and pack art | https://www.nintendo.co.uk/Privacy-policy/Privacy-policy-637785.html |
| **Xbox** (Microsoft) | Xbox and Microsoft Store game listings and box art | https://privacy.microsoft.com/privacystatement |
| **PlayStation** (Sony Interactive Entertainment) | PlayStation Store game listings and cover art | https://www.playstation.com/legal/privacy-policy/ |
| **Wikidata** (Wikimedia Foundation) | Awards, release dates, series order, and links between related works | https://foundation.wikimedia.org/wiki/Policy:Privacy_policy |
| **Wikipedia** (Wikimedia Foundation) | Author and artist biographies, critical reception | https://foundation.wikimedia.org/wiki/Policy:Privacy_policy |
| **Google Books** | Book metadata, covers | https://policies.google.com/privacy |
| **Open Library** (Internet Archive) | Supplementary book metadata, including whether a book can be borrowed free | https://archive.org/about/terms |
| **New York Times Books API** | Bestseller lists | https://www.nytimes.com/privacy/privacy-policy |
| **Deezer** | Music track and album metadata | https://www.deezer.com/legal/personal-datas |
| **MusicBrainz** | Open-source music database | https://metabrainz.org/privacy |
| **ListenBrainz** | Listening history, only if you connect a username | https://metabrainz.org/privacy |
| **Cover Art Archive** | Album artwork | https://metabrainz.org/privacy |
| **Apple iTunes Search API** | Music and album metadata, chart listings | https://www.apple.com/legal/privacy/ |

### 4.3a How these requests reach the provider

There are two paths, and the difference matters for your IP address. Where a request is made directly by the app, that provider receives your device's IP address and standard HTTP request metadata, in the same way as if you had opened a page in a browser.

- **Through the Cloudflare Worker** — every service in the table above except the two named below. The provider sees the Worker, not your device, so it does not receive your IP address. Cloudflare does, as described in 4.2.
- **Directly — the Apple iTunes Search API**, because routing it through the Worker is unreliable. Apple receives only the search term or identifier being looked up, never your Firebase UID, email, display name or library contents.
- **Directly — ListenBrainz**, but only if you connect a ListenBrainz account. Your ListenBrainz username is sent so your listening history can be read, and if you supply a ListenBrainz API token (needed only for a private profile) that token is sent with each request to prove you are entitled to it. The token is stored on your device and is never sent anywhere except ListenBrainz. Consu sends ListenBrainz nothing about your Consu account or library.

### 4.3b Artwork and cover images

Posters, box art, album covers, cast photographs and service logos are **loaded directly by your device from each provider's image servers** while you browse — they are not proxied. The image address itself is the only thing sent, but the provider's image server does receive your device's IP address and standard HTTP request metadata, exactly as any website's images would.

The image servers involved belong to the same companies listed in 4.3 — principally TMDB, IGDB, RAWG, Steam, Nintendo, PlayStation, Xbox, Deezer, Apple, Google Books, Open Library and the Wikimedia Foundation (author and artist photographs come from Wikimedia Commons). Their privacy policies are the ones already linked in the table above.

The single exception is described in 4.2: when you generate a shareable image, that artwork is fetched through the Cloudflare Worker instead.

### 4.3c Links out of the app

Some screens offer links to services we do not fetch data from — an **Internet Archive** page where a book can be borrowed free, a store page for a game, a **YouTube** trailer, or a music link-out page. Consu sends nothing to these services unless you tap the link, and nothing from them is embedded in the app. Once you tap, you are on that service's own site and its privacy policy applies.

This product uses the TMDB API but is not endorsed or certified by TMDB. Similarly, Consu is not affiliated with or endorsed by any of the other metadata providers listed.

### 4.4 App-store billing (Apple / Google)

If you purchase Consu Pro, the payment is processed by the app store you bought it through — the **Apple App Store** (Apple Distribution International Ltd.) on iOS, or **Google Play Billing** (Google Ireland Limited) on Android. Consu never sees your card details.

Policies: https://www.apple.com/legal/privacy/ · https://policies.google.com/privacy

### 4.5 RevenueCat (RevenueCat, Inc.)

If you purchase Consu Pro, RevenueCat acts as the purchase-validation layer between the app store (Apple App Store or Google Play) and Consu. RevenueCat receives your anonymous Firebase UID (to associate the purchase with your account) and the standard purchase receipt from Apple or Google. RevenueCat does not receive your name, email, or library contents.

Policy: https://www.revenuecat.com/privacy

### 4.6 Google Fonts (Google Ireland Limited / Google LLC)

Consu's typefaces are loaded from **Google Fonts** when the app opens, and again whenever you open the font picker or choose a different font under Settings → Appearance (opening the picker loads a sample of each font it offers). The stylesheet comes from `fonts.googleapis.com` and the font files themselves from `fonts.gstatic.com`. Google therefore receives your device's IP address and standard HTTP request metadata, along with the name of the typeface being requested. It receives nothing else — no Firebase UID, no email, no library contents — and these requests set no cookie and load no Google script.

Policy: https://policies.google.com/privacy

## 5. Where your data is stored

- **On your device.** Your library is held in the app's own local database, and your settings and preferences alongside it. This is the copy the app reads from, so Consu works with no connection and without an account. Uninstalling the app removes it. **Settings → Reset All Data** clears your library from this device but deliberately leaves your cloud backup in place so you can restore it; to remove everything everywhere, delete your account (section 8).
- **In the cloud, if you are signed in.** Your library is backed up to Firestore under your account, together with a small number of dated restore points so an accidental deletion can be undone (see section 6). A very large library is split across several backup records rather than one; this is a storage detail and changes nothing about who can read it — the records are readable only by your own account.
- Data synced to Firestore and Firebase Storage is hosted in the **`europe-west2` (London, United Kingdom)** region.
- Transfers to Google's US infrastructure for core authentication, Crashlytics, and Analytics services are covered by the EU Standard Contractual Clauses.
- Cloudflare Worker requests are routed through Cloudflare's global edge network.

## 6. How long we keep your data

- While your account is active, we retain your library and profile so that it stays available across your devices.
- **Restore points.** Alongside the current backup we keep up to five dated copies of your library, at most one per day, so that you can undo an accidental deletion. Each new copy replaces the oldest, so nothing older than the last few days of use is retained. You can restore one yourself from **Settings → Data**.
- When you delete your account (see section 8), your Firestore data — including the backup and its restore points — and your Firebase Storage files are deleted immediately. Any residual copies in operational backups or logs are deleted within 30 days.
- Crash reports captured by Crashlytics are retained by Google for up to 90 days and then deleted automatically.
- Analytics events are retained by Google for up to 14 months and then deleted automatically.
- If you simply uninstall the app without deleting your account, your Firestore data remains stored so you can restore it if you reinstall and sign back in. It stays until you delete your account. We may remove data belonging to long-dormant accounts, but we do not commit to a fixed timetable — to have your data erased at any time, use the in-app deletion feature or email us.

## 7. Your rights under GDPR

If you are in the EEA, UK or Switzerland you have the right to:

- **Access** — request a copy of the personal data we hold about you.
- **Rectification** — correct inaccurate data (you can edit most of it yourself in the app).
- **Erasure** ("right to be forgotten") — delete your data, primarily by using the in-app deletion feature.
- **Restriction** — ask us to limit how we process your data.
- **Portability** — receive your data in a machine-readable format. Consu lets you export your full library as JSON from **Settings → Data → Export JSON**, free and with no account requirement. A spreadsheet-friendly CSV export is also offered as part of the paid Pro upgrade; this is a convenience format only, and it does not affect your right to obtain your data free of charge through the JSON export or by emailing us.
- **Objection** — object to processing based on legitimate interests, including crash diagnostics and analytics. You can exercise this directly in the app under **Settings → Diagnostics**.
- **Withdraw consent** — where processing is based on consent.
- **Lodge a complaint** with the Irish Data Protection Commission (https://www.dataprotection.ie) or your local EEA data-protection authority.

To exercise any of these rights, email **privacy@getconsu.com**. We will respond within one month.

## 8. How to delete your data

In the app: scroll to the bottom of **Settings**, tap **Delete My Account & All Data**, type `DELETE`, confirm. This removes your profile, library, ratings, cloud backup and its restore points, friend connections, follow graph, feed activity, notifications, reactions, public profile, custom avatar and Firebase Auth account. For users who signed in with Apple, we also revoke the Apple sign-in token as part of deletion.

**What may survive in someone else's account, and how to have it removed.** Some things you create are, by design, copies held by other people:

- A **Shared List** or **Together queue** belongs to all of its members. Deleting your account removes you from the member list, but the list itself, the titles you added and your votes remain for the other members. Remove them from the list before you delete your account if you want them gone.
- A **recommendation** you sent, and the notification announcing it, sit in the recipient's account. Deleting your account clears these from the accounts of people you follow and people who follow you. If one somehow remains, tell us and we will remove it.

If anything of yours is still visible after deletion, or the in-app flow fails for any reason, email **privacy@getconsu.com** from the address linked to your account — or with your display name and friend code — and we will delete it manually.

## 9. Children

Consu is intended for users aged 13 and over and is not directed at children under 13. The age ratings shown on the Apple App Store and Google Play describe content suitability and are set through each store's own questionnaire; the minimum age for using Consu is the one stated in our Terms of Service.

In countries where the digital age of consent under GDPR is higher than 13 (Ireland: 16; Germany: 16; Netherlands: 16; Italy: 14; France: 15; etc.), users under that age must have the consent of a parent or legal guardian to use Consu. If we become aware that we have collected personal data from a child below the applicable age without parental consent, we will delete it.

Parents: to request deletion of a child's data, email **privacy@getconsu.com**.

## 10. Profile visibility — who else can see your data

Firebase Storage and Firestore enforce per-user security rules. What other people can see depends on the visibility setting you choose for your profile:

- **Private** — no other user can read your library or profile.
- **Mutuals** — only people you and they both follow each other ("mutuals") can see your full library and profile.
- **Public** — your display name, avatar and a snapshot of your library are visible to other Consu users, including through the in-app Explore surface. Public-profile data is readable by anyone using the app.

Where your profile is visible, it can include your display name and avatar, a snapshot of your library and ratings, your taste statistics, what you are currently reading, watching or playing, your follower and following counts, your estimated tracked time, the milestones you have earned and your current day-streak, and an approximate last-active time.

You can change this setting at any time in the app, and you can choose which sections are included. Seven parts of your profile have their own switch: top-rated items, what you are currently consuming, your backlog, your taste statistics and genres, your completed count, hours tracked, and achievements and streak.

Two levels of control, and the difference matters:

- **The seven section switches apply to your public profile.** They govern what strangers and people who merely follow you can see. **Mutuals see your full library regardless of them** — that is what choosing the Mutuals tier means, and the switches are not a way to keep something from someone you follow each other with.
- **Hiding a category hides it from everyone, mutuals included.** If you want your books private but your films visible, hide the category.

Either way the effect is real rather than cosmetic: hidden content is stripped before your profile is written out, so it never leaves your device.

**Two things this setting does not cover.** Setting your profile to Private does not retract them, so they are worth knowing about:

- **Shared Lists and Together queues.** These are joint by nature. The other members can always see the list, its members, the titles you added, your display name against them and your votes. Leave the list, or remove your items from it, if you do not want that.
- **Recommendations you send.** Sending someone a recommendation shows them the title and that it came from you.

Separately, you can **block** another user at any time from their profile, and review or undo that under **Settings → Blocked Users**.

## 11. Security

- All traffic between the app and any external service — Firebase, the Cloudflare Worker, and the services named in section 4 — is encrypted with TLS.
- Firestore and Firebase Storage enforce per-user security rules so that data is only readable in line with your chosen visibility setting (see section 10).
- Your password is never handled by Consu — authentication is delegated to Google or Apple.

No system is perfectly secure. If you believe your account has been compromised, contact **privacy@getconsu.com** and change your linked Google or Apple account password immediately.

## 12. Changes to this policy

We may update this Privacy Policy to reflect changes to the app, legal requirements, or sub-processors. The "Last updated" date at the top of this document indicates when the most recent change was made. Material changes will be announced in the app before they take effect.

## 13. Contact

For any privacy-related question, request or complaint:

**Karl Holmes** — privacy@getconsu.com
