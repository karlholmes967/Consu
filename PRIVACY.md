# Consu Privacy Policy

**Last updated: 1 July 2026**

This Privacy Policy explains how Consu ("the app", "we", "our") collects, uses, and protects personal data when you use the Consu mobile application.

## 1. Who we are (data controller)

Consu is developed and operated by:

**Karl Holmes**, sole developer (personal capacity). Based in Ireland. Contact: **karlballina@gmail.com**

For the purposes of the EU General Data Protection Regulation (GDPR) and the Irish Data Protection Act 2018, Karl Holmes is the data controller for the personal data processed through Consu.

## 2. What we collect

Consu is designed to minimise data collection. The following is the full list of information we or our sub-processors handle:

### 2.1 Information you provide directly

- **Media library data** — the films, TV shows, games, books and music you add to your library, along with any ratings, notes, tags, pinned items, custom lists, completion dates and parental-control settings you create.
- **Profile information** — a display name, friend code, and optional custom avatar image you choose yourself.
- **Social data** — the friend codes of other Consu users you connect with, shared lists you create or join, and recommendations you send or receive. You control how much of your profile is visible to other people through the Public / Friends / Private setting (see section 10).
- **Account linking data** (optional) — if you choose to link your account to a Google or Apple sign-in provider, we receive the email address associated with that provider to identify your account across devices. If you use Sign in with Apple and choose "Hide My Email," we receive only Apple's anonymised relay address, not your real email.

### 2.2 Information created automatically

- **Anonymous user ID (UID)** — when you first open the app, Firebase Authentication assigns you a random anonymous UID. This UID is used to associate your cloud-synced data with your device. It is not linked to any personally identifying information unless you choose to link a Google or Apple account.
- **Device-local preferences** — theme, accent colour, zoom settings, completed tutorials and similar UI state are stored on your device.
- **App-integrity checks** — Consu uses Firebase App Check (Play Integrity on Android, App Attest on iOS) to confirm that requests come from a genuine, untampered copy of the app. This produces a short-lived device-integrity token used only to protect the service from abuse; it does not identify you personally.
- **Crash diagnostics** — when the app crashes, Firebase Crashlytics records the crash stack trace, the operating system version, the device model, the app version, and the breadcrumbs of the most recent in-app actions. This data is automatically generated and does not include the contents of your library or personal messages. You can opt out under **Settings → Diagnostics → Send crash reports**.
- **Usage analytics** — Firebase Analytics records a small set of funnel events (first app open, onboarding completion, first item added, first rating, Pro purchase, account deletion). The events themselves carry no library content, names, or messages. Firebase also automatically logs technical events such as screen views and an approximate country derived from your IP address. You can opt out under **Settings → Diagnostics**.

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

We do not rely on consent as the primary legal basis for the processing above, because the processing is necessary to provide the service you requested or is based on our legitimate interests where the data is minimised and the impact on you is low. You can stop all processing at any time by deleting your account (see section 9). You can opt out of crash diagnostics and analytics under **Settings → Diagnostics**.

## 4. Third-party services and data transfers

Consu uses the following sub-processors. Each has their own privacy policy governing how they handle data.

### 4.1 Firebase (Google Ireland Limited / Google LLC)

Used for:

- **Firebase Authentication** — anonymous UIDs and, if you link your account, Google or Apple sign-in.
- **Firestore** — cloud backup of your library and profile, friend graph, activity feed, shared lists.
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

- Six custom events: `install`, `onboarding_complete`, `first_add`, `first_rate`, `pro_purchase`, `account_deletion`. Event names only — no parameters carrying content.
- Auto-collected events such as `screen_view`, `app_open`, and `first_open`.
- An approximate country derived from your IP address. The IP itself is not retained.
- A randomly generated app-instance identifier used to deduplicate sessions.

