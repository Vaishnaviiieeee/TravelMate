# 🧳 TravelMate

> A travel companion platform that helps travelers plan trips, find verified tour guides, manage expenses and meet like-minded companions.

![Status](https://img.shields.io/badge/status-in%20development-orange)
![Project](https://img.shields.io/badge/project-MCA%20Academic-blue)

---

## 📌 1. Project Overview
**TravelMate** is an academic MCA project that brings the main steps of a trip into one platform: exploring destinations, planning an itinerary, booking a local tour guide, tracking expenses, finding travel companions and chatting with them. Guides are verified automatically and user reports are moderated automatically to keep the community safe.

## ❗ 2. Problem Statement
Travelers usually depend on many separate apps and websites: one for destination research, another for itinerary planning, another for guides, and another for budgeting. It is also hard to know whether a local guide is genuine, or to find safe companions for a trip. TravelMate aims to solve this with **one platform** that offers verified guides, organised planning and safer interaction.

## 🎯 3. Project Objectives
- Provide a single platform for trip planning and management.
- Let travelers find and book **verified** tour guides.
- Help travelers discover destinations and attractions.
- Help travelers track trip expenses and view a trip report.
- Connect travelers with compatible companions and allow chat.
- Keep the platform safe through automatic moderation of reports.

## ✨ 4. Main Features
See [Project Status](#-13-project-status) for what is implemented today.

- 🔐 Account management with automatic guide verification
- 📅 Tour guide booking
- 🗺️ Destination and attraction exploration
- 🧭 Trip, itinerary and route planning
- 💰 Expense tracking and trip report
- 🤝 Companion matching and chat
- 🛡️ Automatic moderation of user reports

## 🧩 5. Project Modules
Based on the project's Level-1 Data Flow Diagram ([`Documentation/diagrams/TravelMate-DFD-Level1.pdf`](Documentation/diagrams/TravelMate-DFD-Level1.pdf)).

| # | Module | Description | Data Store |
|---|--------|-------------|------------|
| 1.0 | **Manage Accounts and Auto-Verify Guides** | Registration/login for travelers and guides; guide profiles are verified automatically | D1 – Users and Guide Profiles |
| 2.0 | **Book Tour Guide** | Travelers book guides; guides respond to bookings | D5 – Guide Bookings |
| 3.0 | **Explore Destinations** | Browse destinations and attractions | D2 – Destinations and Attractions |
| 4.0 | **Plan Trip** | Create trips, itineraries and routes | D3 – Trips, Itineraries and Routes |
| 5.0 | **Manage Expenses and Trip Report** | Record expenses and generate a trip report | D4 – Expenses and Trip Reports |
| 6.0 | **Match Companions and Chat** | Find travel companions and chat | D6 – Companions and Chat |
| 7.0 | **Auto-Moderate Reports** | User reports are checked and handled automatically | D7 – User Reports |

## 👥 6. User Roles
| Role | Can access (as per DFD) |
|------|--------------------------|
| 🧍 **Traveler** | Modules 1.0 – 7.0 (accounts, booking guides, destinations, trip planning, expenses, companions/chat, reporting) |
| 🧑‍🏫 **Tour Guide** | Modules 1.0 and 2.0 (account/verification and handling bookings) |

> Detailed role permissions are to be finalised in the SRS/design phase.

## 🛠️ 7. Technology Stack
> ⚠️ **Needs confirmation.** The repository currently contains only two blank `index.html` files, so no framework, language or database has been chosen in code yet. Fill in the table once decided.

| Layer | Technology |
|-------|-----------|
| Frontend | HTML (placeholder file only) – framework **to be confirmed** |
| Backend | **To be confirmed** |
| Database | **To be confirmed** |
| Auto-verification / auto-moderation method | **To be confirmed** |
| Version Control | Git & GitHub |

## 🗄️ 8. Database Information
The database is designed through an **Entity Relationship Diagram with 19 entities**, grouped under the 7 DFD data stores:

| DFD Data Store | Main ERD Entities |
|----------------|-------------------|
| D1 Users and Guide Profiles | USER, GUIDE_PROFILE |
| D2 Destinations and Attractions | TOURISM_CATEGORY, DESTINATION, ATTRACTION |
| D3 Trips, Itineraries and Routes | TRIP, ITINERARY, ITINERARY_STOP, ROUTE, ROUTE_STOP |
| D4 Expenses and Trip Reports | EXPENSE, EXPENSE_ITEM, TRIP_REPORT |
| D5 Guide Bookings | GUIDE_BOOKING |
| D6 Companions and Chat | COMPANION_REQUEST, TRAVEL_CONNECTION, CHAT_ROOM, CHAT_MESSAGE |
| D7 User Reports | USER_REPORT |

The database software and schema scripts are **to be confirmed / not created yet**. Full entity and attribute list: [`Database/README.md`](Database/README.md).

## 📁 9. Repository Structure
```
TravelMate/
├── Frontend/                 # Client-side code (currently a placeholder index.html)
│   ├── index.html
│   └── README.md
├── Backend/                  # Server-side code (currently a placeholder index.html)
│   ├── index.html
│   └── README.md
├── Database/                 # Database notes and, later, schema scripts
│   └── README.md
├── Documentation/            # Project documents
│   ├── project-scope.md
│   └── diagrams/
│       └── TravelMate-DFD-Level1.pdf   # (ERD to be added)
├── Testing/                  # Test plan and, later, test files
│   └── README.md
├── .gitignore
└── README.md
```
*(No GitHub Actions workflow is included yet; it will be added once the tech stack is fixed.)*

## ⚙️ 10. Installation and Setup
Clone the repository:
```bash
git clone https://github.com/Vaishnaviiieeee/TravelMate.git
cd TravelMate
```
Dependency installation steps will be added after the technology stack is confirmed. Never commit `.env` files or API keys; share a `.env.example` instead.

## ▶️ 11. How to Run the Project
Currently only placeholder pages exist, so there is nothing functional to run. Open `Frontend/index.html` in a browser to see the blank page. Run instructions will be updated as development progresses.

## 🧪 12. Testing Information
No automated tests exist yet. A module-wise test plan outline is in [`Testing/README.md`](Testing/README.md).

## 📊 13. Project Status
| Module | Design (DFD) | Implementation |
|--------|:-----------:|:--------------:|
| 1.0 Manage Accounts and Auto-Verify Guides | ✅ Done | ⏳ Planned |
| 2.0 Book Tour Guide | ✅ Done | ⏳ Planned |
| 3.0 Explore Destinations | ✅ Done | ⏳ Planned |
| 4.0 Plan Trip | ✅ Done | ⏳ Planned |
| 5.0 Manage Expenses and Trip Report | ✅ Done | ⏳ Planned |
| 6.0 Match Companions and Chat | ✅ Done | ⏳ Planned |
| 7.0 Auto-Moderate Reports | ✅ Done | ⏳ Planned |

**Current stage:** Repository set up, analysis/design phase (Level-1 DFD complete). Implementation has not started.

## 🚀 14. Future Enhancements
*(Ideas beyond the current scope — to be discussed with your guide)*
- Mobile application version
- Notifications for bookings and chat messages
- Multi-language support

## 👩‍💻 15. Development Team / Contributors
| Name | Role | GitHub |
|------|------|--------|
| Vaishnavi *(add full name)* | Developer | [@Vaishnaviiieeee](https://github.com/Vaishnaviiieeee) |

**Institution / Course:** MCA *(add college & year)*  
**Project Guide:** *(add guide's name)*