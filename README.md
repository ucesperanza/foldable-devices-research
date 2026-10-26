# foldable-devices-research
## TO BE UPDATED AS I GO

# Foldable Device App Reliability & RotDroid Testing Framework

## Current standing
This repository serves as the central evaluation suite for detecting and analyzing **GUI rotation bugs, cross-orientation state equivalence, and layout reliability failures** on foldable Android devices.

Our work integrates extensive empirical data collected across **300+ commercial and open-source applications** (from our core testbed and filtered dataset batches) with the **RotDroid** framework. Some stuff from previous testing will be added alongside new testing.

---

## 📂 Core Components & Repository Map
```text
foldable-rotdroid-testing/
│
├── .github/
│   └── workflows/
│       └── main.yml               # Automated CI/CD workflow configuration
│
├── apks/
│   └── README.md                  # Detailed guide on downloading APK batches via Releases
│
├── docs/
│   ├── app-inventory.md           # Comprehensive catalog of all tested apps, packages & batches
│   ├── setup-guide.md             # Android usage, ADB deployment & environment setup
│   └── rotdroid-integration.md    # ISSRE 2026 RotDroid, RotBench, & RotVL specifications
│
├── status/
│   └── email-status.md            # Communications log, stakeholder reports & Nov 2 milestone
│
├── .gitignore                     # Prevents large binary files (*.apk) from cluttering Git history
├── LICENSE                        # Open-source project license
└── README.md                      # Main repository landing page & executive summary
```


| Path / File | Description |
| **[`docs/app-inventory.md`](docs/app-inventory.md)** | Full app catalog listing package names, entry activities, and test statuses across all filtered datasets (`filtered_apks.csv` – `filtered_apks_4.csv` & `300APPSTESTING`). |
| **[`docs/setup-guide.md`](docs/setup-guide.md)** | Step-by-step user guide for installing APKs via ADB, configuring physical testbed devices, and maintaining environment consistency. |
| **[`docs/rotdroid-integration.md`](docs/rotdroid-integration.md)** | Replication documentation referencing the **RotDroid** source code, **RotBench** dataset, and **RotVL** models. |
| **[`status/email-status.md`](status/email-status.md)** | Log of email status reports, stakeholder communications, and our **November 2** progress summary. |
| **[`apks/README.md`](apks/README.md)** | Download guide for retrieving compiled `.apk` binary batches securely via GitHub Releases. |

---

## 📱 Evaluated Datasets & Categories
Our benchmark encompasses diverse application domains evaluated across both **book-style** (e.g., Samsung Galaxy Z Fold 4, Google Pixel Fold) and **flip-style** (e.g., Samsung Galaxy Z Flip 6, Motorola RAZR 2023) hardware matrix form factors:

* **Navigation & Travel:** `net.osmand.plus`, `app.organicmaps`, `mobi.maptrek`
* **Privacy & Security:** `ch.protonvpn.android`, `com.celzero.bravedns`, `com.windscribe.vpn`
* **Finance & Crypto:** `co.electriccoin.zcash.foss`, `com.coinerella.peercoin`, `com.capitalone.credittracker`
* **Communication:** `chat.delta.lite`, `chat.schildi.android`, `org.briarproject.briar`
* **Productivity:** `com.logseq.app`, `com.streetwriters.notesnook`, `io.github.quillpad`

---

## 🔗 Key External References
* **RotDroid Source Code:** [GitHub Repository (ImDiM/RotDroid)](https://github.com/ImDiM/RotDroid)
* **RotVL Vision Models:** [Hugging Face Models (ImDim/RotVL)](https://huggingface.co/ImDim/RotVL)
* **RotBench Dataset:** [Hugging Face Dataset (ImDim/RotBench)](https://huggingface.co/datasets/ImDim/RotBench)

---

## 📦 Binary APK Distribution
To avoid repository bloat and comply with Git storage best practices, raw application packages (`.apk`) are hosted under the **[Releases](../../releases)** tab.

1. Navigate to **Releases** on the right sidebar.
2. Select the target batch (e.g., `Nov 2 Standardized APK Batch`).
3. Download the zipped package or individual `.apk` assets for local device deployment.

## Everything is being slowly added so please be patient.
