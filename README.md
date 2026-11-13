# 🌾 FarmLink AI
### From Farm to Market. Smarter. Faster. Fairer.

<p align="center">
  <strong>An intelligent agricultural supply-chain platform connecting farmers, buyers, FPOs and logistics providers.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Flask-3-black?style=for-the-badge&logo=flask" />
  <img src="https://img.shields.io/badge/PostgreSQL-18-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/AI-Driven-8A2BE2?style=flat-square" />
  <img src="https://img.shields.io/badge/AgriTech-Innovation-2E8B57?style=flat-square" />
  <img src="https://img.shields.io/badge/Status-Prototype-orange?style=flat-square" />
  <img src="https://img.shields.io/badge/Languages-13-blue?style=flat-square" />
</p>

---

## 🌱 The Vision

Agricultural supply chains often involve multiple intermediaries, fragmented transportation, unpredictable demand and limited access to market intelligence.

Small farmers frequently struggle to reach buyers directly, while inefficient transportation increases costs and the risk of produce spoilage.

**FarmLink AI aims to change this.**

It brings farmers, Farmer Producer Organizations (FPOs), buyers and logistics operators together through an intelligent digital ecosystem.

By combining marketplace connectivity, AI-assisted insights, collaborative transportation and supply-chain management, FarmLink AI aims to make agricultural trade more transparent, efficient and accessible.

---

## ✨ What Makes FarmLink AI Different?

<table>
<tr>
<td width="50%">
<h3>🌾 Direct Farmer Marketplace</h3>
Connect farmers and FPOs with buyers through digital produce listings, transparent pricing and order management.
</td>
<td width="50%">
<h3>🚛 Intelligent Load Pooling</h3>
Combine compatible orders into shared shipments, improving vehicle utilisation and reducing fragmented transportation.
</td>
</tr>
<tr>
<td width="50%">
<h3>📊 AI-Powered Intelligence</h3>
Demand forecasting, supply-demand gap analysis and price intelligence to support better agricultural decisions.
</td>
<td width="50%">
<h3>📍 Smart Logistics</h3>
Shipment manifests, route planning, delivery stages and GPS-based location updates.
</td>
</tr>
<tr>
<td width="50%">
<h3>🌐 Multilingual Accessibility</h3>
13 selectable languages, including Kannada, Hindi, Telugu, Tamil, Malayalam and other Indian languages.
</td>
<td width="50%">
<h3>🏢 Enterprise Integration</h3>
SAP-style export adapters for purchase orders, transportation orders and supply-chain disruption alerts.
</td>
</tr>
</table>

---

## 🚀 Key Features

### 1. Farmer & FPO Workspace
- Create and manage agricultural produce listings.
- Track available inventory and quantities.
- Access demand forecasts and price intelligence.
- Compare buyer offers and estimated net proceeds.
- Participate in shared transportation opportunities.
- Manage orders and notifications.

### 2. Buyer Marketplace
- Explore available agricultural produce.
- View product details and pricing.
- Add products to cart and place orders.
- Simulated checkout and order management.
- Track order and delivery stages.

### 3. Logistics Management
- Manage shipments and transportation capacity.
- Coordinate pooled orders.
- Create shipment manifests and delivery stops.
- View routes and shipment locations.
- Receive GPS location updates.
- Manage delivery progress and disruptions.

### 4. AI & Supply-Chain Intelligence
- Agricultural demand forecasting.
- Supply-demand gap analysis.
- Price intelligence.
- Buyer-offer comparison.
- Alternative buyer matching during disruptions.
- Operational analytics.

### 5. Multilingual Experience

FarmLink AI supports 13 selectable locales:

| Language | Code |
|---|---|
| English | `en` |
| Kannada | `kn` |
| Hindi | `hi` |
| Telugu | `te` |
| Tamil | `ta` |
| Malayalam | `ml` |
| Marathi | `mr` |
| Bengali | `bn` |
| Gujarati | `gu` |
| Punjabi | `pa` |
| Odia | `or` |
| Assamese | `as` |
| Urdu | `ur` |

Language preferences persist across refreshes, with English as the fallback when translations are unavailable.

---

