# Consu Privacy Policy

**Last updated: 27 October 2026**

This Privacy Policy explains how Consu ("the app", "we", "our") collects, uses, and protects personal data when you use the Consu mobile application, and the public profile pages Consu publishes on getconsu.com.

## 1. Who we are (data controller)

Consu is developed and operated by:

**Karl Holmes**, sole developer (personal capacity). Based in Ireland. Contact: **privacy@getconsu.com**

For the purposes of the EU General Data Protection Regulation (GDPR) and the Irish Data Protection Act 2018, Karl Holmes is the data controller for the personal data processed through Consu.

## 2. What we collect

Consu is designed to minimise data collection. The following is the full list of information we or our sub-processors handle:

### 2.1 Information you provide directly

- **Media library data** — the films, TV shows, games, books and music you add to your library, along with your ratings (including per-episode ratings), statuses, progress, notes, reviews, tags, favourites, favourite characters, custom lists, start and finish dates, rewatch counts, who recommended a title to you (a name you type, or the person you added it from), what you paid for it, the platform or service you used for it, and parental-control settings. A cover image you upload for a title yourself is stored inside that title; a cover you set by pasting an image address is stored as that address and loads from it (section 4.3b). Notes and prices are never shown to anyone else; reviews can be (section 10).
- **Imported library data** (optional) — under **Settings → Your data → Import**, Consu reads the file or account you point it at and turns it into library items. The sources are a Letterboxd export, a Goodreads export, a TV Time data export (or a TV Time app cache file recovered from a phone backup, and a TV Time ratings file), the Spotify extended streaming history, a ListenBrainz username you connect (ListenBrainz can itself mirror Last.fm scrobbles, in which case Consu reads them from ListenBrainz and never contacts Last.fm), a Steam profile you identify by its Steam ID or profile address, a list of game titles you type or pick as a text file, and a previous Consu backup. Depending on the source, Consu brings across titles, years, ratings, shelves, start and finish dates, reviews, rewatch and re-read counts, which episodes you watched (with when you first and last watched each show), favourites, authors, page counts, ISBNs, and minutes listened with your first and last listening dates; a Consu backup brings back every field it holds. Goodreads reviews marked as containing spoilers are left behind. Imported reviews are treated like the reviews you write (section 10). Any file you import is read on your device and the file itself is never uploaded to us. To match each title, Consu looks it up by name, year, author, ISBN or catalogue ID through the Cloudflare Worker described in section 4.2.
- **A connected Steam profile or ListenBrainz account** (optional) — from a Steam profile, Consu reads its public game library and wishlist, your total and recent playtime, when you last played each game, and, when you open a game's card or your Journey numbers, the achievements you have unlocked with their dates. While a Steam profile is connected, Consu refreshes those playtimes about once a day and store prices about once a week. While a ListenBrainz username is connected, Consu reads your new listens about once a day. Your Steam ID and ListenBrainz details are stored only on your device; they are sent with each request that reads the profile (sections 4.2 and 4.3a). A Steam profile or ListenBrainz username counts as connected only once an import from it has finished. While one is connected, **Settings → Your data** lists it with **Sync now** and **Disconnect**: Disconnect removes its details from your phone and stops its syncs, and the titles already imported stay. Deleting your account, signing in to another account that already has Consu, or uninstalling the app disconnects them too (Settings → Reset this phone keeps them).
- **Tracked time** — where a title has a known runtime, length or playtime, Consu derives an estimate of the time you have spent on your library and shows it back to you as totals and estimates. This is calculated from the items you have logged, and from the playtime Steam recorded and the minutes in your listening history where you connected or imported them; Consu does not measure your use of other apps or services itself.
- **Profile information** — a display name, a friend code generated for you, an avatar (an octopus in a colour you pick or, with Pro, a photo of your own), a profile colour and card frame, up to five favourite titles, and your privacy choices (section 10).
- **Social data** — the people you follow and who follow you; the posts Consu makes when you start or finish something (section 10.3); the reactions and replies you leave on posts, including the people you @name; the titles you send to other people, with any note you add (up to 200 characters); the people you hide from Explore or block; and any report you make about a profile, a review or a reply (section 10.5).
- **Shared lists and Together queues** (optional) — Consu has two kinds of list, and they are not stored the same way. **Lists** (Settings → Library → Lists) are personal: they live with your own library and nobody else can join them. **Shared Lists** and **Together queues** are deliberately multi-person: they are stored in our database with a member list, and every member can see the list's name, its members and the titles added to it, with which member added each; on a Shared List also the display name of whoever added each title, and everyone's votes, reactions and "seen" marks. A Shared List made in an earlier version of Consu added all of its maker's mutuals as members, without asking them; this version of the app cannot make new ones, and these screens open only for people who already belong to a list or queue. You can leave a list or queue at any time (section 10.5). Anything you add to one is visible to its other members regardless of your profile-visibility setting — see section 10.
- **Account linking data** (optional) — if you link your account to Google (on Android or iPhone) or Apple (on iPhone), we receive the email address associated with that provider to identify your account across devices. It is shown to you in the app; it is not part of your profile and other users cannot see it. If you use Sign in with Apple and choose "Hide My Email," we receive only Apple's anonymised relay address, not your real email.

### 2.2 Information created automatically

