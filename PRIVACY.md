# Privacy Policy

**Last updated: 24 April 2026**

This Privacy Policy explains how Consu ("the app", "we", "our") collects, uses,
and protects personal data when you use the Consu mobile application.

## 1. Who we are (data controller)

Consu is developed and operated by:

**Karl Holmes**, sole developer (personal capacity)
Based in Ireland
Contact: **karlballina@gmail.com**

For the purposes of the EU General Data Protection Regulation (GDPR) and the
Irish Data Protection Act 2018, Karl Holmes is the data controller for the
personal data processed through Consu.

## 2. What we collect

Consu is designed to minimise data collection. The following is the full list of
information we or our sub-processors handle:

### 2.1 Information you provide directly

- **Media library data** — the films, TV shows, games, books and music you add
  to your library, along with any ratings, notes, tags, pinned items, custom
  lists, completion dates and parental-control settings you create.
- **Profile information** — a display name, friend code, and optional custom
  avatar image you choose yourself.
- **Social data** — the friend codes of other Consu users you connect with,
  shared lists you create or join, and recommendations you send or receive.
- **Account linking data** (optional) — if you choose to link your account to a
  Google or Apple sign-in provider, we receive the email address associated
  with that provider to identify your account across devices.

### 2.2 Information created automatically

- **Anonymous user ID (UID)** — when you first open the app, Firebase
  Authentication assigns you a random anonymous UID. This UID is used to
  associate your cloud-synced data with your device. It is not linked to any
  personally identifying information unless you choose to link a Google or
  Apple account.
- **Device-local preferences** — theme, accent colour, zoom settings, completed
  tutorials and similar UI state are stored on your device.

### 2.3 Information we do NOT collect

- We do not use analytics SDKs (Google Analytics for Firebase, Crashlytics,
  Mixpanel, Segment, or similar) in this version of Consu.
- We do not use advertising networks or serve ads.
- We do not collect location data.
- We do not access your contacts, phone, camera roll (except when you
  explicitly pick an image for your custom avatar), SMS, call log or microphone.
- We do not sell data to third parties. We do not share data with advertisers.

## 3. Why we process your data (purposes and legal basis)

| Purpose | Legal basis (GDPR Article 6) |
|---|---|
| Provide the core app functionality (library, stats, social) | Contract (6(1)(b)) |
| Cloud backup and cross-device sync via Firebase | Contract (6(1)(b)) |
| Connect you with friends you choose to add | Contract (6(1)(b)) |
| Process one-time Pro upgrade payments | Contract (6(1)(b)) |
| Prevent abuse and secure the service | Legitimate interest (6(1)(f)) |
| Comply with legal obligations (e.g. tax records for sales) | Legal obligation (6(1)(c)) |

We do not rely on consent as the primary legal basis for the processing above,
because the processing is necessary to provide the service you requested. You
can stop all processing at any time by deleting your account (see section 8).

## 4. Third-party services and data transfers

Consu uses the following sub-processors. Each has their own privacy policy
governing how they handle data.

### 4.1 Firebase (Google Ireland Limited / Google LLC)

Used for:

- **Firebase Authentication** — anonymous UIDs and, if you link your account,
  Google or Apple sign-in.
- **Firestore** — cloud backup of your library and profile, friend graph,
  activity feed, shared lists.
- **Firebase Storage** — custom avatar images (Pro feature).

Data is processed in Google's data centres. Consu's Firestore instance is
hosted in the **`europe-west2` (London, United Kingdom)** region. Some core
Firebase Authentication services are operated from Google's global
infrastructure, including servers in the United States; transfers outside the
European Economic Area (EEA) are covered by the EU Standard Contractual Clauses
in Google's Data Processing Addendum.

Policy: https://firebase.google.com/support/privacy

### 4.2 Cloudflare Worker (Cloudflare, Inc.) — metadata proxy

Consu fetches media metadata (posters, descriptions, ratings) through a
Cloudflare Worker that proxies requests to the third-party APIs listed in 4.3
below. The Worker:

- Does not receive your Firebase UID, email, display name, or library contents.
- Receives only the media title, ID, or search term you are looking up, plus
  standard HTTP request metadata (your IP address, user-agent, `Accept`
  headers) that Cloudflare requires to route the request.
- Uses your IP address solely for short-term rate limiting (a rolling 60-second
  window) to prevent abuse. IP addresses are not persisted to long-term storage
  by the Worker itself.
- Caches responses at Cloudflare's edge for up to 7 days to reduce load on the
  upstream APIs.