## 🛠️ Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | React 19, Vite 8 |
| Routing | React Router 7 |
| Styling | Tailwind CSS 4 |
| UI & Charts | Lucide React, Recharts |
| Internationalization | i18next, react-i18next |
| Backend | Python, Flask 3 |
| Database | PostgreSQL 18 / SQLite |
| ORM | SQLAlchemy 2 |
| Database Driver | psycopg 3 |
| Maps | Google Maps, Geoapify |
| Testing | pytest, oxlint |
| Enterprise | SAP-style integration adapters |

---

## 🏗️ System Architecture

```mermaid
flowchart TB
    A["👨‍🌾 Farmer / FPO"]
    B["🛒 Buyer"]
    C["🚛 Logistics Operator"]
    D["⚙️ Administrator"]

    A --> E["React + Vite Frontend"]
    B --> E
    C --> E
    D --> E

    E --> F["Flask REST API"]

    F --> G[("PostgreSQL / SQLite")]
    F --> H["AI & Intelligence Engines"]
    F --> I["Shipment & Routing Services"]
    F --> J["SAP Export Adapters"]

    I --> K["Google Maps / Geoapify"]
```

### Order-to-Delivery Workflow

```mermaid
flowchart TD
    A["Farmer creates produce listing"]
    B["Buyer discovers produce"]
    C["Buyer places an order"]
    D["Inventory gets reserved"]
    E["Compatible orders are pooled"]
    F["Shipment and manifest created"]
    G["Logistics manages delivery"]
    H["Delivery status updated"]

    A --> B --> C --> D --> E --> F --> G --> H
```

---

## 💻 Getting Started

### Prerequisites

- Node.js 20.19+ or 22.12+
- Python 3.10+
- PostgreSQL 18+ (optional when using SQLite)

### 1. Clone the repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd <YOUR_PROJECT_FOLDER>
```

### 2. Install frontend dependencies

```bash
npm install
npm run dev
```

Frontend: `http://localhost:5173`

### 3. Configure the backend

Open a second terminal:

```bash
cd server
pip install -r requirements.txt
python app.py
```

Backend: `http://127.0.0.1:5000`

### 4. Environment configuration

Create a `.env` file in the project root using `.env.example` as a reference.

```env
VITE_API_BASE_URL=

FARMLINK_DATABASE_URL=postgresql+psycopg://username:password@127.0.0.1:5432/farmlink

FARMLINK_CORS_ORIGINS=http://localhost:5173,http://127.0.0.1:5173
FARMLINK_HOST=127.0.0.1
PORT=5000

VITE_GOOGLE_MAPS_API_KEY=
VITE_GOOGLE_MAPS_MAP_ID=

GOOGLE_MAPS_SERVER_API_KEY=
GEOAPIFY_API_KEY=
FARMLINK_GEOCODE_REGION=in
```

**Important:** Never commit `.env` files or expose server-side API keys through frontend environment variables.

### 5. Database setup

FarmLink AI includes SQLite for local demonstration and supports PostgreSQL for persistent database storage.

For an existing database requiring migrations:

```bash
cd server

python migrate_shipment_items.py
python migrate_shipment_locations.py
python seed.py --repair-demo-users
```

For transferring existing SQLite data to an empty PostgreSQL database:

```bash
python migrate_sqlite_to_postgres.py
```

---

## 📂 Project Structure

```text
FarmLink-AI/
│
├── src/
│   ├── pages/              # Role-specific application screens
│   ├── components/         # Reusable UI components
│   ├── context/            # Application state management
│   ├── services/           # API integration
│   ├── i18n/               # Language resources
│   └── data/               # Demo data
│
├── server/
│   ├── app.py              # Flask REST API
│   ├── models.py           # Database models
│   ├── *_engine.py         # Forecasting, pricing, pooling
│   ├── routing_service.py  # Geocoding and routing
│   ├── sap_adapter.py      # SAP-style export adapters
│   ├── seed.py             # Database seeding
│   ├── migrate_*.py        # Database migrations
│   └── tests/              # Backend tests
│
├── scripts/                # Translation audit utilities
├── .env.example            # Environment template
├── package.json
└── README.md
```

---

## 🔌 API Overview

The backend exposes REST APIs under `/api`.