Analytics does not receive your library contents, friend codes, display name, email, or any in-app messages. Analytics data is retained by Google for up to 14 months (Firebase's default retention) and then deleted. You can opt out under **Settings → Diagnostics**.

Policy: https://firebase.google.com/support/privacy

### 4.2 Cloudflare Worker (Cloudflare, Inc.) — metadata proxy

Consu fetches media metadata (posters, descriptions, ratings) through a Cloudflare Worker that proxies requests to the third-party APIs listed in 4.3 below. The Worker:

- Does not receive your Firebase UID, email, display name, or library contents.
- Receives only the media title, ID, or search term you are looking up, plus standard HTTP request metadata (your IP address, user-agent, `Accept` headers) that Cloudflare requires to route the request.
- Uses your IP address solely for short-term rate limiting (a rolling 60-second window) to prevent abuse. IP addresses are not persisted to long-term storage by the Worker itself.
- Caches responses at Cloudflare's edge for up to 7 days to reduce load on the upstream APIs.

Cloudflare, acting as an independent processor, may log request metadata in accordance with its own privacy policy.

Policy: https://www.cloudflare.com/privacypolicy/

### 4.3 Third-party metadata providers

Consu displays metadata sourced from the following services. Each receives only the query (e.g. a film title or ISBN) necessary to return a result, proxied via the Cloudflare Worker described above. None of them receive your Firebase UID, email, or library contents.

| Service | Purpose | Privacy policy |
|---------|---------|---|
| **TMDB** (The Movie Database) | Film and TV metadata, posters | https://www.themoviedb.org/privacy-policy |
| **OMDB** | Supplementary film metadata (IMDb ratings, runtimes) | https://www.omdbapi.com/ |
| **RAWG** | Video-game metadata, screenshots | https://rawg.io/privacy_policy |
| **Steam** (Valve) | Video-game store data | https://store.steampowered.com/privacy_agreement/ |
| **Google Books** | Book metadata, covers | https://policies.google.com/privacy |
| **Open Library** | Supplementary book metadata | https://openlibrary.org/about/privacy |
| **New York Times Books API** | Bestseller lists | https://www.nytimes.com/privacy/privacy-policy |
| **Deezer** | Music track and album metadata | https://www.deezer.com/legal/personal-datas |
| **MusicBrainz** | Open-source music database | https://metabrainz.org/privacy |
| **Cover Art Archive** | Album artwork | https://metabrainz.org/privacy |
| **Apple iTunes Search API** | Music and podcast metadata | https://www.apple.com/legal/privacy/ |

This product uses the TMDB API but is not endorsed or certified by TMDB. Similarly, Consu is not affiliated with or endorsed by any of the other metadata providers listed.

### 4.4 App-store billing (Apple / Google)

If you purchase Consu Pro, the payment is processed by the app store you bought it through — the **Apple App Store** (Apple Distribution International Ltd.) on iOS, or **Google Play Billing** (Google Ireland Limited) on Android. Consu never sees your card details.

Policies: https://www.apple.com/legal/privacy/ · https://policies.google.com/privacy

### 4.5 RevenueCat (RevenueCat, Inc.)

If you purchase Consu Pro, RevenueCat acts as the purchase-validation layer between the app store (Apple App Store or Google Play) and Consu. RevenueCat receives your anonymous Firebase UID (to associate the purchase with your account) and the standard purchase receipt from Apple or Google. RevenueCat does not receive your name, email, or library contents.

Policy: https://www.revenuecat.com/privacy

## 5. Where your data is stored

- Data stored on your device stays on your device.
- Data synced to Firestore and Firebase Storage is hosted in the **`europe-west2` (London, United Kingdom)** region.
- Transfers to Google's US infrastructure for core authentication, Crashlytics, and Analytics services are covered by the EU Standard Contractual Clauses.
- Cloudflare Worker requests are routed through Cloudflare's global edge network.

## 6. How long we keep your data

- While your account is active, we retain your library and profile so that it stays available across your devices.
- When you delete your account (Settings → Account → Delete Account), your Firestore data and Firebase Storage files are deleted immediately. Any backups or logs containing personal data are deleted within 30 days.
- Crash reports captured by Crashlytics are retained by Google for up to 90 days and then deleted automatically.
- Analytics events are retained by Google for up to 14 months and then deleted automatically.
- If you simply uninstall the app without deleting your account, your Firestore data remains stored so you can restore it if you reinstall and sign back in. It stays until you delete your account. We may remove data belonging to long-dormant accounts, but we do not commit to a fixed timetable — to have your data erased at any time, use the in-app deletion feature or email us.

## 7. Your rights under GDPR

If you are in the EEA, UK or Switzerland you have the right to:

- **Access** — request a copy of the personal data we hold about you.
- **Rectification** — correct inaccurate data (you can edit most of it yourself in the app).
- **Erasure** ("right to be forgotten") — delete your data, primarily by using the in-app deletion feature.
- **Restriction** — ask us to limit how we process your data.
- **Portability** — receive your data in a machine-readable format. Consu lets you export your full library to CSV from Settings (Pro feature; available free on request).
- **Objection** — object to processing based on legitimate interests, including crash diagnostics and analytics. You can exercise this directly in the app under **Settings → Diagnostics**.
- **Withdraw consent** — where processing is based on consent.
- **Lodge a complaint** with the Irish Data Protection Commission (https://www.dataprotection.ie) or your local EEA data-protection authority.

To exercise any of these rights, email **karlballina@gmail.com**. We will respond within one month.

## 8. How to delete your data

In the app: **Settings → Account → Delete Account**, type `DELETE`, confirm. This removes your profile, library, ratings, friend connections, follow graph, shared lists, feed activity, notifications, custom avatar and Firebase Auth account. For users who signed in with Apple, we also revoke the Apple sign-in token as part of deletion.

If the in-app flow fails for any reason, email **karlballina@gmail.com** with the Firebase UID visible in Settings → About, and we will delete your data manually.

## 9. Children

Consu is intended for users aged 13 and over, is age-rated accordingly on the Apple App Store and Google Play, and is not directed at children under 13.

In countries where the digital age of consent under GDPR is higher than 13 (Ireland: 16; Germany: 16; Netherlands: 16; Italy: 14; France: 15; etc.), users under that age must have the consent of a parent or legal guardian to use Consu. If we become aware that we have collected personal data from a child below the applicable age without parental consent, we will delete it.

Parents: to request deletion of a child's data, email **karlballina@gmail.com**.

## 10. Profile visibility — who else can see your data

Firebase Storage and Firestore enforce per-user security rules. What other people can see depends on the visibility setting you choose for your profile:

- **Private** — no other user can read your library or profile.
- **Friends** — only people whose friend request you have accepted can see your full library and profile.
- **Public** — your display name, avatar and a snapshot of your library are visible to other Consu users, including through the in-app Explore surface. Public-profile data is readable by anyone using the app.

You can change this setting at any time in the app, and you can choose which sections (for example your taste stats or current activity) are included.

## 11. Security

- All traffic between the app and Firebase / Cloudflare is encrypted with TLS.
- Firestore and Firebase Storage enforce per-user security rules so that data is only readable in line with your chosen visibility setting (see section 10).
- Your password is never handled by Consu — authentication is delegated to Google or Apple.

No system is perfectly secure. If you believe your account has been compromised, contact **karlballina@gmail.com** and change your linked Google or Apple account password immediately.

## 12. Changes to this policy

We may update this Privacy Policy to reflect changes to the app, legal requirements, or sub-processors. The "Last updated" date at the top of this document indicates when the most recent change was made. Material changes will be announced in the app before they take effect.

## 13. Contact

For any privacy-related question, request or complaint:

**Karl Holmes** — karlballina@gmail.com