- **Anonymous user ID (UID)** — when you first open the app, Firebase Authentication assigns you a random anonymous UID. It identifies your records in our database, and it is also given to RevenueCat (section 4.5). It is not linked to any personally identifying information unless you choose to link a Google or Apple account.
- **Records kept before you sign in** — your library is backed up to the cloud only once you link Google or Apple (section 5), and Consu writes no posts before then. Earlier versions did write a guest's posts to our database; this version deletes them the first time it opens while you are still a guest. If you have Pro and choose a profile photo before signing in, the photo is uploaded (section 11). If you later sign in to a Google or Apple account that already has Consu, instead of linking this one, what the guest left (its sign-in record, a photo, and any posts from an earlier version not yet deleted) stays under the guest UID, where the app's account deletion cannot reach it; email us to have it removed.
- **Data kept on your device** — your library, settings and preferences are kept on your device (section 5). Some of it is stored only on your device, never in your backup or our database: dark mode and whether the app follows your phone's appearance, your parental PIN, your streaming region, vibration, which tips and introduction screens you have seen (the Social tab's notices about your profile and web page are recorded with your profile instead), your recent searches and recently viewed titles, the For You picks you dismissed and the creators whose alerts you muted, text you have typed but not yet sent (up to 40 drafts, each kept for up to 30 days, so closing a sheet does not lose it), your reminder settings, your Steam and ListenBrainz details, your app icon and your import receipts. Your region and your Steam and ListenBrainz details are still sent with the lookups that need them (sections 2.3, 4.2 and 4.3a). Your other preferences, such as your theme, font, text size, rating style, streaming services, blocked people and Journey card, are included in your cloud backup when you are signed in. Consu also keeps a cache of the details it has looked up, so it can work offline.
- **Reminders and alerts** (optional, off by default) — if you turn on **Settings → Discover and watching → Episode reminders**, Consu asks your operating system for permission to show notifications and then schedules reminders on your device for episodes airing in shows on your Current or Upcoming shelf, new albums from the artists most in your library, and, with Pro, titles on your list arriving on one of your streaming services. These are ordinary device alarms set by the app: the schedule is worked out on your device, and Consu has no push-notification server. To find new albums and arrivals, Consu looks those artists and titles up through the Cloudflare Worker (section 4.2). Turning the setting off cancels them; revoking the permission in your device settings stops them being shown.
- **Last-active time** — each time your profile is synced (when you open the app, and when you change your library) the exact time is stored with your profile, in the records other people can read (section 10). The app shows it to them as an approximate "last active" time, such as "Active today", and Explore can order people by it. It is not published while your profile is Private.
- **App-integrity checks** — Consu uses Firebase App Check to confirm that requests come from a genuine, untampered copy of the app: it asks Google Play Integrity on Android, and Apple's App Attest on iPhone, for a short-lived integrity token, used only to protect the service from abuse; the token does not identify you personally.
- **Crash diagnostics** — when the app crashes or hits an unexpected error, Firebase Crashlytics records the error and its stack trace, the operating system version, the device model, the app version, the screens and sheets you last opened (some carrying a genre or a title's internal ID), and whether a network request had just failed. Crash reports do not include your UID, the contents of your library or anything you have written. They are on unless you turn off **Settings → Privacy and safety → Crash reports**.
- **Usage analytics** — Firebase Analytics records which parts of the app are used, from a closed, hard-coded list of events: for example a sheet opening, a title added from a particular row, a tab switched, an import started or finished, a tip shown, or the Pro screen opened from a particular feature. An event records the *kind* of thing that happened, never which title, person, search or text was involved, and is described in full in section 4.1b. Firebase also automatically logs technical events such as screen views, app opens and in-app purchases, and an approximate location (country, region and city) derived from your IP address. Analytics is on unless you turn off **Settings → Privacy and safety → Usage analytics**.

### 2.3 Information we do NOT collect

- We do not use third-party analytics SDKs such as Mixpanel, Segment, Amplitude or advertising-attribution SDKs. The only analytics layer in Consu is the Firebase Analytics described in section 2.2.
- We do not use advertising networks or serve ads. Consu does not use the advertising identifier (IDFA/AAID): on Android it removes the advertising-ID permissions Google Play services would add and switches off Firebase Analytics' collection of the advertising ID, and on iPhone it never asks for tracking permission.
- We do not collect your precise location. Consu works out a country from your phone's time zone and language settings (or uses the streaming region you choose), and sends that two-letter country code with store and catalogue lookups so that prices and availability match your region. Analytics derives only an approximate location (country, region and city) from your IP address.
- We do not access your contacts, phone, SMS, call log or microphone. Consu uses your photo library only when you choose a picture: a profile photo, or a cover image for a title; on iPhone you can also take a photo with the camera for either. On iPhone, when you choose **Save Image** from the share sheet, Consu asks to add that one image to your photo library; this permission lets it add images, not read your photos.
- We do not sell data to third parties. We do not share data with advertisers.

## 3. Why we process your data (purposes and legal basis)

| Purpose | Legal basis (GDPR Article 6) |
|---------|-----|
| Provide the core app functionality (library, stats, imports, reminders) | Contract (6(1)(b)) |
| Cloud backup and cross-device sync via Firebase | Contract (6(1)(b)) |
| The social features: following, posts, replies, reactions, sending titles, shared lists, and showing your profile to the people your settings allow, including on the web | Contract (6(1)(b)) |
| Process one-time Pro upgrade payments | Contract (6(1)(b)) |
| Diagnose crashes and improve app stability | Legitimate interest (6(1)(f)) |
| Measure aggregate product usage to prioritise improvements | Legitimate interest (6(1)(f)) |
| Verify app integrity, prevent abuse and fraud, and act on reports | Legitimate interest (6(1)(f)) |
| Comply with legal obligations (e.g. tax records for sales) | Legal obligation (6(1)(c)) |

We do not rely on consent as the primary legal basis for the processing above, because the processing is necessary to provide the service you requested or is based on our legitimate interests where the data is minimised and the impact on you is low. You can stop all processing at any time by deleting your account (see section 8). You can opt out of crash diagnostics and analytics under **Settings → Privacy and safety**.

## 4. Third-party services and data transfers

Consu uses the following sub-processors. Each has their own privacy policy governing how they handle data.

### 4.1 Firebase (Google Ireland Limited / Google LLC)

Used for:

- **Firebase Authentication** — anonymous UIDs and, if you link your account, Google or Apple sign-in.
- **Firestore** — your profile and privacy choices; the cloud backup of your library and its dated copies; the follow graph; your posts and the reactions and replies on them; the titles people send each other, and notifications; the copies of your profile that other people can read (section 10); reports; and any shared lists or Together queues you are a member of.
- **Firebase Storage** — your profile photo, if you upload one (Pro feature).

Data is processed in Google's data centres. Consu's Firestore instance is hosted in the **`europe-west2` (London, United Kingdom)** region. Some core Firebase Authentication services are operated from Google's global infrastructure, including servers in the United States; transfers outside the European Economic Area (EEA) are covered by the EU Standard Contractual Clauses in Google's Data Processing Addendum.

Policy: https://firebase.google.com/support/privacy

### 4.1a Firebase Crashlytics (Google Ireland Limited / Google LLC)

Used to capture crash and error reports. Crashlytics receives:

- The crash or error, its stack trace and exception type.
- Device model, operating-system version, app version and build identifier.
- A short log of the screens and sheets you last opened (some carrying a genre or a title's internal ID), and whether a network request had just failed.
- A random identifier for this installation of the app, which Crashlytics creates to count how many installs a crash affects.

Crash reports do not include your Firebase UID, name, email or library contents (earlier versions of the app sent the UID with them). Crash data is retained by Google for up to 90 days and then deleted.

You can turn crash reporting off under **Settings → Privacy and safety → Crash reports**; reports stop from the next time the app starts. The choice is kept on your device, and it stays as you set it when you delete your account or sign in to another account that already has Consu; a new install starts with crash reporting on again.

Policy: https://firebase.google.com/support/privacy

### 4.1b Firebase Analytics (Google Ireland Limited / Google LLC)

Used to measure how the app is used. Analytics receives:

- **Product events** drawn from a closed, hard-coded list of event names (currently about 330). They cover the first-run and sign-up steps (`onboarding_complete`, `first_add`, `first_rate` and similar), imports (started, finished, failed, undone), Pro (a trial started, a purchase or restore, which feature opened the Pro screen), a daily "app active" event, and how features are used across Discover, the detail sheet, the Feed, Explore, profiles, Journey, recommendations, tips and settings such as the app icon. The names describe the *kind* of action, never its subject: they contain no title, no person, no search term, no review or other text, and no Steam ID. An event name that is not on the list is discarded rather than sent.
- **A small set of event parameters**, each restricted to a fixed list of permitted values: the media category, a position or row label, how an item was added (a long press or its page), which kind of surface it came from, small numeric buckets (such as how many titles an import brought in, or roughly how big your library is), which import source was used (such as Letterboxd or Steam), which Pro feature was involved and whether this phone has used the free trial, what prompted a request for a store rating, how far off an upcoming release is, the time window chosen in Fits tonight, which first-run step was reached, which tip was shown, the app icon colour chosen, and whether your account is linked to Google or Apple or still anonymous. A value outside the permitted list is replaced or dropped before the event is sent, so these parameters cannot carry library content.
- Auto-collected events such as `screen_view`, `app_open`, `first_open` and `in_app_purchase` (for a purchase, the product and its price).
- An approximate location (country, region and city) derived from your IP address. The IP itself is not retained.
- The device details Firebase attaches to every event: device model, operating-system version, app version and language, and, on Android, Google Play's install referrer (which store listing or campaign led to the install).
- A randomly generated app-instance identifier used to deduplicate sessions, and, on iPhone, Apple's identifier for vendor (an ID that only apps from the same developer share).

Analytics does not receive your library contents, friend code, display name, email, Firebase UID, or anything you write. Analytics data is retained by Google for up to 14 months and then deleted. You can turn it off under **Settings → Privacy and safety → Usage analytics**. The choice is kept on your device, and it stays as you set it when you delete your account or sign in to another account that already has Consu; a new install starts with analytics on again.

Policy: https://firebase.google.com/support/privacy

### 4.2 Cloudflare Worker (Cloudflare, Inc.) — metadata proxy

Consu fetches most media metadata (descriptions, ratings, release dates) through a Cloudflare Worker that proxies requests to the third-party APIs listed in 4.3 below. The Worker:

- Receives only what is being looked up (a title, catalogue ID, search term, ISBN, artist name, Steam ID or image address, with your region's two-letter country code and, when a list is filtered to your streaming services, which services those are), plus standard HTTP request metadata (your IP address, user-agent, `Accept` headers) that Cloudflare requires to route the request. Some lookups name several titles from your library at once: the Steam games on your list when Consu checks their prices, and the books and games you rated highly when it looks for more like them. It does not receive your email or display name, and it receives your Firebase UID only inside your profile photo's address, when your Journey card's share sheet or Poster Wall draws the photo.
- Passes nothing about your device on to the provider: the provider sees the Worker, not your IP address.
- Uses your IP address solely for short-term rate limiting (a 60-second window, currently 100 requests) to prevent abuse. IP addresses are not persisted to long-term storage by the Worker itself.
- Caches successful lookups at Cloudflare's edge to reduce load on the upstream APIs. A cached entry is keyed by the request, so it can hold the title or Steam profile that was looked up, but nothing that says who asked. How long depends on how fast the data changes: from ten minutes for Steam profile data and six hours for TMDB's film and TV details, up to 7 days for slower-changing data such as Open Library, Wikidata, IGDB and OMDb. Of the images it relays (below), album covers from the Cover Art Archive are kept for up to 7 days, and the pictures in a share image, your profile photo included, for up to a day.
- Holds the API keys for those providers that require one, so that no key ever ships inside the app. For IGDB this includes obtaining the access token from **Twitch**, which operates IGDB's authentication: that exchange happens between the Worker and Twitch, so Twitch never sees your device or anything about you.
- Relays images in two cases: album covers from the Cover Art Archive, which always come through the Worker, and the pictures in an image Consu draws for you to share (your Journey card or Poster Wall): when you open its share sheet or Poster Wall, the covers and your profile photo are fetched through the Worker so they can be drawn onto it. Other artwork loads directly — see 4.3b.

Cloudflare, acting as an independent processor, may log request metadata in accordance with its own privacy policy.

Policy: https://www.cloudflare.com/privacypolicy/

### 4.3 Third-party metadata providers

Consu displays metadata sourced from the following services. Each receives only the query (e.g. a film title or ISBN) necessary to return a result; a few lookups name several titles at once (4.2). None of them receive your Firebase UID, email, or your library as a whole. Section 4.3a explains which of them see your IP address and which do not.

| Service | Purpose | Privacy policy |
|---------|---------|---|
| **TMDB** (The Movie Database) | Film and TV metadata, posters, cast and crew, and streaming availability (supplied to TMDB by JustWatch) | https://www.themoviedb.org/privacy-policy |
| **OMDB** | Supplementary film metadata (IMDb ratings, runtimes) | https://www.omdbapi.com/ |
| **IGDB** (Twitch / Amazon) | Video-game metadata, cover art, screenshots, release dates and ratings — Consu's primary games source | https://www.twitch.tv/p/legal/privacy-notice/ |
| **RAWG** | Supplementary video-game metadata and screenshots | https://rawg.io/privacy_policy |
| **Steam** (Valve) | Video-game store data and prices, and — only if you connect a Steam profile — that profile's public game library, wishlist, playtimes and achievements | https://store.steampowered.com/privacy_agreement/ |
| **Nintendo** (Nintendo of Europe) | Nintendo Switch game listings and pack art | https://www.nintendo.co.uk/Privacy-policy/Privacy-policy-637785.html |
| **Xbox** (Microsoft) | Xbox and Microsoft Store game listings and box art | https://privacy.microsoft.com/privacystatement |
| **PlayStation** (Sony Interactive Entertainment) | PlayStation Store game listings and cover art | https://www.playstation.com/legal/privacy-policy/ |
| **Wikidata** (Wikimedia Foundation) | Awards, release dates, series order, and links between related works | https://foundation.wikimedia.org/wiki/Policy:Privacy_policy |
| **Wikipedia** (Wikimedia Foundation) | Author and artist biographies, critical reception | https://foundation.wikimedia.org/wiki/Policy:Privacy_policy |
| **Google Books** | Book metadata, covers | https://policies.google.com/privacy |
| **Open Library** (Internet Archive) | Supplementary book metadata, including whether a book can be borrowed free | https://archive.org/about/terms |
| **New York Times Books API** | Bestseller lists and book reviews | https://www.nytimes.com/privacy/privacy-policy |
| **Deezer** | Music track and album metadata, covers, song previews, and new albums from your artists | https://www.deezer.com/legal/personal-datas |
| **MusicBrainz** | Open-source music database | https://metabrainz.org/privacy |
| **ListenBrainz** | Listening history, only if you connect a username | https://metabrainz.org/privacy |
| **Cover Art Archive** | Album artwork | https://metabrainz.org/privacy |
| **Apple iTunes Search API** | Music and album metadata, chart listings, song previews | https://www.apple.com/legal/privacy/ |
| **YouTube** (Google) | Trailer thumbnails; a trailer opens on YouTube when you tap it | https://policies.google.com/privacy |

### 4.3a How these requests reach the provider

There are two paths, and the difference matters for your IP address. Where a request is made directly by the app, that provider receives your device's IP address and standard HTTP request metadata, in the same way as if you had opened a page in a browser.

- **Through the Cloudflare Worker** — every service in the table above except the ones named below. The provider sees the Worker, not your device, so it does not receive your IP address with the lookup (its image servers are a different matter: 4.3b). Cloudflare does, as described in 4.2.
- **Directly — the Apple iTunes Search API**, because routing it through the Worker is unreliable. Apple receives only the search term, the album being looked up, or your region's two-letter store code when Consu reads the album charts — never your Firebase UID, email, display name or library.
- **Directly — ListenBrainz**, but only if you connect a ListenBrainz account. Your ListenBrainz username is sent so your listening history can be read (about once a day while it is connected), and if you supply a ListenBrainz API token (needed only for a private profile) that token is sent with each request to prove you are entitled to it. The token is stored on your device and is never sent anywhere except ListenBrainz. Consu sends ListenBrainz nothing about your Consu account or library.
- **YouTube** is not asked for any data; only its trailer thumbnails load, as images (4.3b).

### 4.3b Artwork, previews and other images

Posters, box art, album covers, cast and author photographs, service logos, trailer thumbnails, other people's profile photos and short song previews are **loaded directly by your device from each provider's servers** while you browse — they are not proxied. The address itself is the only thing sent, but the provider's server does receive your device's IP address and standard HTTP request metadata, exactly as any website's images would.

The servers involved belong to the same companies listed in 4.3 — principally TMDB, IGDB, RAWG, Steam, Nintendo, PlayStation, Xbox, Deezer, Apple, Google (Google Books covers, the New York Times' bestseller covers, YouTube thumbnails and profile photos in Firebase Storage), Open Library and the Wikimedia Foundation (author and artist photographs come from Wikimedia Commons). Their privacy policies are the ones already linked in the table above.

A cover you set by pasting an image address (section 2.1) loads from that address on your own phone, whatever server it is on. Other people see it, on your profile in the app or on your web page, only when the address is an https address on one of these image servers: TMDB, RAWG, Open Library, Google Books, Apple, Deezer, Steam, IGDB, Nintendo, PlayStation, the Microsoft Store, the Cover Art Archive, the Internet Archive or Wikimedia; from any other address they see the catalogue's cover instead, and Consu leaves the address out of your profile. That server receives each viewer's IP address in the same way.

The exceptions are described in 4.2: album covers from the Cover Art Archive, and the images Consu draws for you to share, are fetched through the Cloudflare Worker instead.

### 4.3c Links out of the app

Many screens link to other services: where to watch, buy, play, read or listen (for example TMDB's watch page, Google Play, Amazon, Steam, the PlayStation, Xbox and Nintendo stores, the App Store, Epic Games, GOG, itch.io, the Internet Archive, Open Library, Kindle, Audible, Spotify, Apple Music, YouTube Music, Deezer, Tidal, album.link and Last.fm), trailers on YouTube or the video host a game's listing names, Wikipedia, a title's official website and New York Times reviews. A link carries what is needed to open the right page, such as the title or ISBN. Consu sends nothing to these services unless you tap the link. Once you tap, you are on that service's own site and its privacy policy applies.

This product uses the TMDB API but is not endorsed or certified by TMDB. Similarly, Consu is not affiliated with or endorsed by any of the other metadata providers listed.

### 4.4 App-store billing and store services (Apple / Google)

If you purchase Consu Pro, the payment is processed by the app store you bought it through — the **Apple App Store** (Apple Distribution International Ltd.) on iOS, or **Google Play Billing** (Google Ireland Limited) on Android. Consu never sees your card details. The app also uses each store's own services to show its rating prompt and, on Android, to check whether an update is available.

Policies: https://www.apple.com/legal/privacy/ · https://policies.google.com/privacy

### 4.5 RevenueCat (RevenueCat, Inc.)

RevenueCat acts as the purchase-validation layer between the app store (Apple App Store or Google Play) and Consu. Each time the app starts it gives RevenueCat your Firebase UID, whether or not you have bought anything, so RevenueCat can say whether your account owns Consu Pro; if you buy Pro, RevenueCat also receives the standard purchase receipt from Apple or Google. RevenueCat does not receive your name, email, or library contents. When you delete your account, our monthly clean-up deletes your customer record at RevenueCat (your account ID and the receipts it was given); a purchase stays with Apple or Google.

Policy: https://www.revenuecat.com/privacy

### 4.6 Google Fonts (Google Ireland Limited / Google LLC)

Consu's default typeface is built into the app. The other typefaces are loaded from **Google Fonts**: each time the app opens while you have one of them chosen, whenever you open the font picker under **Settings → Look → Font** (which loads each font it offers), and while you try a Pro font. The stylesheet comes from `fonts.googleapis.com` and the font files themselves from `fonts.gstatic.com`. Google therefore receives your device's IP address and standard HTTP request metadata, along with the names of the typefaces being requested. It receives nothing else — no Firebase UID, no email, no library contents — and these requests set no cookie and load no Google script.

Policy: https://policies.google.com/privacy

### 4.7 getconsu.com (Cloudflare, Inc.)

The website at getconsu.com, including the public profile pages described in section 10.6, is served by Cloudflare. It sets no cookies and loads no analytics and no third-party scripts. Cloudflare receives your IP address and standard request metadata in order to serve the page, as for any website. A profile page is built from the public profile index (section 10.6) each time it is requested, and Cloudflare may hold a copy for up to a minute. The cover images and profile photo on a profile page load from the same image servers as in the app (4.3b).

Policy: https://www.cloudflare.com/privacypolicy/

## 5. Where your data is stored

- **On your device.** Your library is held in the app's own local database, and your settings, preferences, drafts and the cache described in section 2.2 alongside it. This is the copy the app reads from, so Consu works with no connection and without an account. Uninstalling the app removes it. **Settings → Reset this phone** removes the titles on this phone and the recommender names you typed, and resets your categories and monthly goal; it keeps your lists, your preferences, any Steam or ListenBrainz connection and your cloud backup, so the titles can be restored; once you add titles again, a new backup can replace it, and its dated copies (section 6) then keep the earlier titles for a few days. On a phone that has run Consu since before version 3.1, an older copy of the library kept from that update stays in the app's storage until you uninstall the app; the app reads it only on a phone where it has never saved your library, so it does not bring titles back after a reset. To remove your data from our servers, delete your account (section 8).
- **In the cloud, once you link Google or Apple.** With auto-backup on (the default), your library and your preferences are backed up to Firestore under your account, together with a small number of dated copies so an accidental deletion can be undone (see section 6). A very large library is split across several backup records rather than one; this is a storage detail and changes nothing about who can read it — the records are readable only by your own account. Each backup also carries a random ID for the phone that wrote it, so that one phone cannot overwrite a newer copy from another. You can manage this under **Settings → Backups**.
- **In the cloud, whether or not you back up.** Your posts (once you have signed in, section 2.2), the list of posts you have hidden (kept beside your backup, readable only by your account), your profile and the copies of it that other people can read (section 10), the people you have blocked (section 10.5), and anything you send, react with or reply.
- Data synced to Firestore and Firebase Storage is hosted in the **`europe-west2` (London, United Kingdom)** region.
- Transfers to Google's US infrastructure for core authentication, Crashlytics, and Analytics services are covered by the EU Standard Contractual Clauses.
- Cloudflare Worker requests are routed through Cloudflare's global edge network.

## 6. How long we keep your data

- While your account is active, we retain your library and profile so that it stays available across your devices.
- **Restore points.** Alongside the current backup we keep up to five earlier copies of your library, at most one per day. Each day's copy replaces an older one, so the copies usually cover your last few days of use; if you have not used the app every day, one can be older. You can restore one yourself from **Settings → Backups**. With a very large library, pieces of older backups can remain until we clear them; like the rest of your backup, only your account can read them, and they are deleted with it.
- **Posts** stay in your activity history until you delete your account, except that hiding a category deletes the posts already made in it (section 10.4). Hiding a post takes it out of other people's feeds in the app (section 10.3), and while your profile is Private nobody else can read your posts at all. No post is made while your profile is Private, for a title in a category you hide, or for a title whose post you have hidden; turning off **Post when I start** stops future posts about starting something, and turning off **Share my reviews** keeps your reviews out of future posts.
- **Reports** are kept for two years from the report, also after either account involved is deleted, so that we can act on repeated abuse; our monthly clean-up deletes older ones.
- When you delete your account (see section 8), the records it lists are deleted from Firestore and Firebase Storage straight away. Consu first writes a short note that the account is being deleted (its account ID, whether it was a guest, and when); our monthly clean-up uses it to remove anything the app could not reach, such as a guest's sign-in record, what you sent or wrote to people you were no longer connected to, and your customer record at RevenueCat, and then deletes the note. Google's data-processing terms allow it up to 180 days to clear deleted data from its own systems, such as its backups.
- Crash reports captured by Crashlytics are retained by Google for up to 90 days and then deleted automatically.
- Analytics events are retained by Google for up to 14 months and then deleted automatically.
- If you simply uninstall the app without deleting your account, your cloud data remains stored so you can restore it if you reinstall and sign back in. It stays until you delete your account. If you never linked Google or Apple, there is no way to sign back in after an uninstall, so delete your account in the app first, or email us. We may remove data belonging to long-dormant accounts, but we do not commit to a fixed timetable — to have your data erased at any time, use the in-app deletion feature or email us.

## 7. Your rights under GDPR

If you are in the EEA, UK or Switzerland you have the right to:

- **Access** — request a copy of the personal data we hold about you.
- **Rectification** — correct inaccurate data (you can edit most of it yourself in the app).
- **Erasure** ("right to be forgotten") — delete your data, primarily by using the in-app deletion feature.
- **Restriction** — ask us to limit how we process your data.
- **Portability** — receive your data in a machine-readable format. Consu lets you export your full library from **Settings → Your data → Export → Consu backup** as a JSON file, free and with no account requirement. A spreadsheet-friendly CSV export is also offered as part of Pro; this is a convenience format only, and it does not affect your right to obtain your data free of charge through the JSON export or by emailing us.
- **Objection** — object to processing based on legitimate interests, including crash diagnostics and analytics. You can exercise this directly in the app under **Settings → Privacy and safety**.
- **Withdraw consent** — where processing is based on consent.
- **Lodge a complaint** with the Irish Data Protection Commission (https://www.dataprotection.ie) or your local EEA data-protection authority.

To exercise any of these rights, email **privacy@getconsu.com**. We will respond within one month.

## 8. How to delete your data

In the app: scroll to the bottom of **Settings**, tap **Delete account**, type `DELETE` and confirm. Deleting needs a connection: if Consu cannot reach our servers, nothing is deleted and the app says so. If your account is linked to Google or Apple, you may be asked to sign in again to confirm it is you. This removes, from our servers:

- your profile, friend code, privacy choices and Firebase Auth account;
- your library backup, all of its dated copies, and the list of posts you have hidden;
- the copies of your profile other people can read, including your web page;
- your follows and followers, in both directions;
- your posts, and the replies other people left on them;
- your notifications;
- the reactions and reply hearts you left;
- your profile photo;
- the people you have blocked;
- the titles you sent and the titles sent to you, and the notifications you sent and the replies you wrote, wherever they sit with the people you follow, the people who follow you and the people you sent titles to;
- your place in every Shared List and Together queue: you leave each one, your votes, "seen" marks and reactions come off every title in it, and your display name and account ID come off the titles you added.

The account record and the sign-in go last. If any step fails, the app lists what is still on our servers and offers to try again. For users who signed in with Apple, we also revoke the Apple sign-in token as part of deletion. If you never linked Google or Apple and your session is old, Firebase can refuse to delete the bare sign-in record (a random ID with nothing attached to it) once everything else is gone; the app then clears your phone and signs you out at once, and our monthly clean-up removes the record. The same clean-up removes, within a month, the notifications and replies you sent to someone you no longer followed and who no longer followed you, the titles you sent them with an earlier version of the app, and your customer record at RevenueCat (section 4.5).

**On your phone.** Deleting your account also removes everything Consu keeps on the phone you delete it from: your library, the app's copies of what it looked up and read from our database, the files it saved in its own folder (exports, calendar files and the images it drew for you to share) and your settings, except your crash-report and analytics choices. The app then starts again as a new guest, at the first-run screens.

**What may survive in someone else's account, and how to have it removed.** Some things you create are, by design, records held by other people:

- A **Shared List** or **Together queue** belongs to all of its members. After you delete your account, the titles you added stay with the other members, without your name or account ID, and a list you made passes to a member who stays; a list or queue is deleted when its last member leaves. Before you delete your account you can remove titles you added (on a Together queue, with **Remove** on your own titles).
- **A title someone added from you.** If someone added a title you sent them, or one they found through you (from your post, your Right now or Upcoming titles, Explore or your profile), their library, and their backup, keep your display name and account ID against it.
- **Someone's block list.** If someone blocked you, their block list, and their backup, keep your account ID, display name and avatar or photo address, and their block record keeps your account ID and when they blocked you.
- **Reactions other people left on your posts and replies**, and notifications they received about your posts, are their records and stay with them; they refer to your account ID and the title (for a heart on a reply, the reply), not to your name.
- **Records made as a guest** stay under the guest ID if you later signed in to an account that already existed instead of linking (section 2.2); email us to have them removed.
- **Reports** made by you or about you are kept for two years from the report (section 6).
- **Purchase records held by Apple or Google** stay with the app store, under its own terms. Crash and analytics data are kept for the periods in section 6.

If anything of yours is still visible after deletion, or the in-app flow fails for any reason, email **privacy@getconsu.com** from the address linked to your account — or with your display name and friend code — and we will delete it manually.

## 9. Children

Consu is intended for users aged 13 and over and is not directed at children under 13. The age ratings shown on the Apple App Store and Google Play describe content suitability and are set through each store's own questionnaire; the minimum age for using Consu is the one stated in our Terms of Service.

In countries where the digital age of consent under GDPR is higher than 13 (Ireland: 16; Germany: 16; Netherlands: 16; Italy: 14; France: 15; etc.), users under that age must have the consent of a parent or legal guardian to use Consu. If we become aware that we have collected personal data from a child below the applicable age without parental consent, we will delete it.

Parents: to request deletion of a child's data, email **privacy@getconsu.com**.

## 10. Profile visibility — who else can see your data

What other people can see depends on the visibility setting you choose for your profile, and on the switches beside it, under **Social → Profile → Privacy**. Firestore and Firebase Storage enforce security rules for each kind of record. A guest who has not linked Google or Apple cannot set up a profile, publishes no part of their library and posts nothing (a display name set as a guest in an earlier version of Consu stays on its profile record, and 10.2 applies to it); what follows applies once you sign in and set up a profile.

### 10.1 The three settings

- **Public** — your profile is listed in Explore, which anyone using the app can browse, and anyone using the app can open it. It shows your display name and avatar and the parts of your library your switches allow (10.4). You also get a web page that anyone with its link can open without the app (10.6). Your mutuals see more, as under Mutuals.
- **Mutuals** — only people you follow who also follow you ("mutuals") can see your library, and they see all of it apart from titles you marked Dropped: every section whatever the section switches say, your hours and achievements, and your reviews if **Share my reviews** is on. You are not listed in Explore and you have no web page. People you connected with by friend code in earlier versions of Consu count as mutuals.
- **Private** — nothing is published: you are not listed in Explore, you have no web page and nobody can open your library. Consu makes no posts while you are Private and tells nobody when you take their picks, and nobody can read the posts you made before while you stay Private. The things in 10.2 stay visible to other Consu users, and 10.5 lists what else Private does not cover.

**A new profile starts as Private**, and nothing is published until you choose. When you set up your profile, Consu asks who sees your library (Public, Mutuals or Private, each with what it shows); if you close the question without answering, your profile stays Private. Every switch starts on. You can change the setting at any time. Other people's apps keep a copy of what they last read, so a change reaches them the next time their app reads your profile from our servers.

### 10.2 What other people can see whatever your setting

Some things can be read by other Consu users at every setting, because the social features need them:

- your display name, avatar or profile photo, friend code and Pro status, and when you joined;
- your visibility setting and the other choices in your Privacy sheet, including which categories you hide, and your profile colour and card frame (the titles of the posts you have hidden are not part of this: see 10.3);
- who you follow and who follows you, and how many;
- your monthly board numbers, while **The monthly board** is on and your profile is Public or Mutuals (10.4).

Searching your exact friend code finds you at any setting. A Private profile then shows its name, avatar and counts, with a note that it is private.

### 10.3 Your posts, the Feed and Right now

When you finish something, and when you start something if **Post when I start** is on, Consu writes a post: the title, its cover, category and genres, the platform or service you used, your score (and your earlier score, when you finish something again), the days you started and finished, how long it took, how many times you have finished it, and your review if **Share my reviews** is on. Your mutuals see your posts in their Feed and can react and reply. People who follow you without being followed back see stories built from your public profile instead, while it is Public; they cannot react to them.

- No post is made while your profile is Private, for a title in a category you hide, or for a title whose post you have hidden. What Consu holds back this way is listed under **Hidden posts** in your Privacy sheet with the reason (for example "Not posted · you were Private"), and it is not posted later: when you make your profile visible again, your profile tells your mutuals' apps not to show those titles as new posts. Your next real post about one of them is made as usual.
- To keep a post out of other people's feeds, tap the ⋯ on your post and choose **Hide this post**. This hides every post you have made about that title, stops new ones, and takes the title off Right now and Upcoming. The posts already made stay in your activity history, where your mutuals' accounts can still read them, and the app hides them: your mutuals' copy of your profile names every title whose post you hid, and your public profile names only those it already shows. **Hidden posts** in your Privacy sheet lists them, each with **Show again**.
- Choosing Private does not delete your posts: they stay in your activity history, unreadable to anyone else until your profile is Public or Mutuals again. Hiding a category deletes the posts you made in it (10.4). Other changes to a switch or your visibility do not withdraw posts already made. Posts stay in your activity history until you delete your account.

Your current titles appear on **Right now** with how far through you are (for example "S2 · E7") and the day you last moved them; titles on your Upcoming shelf appear in your people's **Upcoming** row with their release dates; and a title's page shows which of your mutuals have it, on which shelf and with what score. Your mutuals see these while your profile is Public or Mutuals; at Private, Right now, Upcoming and a title's page show nothing of yours. Right now shows your titles only while **Post when I start** is on. People who follow you without being a mutual see your Right now and Upcoming titles through your public profile, while it is Public and the Current and Backlog switches are on.

### 10.4 The switches

At Public, these seven switches show or hide parts of your profile: **Top rated**, **Current**, **Backlog**, **Taste DNA**, **Completed count** (which shows or hides your whole list of finished titles, not only the count), **Hours**, and **Achievements & streak**. They govern what people who are not your mutuals can see. **Mutuals see your full library regardless of them** — that is what choosing the Mutuals tier means.

The other switches shape what you share beyond your profile. **Post when I start**, **Share my reviews** and **Tell people when I take their picks** (10.5) apply to your posts; reviews reach only your mutuals, never your public profile, Explore or the web. **The monthly board** puts your month's finishes, their covers and your hours on the leaderboards, as far as your **Completed count** and **Hours** switches allow (those two still apply to the board's counts and hours at Mutuals, where the sheet does not show them; the covers your mutuals see there come from your posts): the Everyone board lists Public profiles, and the Friends board shows your mutuals. **On the web** (Public only) controls your web page (10.6). At Mutuals the Privacy sheet shows only these switches, apart from On the web, with your hidden posts and Hidden categories; at Private, where nothing is published or posted, it shows only your hidden posts.

While your profile is visible, a few things are not covered by any switch: your favourites (the five you pick), your highest-rated finished title in each medium, or the one you pinned for it in an earlier version (shown as your favourites if you have not picked any), how many titles you have in each medium (all shelves together), your last-active time, and, on each title shown, its genres and runtime, your score, earlier score and dates, how many times you have finished it, how far through it you are, and your favourite character in it.

**Hidden categories** hides a medium from your profile at every setting, mutuals included: those titles are removed before your profile is written out, so they never leave your device as part of it. No posts are made for titles in that medium and nobody is told when you take their picks in it (10.5), and when you hide a medium, the app deletes the posts you had already made in it. Showing the medium again does not bring those posts back.

### 10.5 Things your visibility setting does not cover

Setting your profile to Private does not retract these, so they are worth knowing about:

- **Shared Lists and Together queues.** These are joint by nature. The other members can always see the list, its members and the titles you added; on a Shared List also your display name against them, and your votes, reactions and "seen" marks. You can remove titles you added (on a Together queue, with **Remove** on your own titles) and undo your votes. **Leave this list** or **Leave this queue** takes you, your votes, your "seen" marks and your reactions off it; the titles you added stay for the other members with your name, a list you made passes to a member who stays, and the last member to leave deletes it. Deleting your account leaves every list and queue the same way and also takes your name off the titles you added (section 8). New Shared Lists cannot be made in this version.
- **Titles you send.** Sending someone a title shows them the title, your name and avatar, your note and your score for it. It is stored in its own record, which only you and the recipient can read. Until a later version, a copy without your note is also stored with the recipient's posts, so that someone still on an earlier version of the app receives it; the accounts of the recipient's mutuals can read that copy.
- **Picks you take.** When you add a title someone sent you, they are told (after a short undo window); when you finish it, they are told with your score. **Tell people when I take their picks** turns this off, and nobody is told while your profile is Private or for a title in a category you hide.
- **Replies and reactions.** A reply is stored with the post it answers, under your display name and avatar, and can be read by the post's owner and their mutuals. The post's owner is notified with its opening words, and so are the person you answer and anyone you @name, when they are your mutuals. You can react only to your mutuals' posts. Reactions are stored with your account ID, the time, the post's owner and its title, and can be read by other Consu users; the post's owner is notified when you are their mutual. A heart on a reply is stored the same way with the reply and its author in place of the post, and the reply's author is notified, with its opening words, when you are their mutual.
- **Reports.** If you report a profile, a review or a reply, we store who reported, who was reported, the reason you chose and, for a review or a reply, a copy of its text and the title it is about. Only we can read reports.

Separately, you can **block** another user from their profile's ⋯ menu, and review or undo that under **Settings → Privacy and safety → Blocked people**. Blocking ends both follows, so neither of you follows the other, and they cannot follow you again, react to or reply on your posts, send you titles or notify you while the block stands. Their profile, posts, reactions and board place are hidden from you. If your profile is Public, they can still open it, as anyone can. **Hide** in Explore hides a person from your own Explore and name search only (their exact friend code still finds them). Your block list, with each person's account ID, display name and avatar, and your hide list of account IDs are kept on your phone and in your own backup. Each block is also recorded in our database (their account ID and when), readable only by you, so that our security rules can refuse those actions.

### 10.6 Your web page

While your profile is Public and **On the web** is on (it is on unless you turn it off), getconsu.com/u/ followed by your friend code shows your profile to anyone with the link, no account needed. The page shows your name, avatar or photo, profile colour, Pro badge, friend code, when you joined, your follower count, your favourites and how many titles you have in each medium, and the parts your switches allow: covers from your library, how many titles you have finished and your average score, your hours and streak, your recent finishes with your scores, what you are on now, and your genres and how you score. A link to it pasted into a chat app previews your name, how many titles you have finished, your average score and your first three favourites (or your top three genres).

The page asks search engines not to list it, but your friend code is part of your Explore entry, which anyone using the app can read. Turning off On the web, or leaving Public, removes the page within about two minutes. Consu tells you about the page when you choose Public (the choice names it, or a notice on the Social tab does, with the choice to turn it off), and **On the web** turns it off at any time.

## 11. Security

- All traffic between the app and any external service — Firebase, the Cloudflare Worker, and the services named in section 4 — is encrypted with TLS.
- Firestore and Firebase Storage enforce security rules on every read and write. Your backup can be read only by your own account; section 10 explains what other people can read.
- A profile photo is stored at an unguessable address that works without signing in, so anyone who has that address can open the photo. The address is part of your profile (section 10.2). Any Consu account that knows your account ID can also open the photo.
- Your password is never handled by Consu — authentication is delegated to Google or Apple.

No system is perfectly secure. If you believe your account has been compromised, contact **privacy@getconsu.com** and change your linked Google or Apple account password immediately.

## 12. Changes to this policy

We may update this Privacy Policy to reflect changes to the app, legal requirements, or sub-processors. The "Last updated" date at the top of this document indicates when the most recent change was made. Material changes will be announced in the app before they take effect.

**Earlier versions of the app.** This policy describes Consu 4.0.1. A phone still running an earlier version, yours or someone else's, behaves as that version did until it updates. On a second phone of yours it can still post about titles in a category you hide, and publish your profile without your hidden posts, so they show again in your mutuals' feeds until your updated phone next opens Consu. On other people's phones it can still let people who follow you without being followed back react to your posts, and someone on an earlier version who sends you a title stores their note with the copy beside your posts. Our security rules apply to every version: nobody else can read your posts while your profile is Private, and once your phone runs this version, nobody you have blocked can follow you, react to or reply on your posts, or send you titles.

## 13. Contact

For any privacy-related question, request or complaint:

**Karl Holmes** — privacy@getconsu.com
