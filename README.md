# TAC Database

> Complete TAC (Type Allocation Code) database for mobile devices up to December 2025. Useful for IMEI lookup, device fingerprinting, and telecom applications.

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
├── tac_full.xlsx
├── LICENSE
└── README.md
```

---

## Data Schema

| Field | Type | Description |
|---|---|---|
| `brand` | `string` | Device manufacturer / brand name (e.g. XIAOMI, SAMSUNG, APPLE, POCO) |
| `tac` | `string` | 8-digit Type Allocation Code |
| `specs` | `string` | Full model name, internal model number, variant, and release year |

---

## Usage

### CSV Lookup (manual)

Open `tac_full.xlsx` and search for a TAC number or device model directly.

---

## Coverage

- ✅ **Total TAC entries:** 254,997
- ✅ **Brands covered:** Xiaomi, Samsung, Apple, Huawei, More
- ✅ **Release years:** 2000 – 2025
- ✅ **Format:** XLSX (with per-brand sheets)

---

## Data Sources

TAC data is sourced and cross-referenced from:

- Public IMEI databases
- [Osmocom TAC](http://tacdb.osmocom.org/)
- [ Is this Phone Blocked?](https://isthisphoneblocked.net.au/)
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
