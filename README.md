# TAC Database

> Complete TAC (Type Allocation Code) database for mobile devices up to October 2026. Useful for IMEI lookup, device fingerprinting, and telecom applications.

---

## What is a TAC?

A **Type Allocation Code (TAC)** is the first 8 digits of an IMEI number. It uniquely identifies the model and origin of a mobile device. TACs are assigned by the **GSMA** and are used globally for:

- Device identification and classification
- IMEI validation
- Network management
- Fraud detection and prevention

---

## Contents

```
tac-database/
├── tac_full.csv
├── tac_full.xlsx
├── LICENSE
└── README.md
```

`tac_full.xlsx` contains three sheets:

- `ALL` — the complete dataset (matches `tac_full.csv`)
- `Common` — curated subset of widely used devices
- `Not_Common` — less common, regional, and legacy devices

---

## Data Schema

| Field | Type | Description |
|---|---|---|
| `brand` | `string` | Device manufacturer / brand name (e.g. XIAOMI, SAMSUNG, APPLE, POCO) |
| `tac` | `string` | 8-digit Type Allocation Code |
| `specs` | `string` | Full model name, internal model number, variant, and release year |

---

## Usage

### CSV

`tac_full.csv` is a plain UTF-8 CSV with the columns `Brand`, `TAC`, and `SPECS`. Search it directly or load it into any spreadsheet or database tool.

### Excel

Open `tac_full.xlsx` and search for a TAC number or device model in the `ALL` sheet. Use the `Common` and `Not_Common` sheets when you only need the curated subset.

---

## Coverage

- ✅ **Total TAC entries:** 259,035
- ✅ **Brands covered:** 11,000+ (Xiaomi, Samsung, Apple, Huawei, and more)
- ✅ **Release years:** 2000 – 2026
- ✅ **Formats:** CSV and XLSX (`ALL`, `Common`, `Not_Common`)
- ✅ **Latest update:** October 2026 — 3,551 more TACs added across Apple, Realme, Vivo, Honor, Huawei, Motorola, ZTE, and more (4,033 new TACs this month)

---

## Data Sources

TAC data is sourced and cross-referenced from:

- Public IMEI databases
- [Osmocom TAC](http://tacdb.osmocom.org/)
- [Is This Phone Blocked?](https://isthisphoneblocked.net.au/)
- [Apple Support](https://support.apple.com/en-us/108044) and [GSMArena](https://www.gsmarena.com/) for model verification
- Community contributions and corrections

---

## Contributing

Contributions are welcome! If you spot a missing or incorrect TAC entry:

1. Fork the repository
2. Edit the relevant file
3. Submit a Pull Request with a short description of the change

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---
