# authorship-tag-generator
A lightweight, offline, open-source tool for generating authorship tags in printed educational documents.

## Overview

The *Authorship Tag Generator* is a simple browser-based tool that allows instructors or educational professionals to generate short, human-readable codes (tags) for printed documents such as exams, handouts, or forms.

Each code is deterministically generated from:
- a manually entered date (`ddmmyy` format)
- a secret 6-character string known only to the document's creator

This approach ensures that each printed page can be uniquely tied to its origin, providing lightweight authorship verification and document integrity — without any need for online infrastructure.

---

## Features

- Fully offline: runs locally in any modern browser
- No installation, servers, or plugins required
- Transparent SHA-256 hashing mechanism
- Base88 encoding for compact, typable output
- Human-readable 9-character code (formatted as three 3-character groups separated by spaces)
- Suitable for exams, assignments, handouts, participation logs, and more
- Open-source (MIT license — free software)

---

## Usage Instructions

1. Open `authorship-tag-generator.html` in any web browser (even offline).
2. Enter the **date** manually in `ddmmyy` format (e.g., `080425` for April 8, 2025).
3. Enter a **secret string** of exactly 6 characters.

4. Allowed characters for the secret string:  
   A-Z, a-z, 0-9, and symbols:  
   `! @ # $ % ^ & * ( ) _ + - = [ ] { } | ; : , . < > ?`

5. Click **Generate Tag** to create your unique authorship tag.

---

## Example

| Input         | Value    |
|---------------|----------|
| Date          | 080425   |
| Secret String | #test!   |
| Generated Tag | H7W lP2 bwM |

*Note*: The output is always 9 characters long, displayed as three blocks of 3 characters separated by spaces for readability.

---

## Why Use This?

- Easy to implement in resource-limited settings
- Avoids the overhead of QR codes or digital certificates
- Prevents unauthorized substitution or alteration of printed materials
- Enhances educational integrity in paper-based workflows
- Can be used to introduce students to basic cryptographic concepts

---

## License

This project is licensed under the [MIT License](./LICENSE).  
The MIT License is a permissive free software license, allowing users to freely use, modify, and distribute the software, including in commercial and closed-source projects, provided that the original license terms and copyright notice are preserved.

---

## Repository

Available at: https://github.com/ericblindgren/authorship-tag-generator

---

## Contributions

Contributions, suggestions, and improvements are welcome!
