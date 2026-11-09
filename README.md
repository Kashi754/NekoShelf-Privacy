# NekoShelf — Privacy Policy

**Effective Date:** November 8, 2026  
**Developer:** Kashi754  
**Application:** NekoShelf (`com.kashi754.nekoshelf`)

---

## Overview

**NekoShelf** is a personal manga collection, volume inventory, and reading progress tracker for Android. NekoShelf does **not** host, stream, or distribute manga chapters.

We respect your privacy. NekoShelf does **not** require user accounts, does **not** include analytics or advertising SDKs, and does **not** collect, sell, or transmit your personal information to any developer-operated server.

---

## 1. Data Stored Locally on Your Device

All personal library data you create in NekoShelf is stored exclusively on your device in a local SQLite database and Android DataStore preferences, including:

- Your custom libraries/collections and categories
- Series you add to your libraries or wishlist
- Owned/unowned volume selections and reading status (`Unread`, `Reading`, `Read`)
- Custom series titles, descriptions, star ratings, and cover image preferences
- App display preferences (e.g., Light/Dark/System theme and Grid/Title view mode)

### Backup & Export
NekoShelf allows you to manually export your library to a local `.json` backup file and import `.json` backup files using the Android system file picker. These files are saved only to the location you choose on your device.

---

## 2. Permissions We Request

### Camera (`android.permission.CAMERA`)
- **Purpose:** Used exclusively for the built-in ISBN barcode scanner so you can quickly look up and add physical manga volumes by scanning the barcode on the back cover.
- **How it is processed:** Camera frames are analyzed in real time **entirely on your device** using Google ML Kit Barcode Scanning. Camera images and video are **never** saved, recorded, or transmitted off your device.
- **Optional:** You can use NekoShelf without granting camera permission by searching for series by title or entering ISBN numbers manually.

### Internet (`android.permission.INTERNET`)
- **Purpose:** Used to fetch public manga series metadata, volume lists, publication dates, ISBN records, and cover art from third-party public APIs when you search for or refresh a series.

---

## 3. Third-Party Services & Public Data Sources

When you search for manga, scan an ISBN barcode, or view series details, the app makes direct HTTPS requests from your device to the following public APIs:

1. **MangaDex API (`https://api.mangadex.org` / `https://uploads.mangadex.org`)** — Used to search series metadata, descriptions, genre tags, community ratings, volume numbers, and cover art.
2. **Anime News Network Encyclopedia API (`https://cdn.animenewsnetwork.com/encyclopedia/api.xml`)** — Used to look up authoritative tankoubon volume counts, North American English release dates, ISBNs, and supplementary series summaries and cover art.
3. **Penguin Random House (`https://images.randomhouse.com`)** — Used to retrieve English edition cover art for PRH-distributed publishers (including Seven Seas Entertainment and Kodansha) by ISBN.
4. **English Wikipedia MediaWiki API (`https://en.wikipedia.org/w/api.php`)** — Used to look up English print volume release dates and ISBN records (content licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)).
5. **Apple Books / iTunes Search API (`https://itunes.apple.com/search`)** — Used to look up US English edition publication dates and English volume cover art.
6. **OpenLibrary Books API (`https://openlibrary.org/api/books`)** — Used to resolve scanned book ISBN barcodes to series titles and volume numbers (CC0 bibliographic data).
7. **Google Books API (`https://www.googleapis.com/books/v1/volumes`)** — Used as a fallback to resolve scanned book ISBN barcodes to series titles and volume numbers.

Standard network request metadata (such as your IP address and the search query or ISBN being looked up) is received by those third-party services in order to fulfill the request, subject to their respective privacy policies.

---

## 4. Children's Privacy

NekoShelf does not knowingly collect any personal information from children under the age of 13 (or the applicable age in your jurisdiction).

---

## 5. Data Retention & Deletion

Because all library data is stored locally on your device, you have full control over it at all times:
- You can delete individual series, categories, or libraries directly within the app.
- Clearing the app's storage in Android Settings or uninstalling NekoShelf permanently deletes all locally stored data from your device.

---

## 6. Changes to This Privacy Policy

If we update this Privacy Policy, we will post the revised version on this page and update the **Effective Date** above.

---

## 7. Contact

If you have any questions about this Privacy Policy or NekoShelf, please open an issue on this repository or contact the developer at **kashi754@gmail.com**.
