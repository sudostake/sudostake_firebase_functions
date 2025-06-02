# 🌐 Sudostake Firebase Functions

The project includes:
- **Firebase Cloud Functions** written in TypeScript for backend logic and API routes.

&nbsp;

## 🔧 Running Firebase Functions Locally

1. **Navigate to the `firebase_functions/` folder**:

```bash
cd firebase_functions
```

2. **Install dependencies**:

```bash
npm install
```

3. **Build the functions**:

```bash
npm run build
```

4. **Start the Firebase Functions emulator**:

```bash
npm run serve
```

```
http://127.0.0.1:5001/sudostake/us-central1

# Index a vault example
curl -X POST http://127.0.0.1:5001/sudostake/us-central1/index_vault \
  -H "Content-Type: application/json" \
  -d '{"vault": "vault-0.nzaza.testnet"}'

# Get user vaults example
curl -X GET "http://127.0.0.1:5001/sudostake/us-central1/get_user_vaults?owner=selfcustody.testnet&factory_id=nzaza.testnet" \
  -H "Content-Type: application/json"

# View pending liquidity requests
curl -X GET "http://127.0.0.1:5001/sudostake/us-central1/view_pending_liquidity_requests?factory_id=nzaza.testnet" \
  -H "Content-Type: application/json"

# View lender positions
curl -X GET "http://127.0.0.1:5001/sudostake/us-central1/view_lender_positions?factory_id=nzaza.testnet&lender_id=usdclender.testnet"
```

> 🔎 View the Emulator UI at [http://localhost:5002](http://localhost:5002)
