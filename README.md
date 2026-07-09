# 9Router

A smart router and token saver for AI coding tools.

## Installation

1. Clone this repository:
```bash
git clone https://github.com/decolua/9router.git
cd 9router
```

2. Copy the environment variables template:
```bash
cp .env.example .env
```

3. Install dependencies:
```bash
npm install --legacy-peer-deps
```

## Running the Application

**Development Mode:**
```bash
PORT=20128 NEXT_PUBLIC_BASE_URL=http://localhost:20128 npm run dev
```

**Production Mode:**
```bash
npm run build
PORT=20128 HOSTNAME=0.0.0.0 NEXT_PUBLIC_BASE_URL=http://localhost:20128 npm run start
```