Cloudflare, acting as an independent processor, may log request metadata in
accordance with its own privacy policy.

Policy: https://www.cloudflare.com/privacypolicy/

### 4.3 Third-party metadata providers

Consu displays metadata sourced from the following services. Each receives
only the query (e.g. a film title or ISBN) necessary to return a result,
proxied via the Cloudflare Worker described above. None of them receive your
Firebase UID, email, or library contents.

| Service | Purpose | Privacy policy |
|---|---|---|
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

This product uses the TMDB API but is not endorsed or certified by TMDB.
Similarly, Consu is not affiliated with or endorsed by any of the other
metadata providers listed.

### 4.4 Google Play Billing (Google Ireland Limited)

If you purchase Consu Pro, the payment is processed by Google Play Billing.
Consu never sees your card details.

Policy: https://policies.google.com/privacy

### 4.5 RevenueCat (RevenueCat, Inc.)

If you purchase Consu Pro, RevenueCat acts as the purchase-validation layer
between Google Play Billing and Consu. RevenueCat receives your anonymous
Firebase UID (to associate the purchase with your account) and the standard
purchase receipt from Google. RevenueCat does not receive your name, email, or
library contents.

Policy: https://www.revenuecat.com/privacy

## 5. Where your data is stored

- Data stored on your device stays on your device.
- Data synced to Firestore and Firebase Storage is hosted in the
  **`europe-west2` (London, United Kingdom)** region.
- Transfers to Google's US infrastructure for core authentication services are
  covered by the EU Standard Contractual Clauses.
- Cloudflare Worker requests are routed through Cloudflare's global edge
  network.

## 6. How long we keep your data

- While your account is active, we retain your library and profile indefinitely.
- When you delete your account (Settings → Account → Delete Account), your
  Firestore data and Firebase Storage files are deleted immediately. Any
  backups or logs containing personal data are deleted within 30 days.
- If you simply uninstall the app without deleting the account, your Firestore
  data remains until you delete the account or **24 months of inactivity**
  elapse, whichever comes first.

## 7. Your rights under GDPR

If you are in the EEA, UK or Switzerland you have the right to:

- **Access** — request a copy of the personal data we hold about you.
- **Rectification** — correct inaccurate data (you can edit most of it yourself
  in the app).
- **Erasure** ("right to be forgotten") — delete your data, primarily by using
  the in-app deletion feature.
- **Restriction** — ask us to limit how we process your data.
- **Portability** — receive your data in a machine-readable format. Consu lets
  you export your full library to CSV from Settings (Pro feature; available
  free on request).
- **Objection** — object to processing based on legitimate interests.
- **Withdraw consent** — where processing is based on consent.
- **Lodge a complaint** with the Irish Data Protection Commission
  (https://www.dataprotection.ie) or your local EEA data-protection authority.

To exercise any of these rights, email **karlballina@gmail.com**. We will
respond within one month.

## 8. How to delete your data

In the app: **Settings → Account → Delete Account**, type `DELETE`, confirm.
This removes your profile, library, friend connections, shared lists, feed
activity, custom avatar and Firebase Auth account.

If the in-app flow fails for any reason, email **karlballina@gmail.com** with
the Firebase UID visible in Settings → About, and we will delete your data
manually.

## 9. Children

Consu is rated 13+ on Google Play and is not directed at children under 13.

In countries where the digital age of consent under GDPR is higher than 13
(Ireland: 16; Germany: 16; Netherlands: 16; Italy: 14; France: 15; etc.), users
under that age must have the consent of a parent or legal guardian to use
Consu. If we become aware that we have collected personal data from a child
below the applicable age without parental consent, we will delete it.

Parents: to request deletion of a child's data, email
**karlballina@gmail.com**.

## 10. Security

- All traffic between the app and Firebase / Cloudflare is encrypted with TLS.
- Firebase Storage and Firestore enforce per-user security rules so that only
  the account owner and their chosen friends can read relevant data.
- Your password is never handled by Consu — authentication is delegated to
  Google or Apple.

No system is perfectly secure. If you believe your account has been
compromised, contact **karlballina@gmail.com** and change your linked Google
or Apple account password immediately.

## 11. Changes to this policy

We may update this Privacy Policy to reflect changes to the app, legal
requirements, or sub-processors. The "Last updated" date at the top of this
document indicates when the most recent change was made. Material changes will
be announced in the app before they take effect.

## 12. Contact

For any privacy-related question, request or complaint:

**Karl Holmes** — karlballina@gmail.com