| Module | Main Endpoints |
|---|---|
| Authentication | `/auth/demo-login`, `/auth/me` |
| Products | `/products` |
| Orders | `/orders` |
| Pooling | `/pooling/opportunities`, `/pooling/confirm` |
| Buyer Offers | `/offers`, `/offers/compare` |
| Forecasting | `/forecasting`, `/forecasting/gaps` |
| Disruptions | `/disruptions` |
| Shipments | `/shipments` |
| Routing | `/routing/geocode`, `/routing/route` |
| Analytics | `/analytics` |
| Notifications | `/notifications` |
| SAP | `/sap/status`, `/sap/export-po`, `/sap/export-tm` |
| Audit Logs | `/audit-logs` |

<details>
<summary><strong>View detailed API documentation</strong></summary>

### Products

- `GET /api/products`
- `GET /api/products/{productId}`
- `POST /api/products`
- `PUT /api/products/{productId}`
- `DELETE /api/products/{productId}`

### Orders

- `GET /api/orders`
- `POST /api/orders`
- `PATCH /api/orders/{orderId}/stage`
- `POST /api/orders/{orderId}/cancel`

### Pooling & Offers

- `GET /api/pooling/opportunities`
- `POST /api/pooling/confirm`
- `GET /api/offers`
- `POST /api/offers/compare`
- `POST /api/offers/{offerId}/accept`

### Forecasting & Disruptions

- `GET /api/forecasting`
- `GET /api/forecasting/gaps`
- `GET /api/disruptions`
- `GET /api/disruptions/{disruptionId}/matches`
- `POST /api/disruptions/{disruptionId}/recover`

### Shipment & Routing

- `GET /api/shipments`
- `POST /api/shipments`
- `GET /api/shipments/{shipmentId}/location`
- `POST /api/shipments/{shipmentId}/location`
- `POST /api/shipments/{shipmentId}/cancel`
- `PATCH /api/shipments/{shipmentId}/stage`
- `GET /api/routing/geocode`
- `POST /api/routing/route`

### SAP & Administration

- `GET /api/sap/status`
- `POST /api/sap/export-po/{orderId}`
- `POST /api/sap/export-tm/{shipmentId}`
- `POST /api/sap/control-tower-alert/{disruptionId}`
- `GET /api/analytics`
- `GET /api/notifications`
- `PATCH /api/notifications/{notificationId}/read`
- `GET /api/audit-logs`

</details>

---

## 🏢 Enterprise Integration – SAP

FarmLink AI includes an adapter layer designed to generate SAP-style integration payloads.

Supported export formats include:

- SAP S/4HANA Materials Management (MM) purchase orders.
- SAP Transportation Management (TM) freight orders.
- SAP Supply Chain Control Tower disruption alerts.

**Note:** These are mock export adapters, not live SAP system integrations.

---

## 🧪 Testing & Quality Checks

Frontend:

```bash
npm run lint
npm run build
npm run i18n:check
npm run i18n:audit
```

Backend:

```bash
cd server
pytest tests/
```

---

## ⚠️ Prototype Scope & Limitations

FarmLink AI is currently a working prototype.

- Authentication uses a demonstration role-selection flow.
- Checkout uses simulated payments; no real money is processed.
- Some language resources may use English fallback.
- Forecasting and price intelligence use demonstration inputs rather than validated live agricultural datasets.
- Live GPS tracking requires an external device or browser location integration.
- SAP exports generate mock payloads rather than connecting to live SAP infrastructure.

Production deployment would require hardened authentication, managed database infrastructure, monitoring, security controls and production integrations.

---

## 🌍 Our Impact

FarmLink AI is designed around several United Nations Sustainable Development Goals:

| Goal | Focus |
|---|---|
| SDG 2 | Zero Hunger |
| SDG 8 | Decent Work and Economic Growth |
| SDG 12 | Responsible Consumption and Production |
| SDG 13 | Climate Action |

---

## 🤝 Contributing

Contributions, suggestions and ideas are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Test your implementation.
5. Submit a pull request with a clear description.

---

## 👨‍💻 Built With Purpose

**FarmLink AI**

Building a smarter, more connected and more accessible agricultural supply chain.

<p align="center">
  🌾 Empowering Farmers · Connecting Markets · Optimising Logistics
</p>

<p align="center">
  <strong>Direct Markets. Smarter Decisions. Better Delivery.</strong>
</p>
