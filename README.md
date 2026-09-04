# Global E.164 Telecommunications Registry & Dialing Directory

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Standards: ITU-T E.164](https://img.shields.io/badge/Standard-ITU--T%20E.164-blue)](https://www.itu.int/)
[![Website](https://img.shields.io/badge/Registry-prefixyr.com-00f5d4)](https://prefixyr.com)

An authoritative open-source reference and normalization database for international dialing prefixes, regional area codes (NPA), and exchange routing data. Designed for global communications platforms, SMS gateways, and VoIP architecture.

---

## 🌐 Overview

Phone number normalization is critical for database integrity, SMS delivery, and SIP routing. **Prefixyr** provides structured mapping according to the **ITU-T Recommendation E.164** standard.

### Core Features
- **E.164 Formatting Rules:** Standardize local phone numbers into global format (`+[CountryCode][NationalDestinationCode][SubscriberNumber]`).
- **Trunk Prefix Handling:** Automated rules for stripping national trunk prefixes (e.g., dropping `0` in the UK, AU, and IN).
- **NANP & Regional Data:** Coverage of North American Numbering Plan allocations, UK area codes, Australian mobile series, and Indian STD prefixes.

---

## 📐 E.164 Quick Reference Table

| Country | Country Code | Trunk Prefix | Local Example | Normalized E.164 |
| :--- | :--- | :--- | :--- | :--- |
| **United States** | `+1` | None | `(212) 555-0199` | `+12125550199` |
| **United Kingdom** | `+44` | `0` | `020 7946 0111` | `+442079460111` |
| **Australia** | `+61` | `0` | `(02) 5550 1234` | `+61255501234` |
| **India** | `+91` | `0` | `022 2345 6789` | `+912223456789` |

---

## ⚙️ Quick Usage (Regex Examples)

### Basic E.164 Validation Regex
Validates international E.164 format (1 to 15 digits overall, excluding the leading `+`):
```regex
^\+[1-9]\d{1,14}$

🔗 Official Registry & Resources
For full destination code indexes, active carrier ranges, and routing data updates:

Official Registry: prefixyr.com

Standard Documentation: ITU-T Recommendation E.164

📄 License
This repository and reference documentation are licensed under the MIT License.
