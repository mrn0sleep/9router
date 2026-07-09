# 9Router

A smart router and token saver for AI coding tools.

## Prerequisites

Before installing 9Router, make sure the following tools are installed on your system.

### Node.js & npm

9Router requires **Node.js v18.18+** (recommended: v20 LTS or later). npm is included with Node.js.

Check if you already have them installed:
```bash
node -v
npm -v
```

If both commands print a version number, you're good to go. If not, follow the installation guide for your OS below.

### Git

```bash
git --version
```

If not installed, download from [git-scm.com](https://git-scm.com/downloads).

---

## Installation (Linux / macOS)

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

### Running the Application

**Development Mode:**
```bash
PORT=20128 NEXT_PUBLIC_BASE_URL=http://localhost:20128 npm run dev
```

**Production Mode:**
```bash
npm run build
PORT=20128 HOSTNAME=0.0.0.0 NEXT_PUBLIC_BASE_URL=http://localhost:20128 npm run start
```

---

## Installation (Windows)

### Step 1 — Install Node.js & npm

1. Go to [https://nodejs.org](https://nodejs.org) and download the **LTS** installer (`.msi`).
2. Run the installer — keep all defaults checked (this will install both Node.js and npm).
3. **Important:** Check the box **"Automatically install the necessary tools"** if prompted (this installs build tools needed by some native dependencies).
4. After installation, **open a new Command Prompt or PowerShell** and verify:
```powershell
node -v
npm -v
```
Both should print a version number (e.g. `v20.x.x` and `10.x.x`).

> **Alternative:** If you prefer a version manager, you can use [nvm-windows](https://github.com/coreybutler/nvm-windows) to install and switch between Node.js versions:
> ```powershell
> nvm install lts
> nvm use lts
> ```

### Step 2 — Install Git

1. Download Git from [https://git-scm.com/download/win](https://git-scm.com/download/win).
2. Run the installer — the defaults are fine.
3. Verify:
```powershell
git --version
```

### Step 3 — Clone & Setup

Open **Command Prompt**, **PowerShell**, or **Git Bash** and run:

```powershell
git clone https://github.com/decolua/9router.git
cd 9router
```

Copy the environment file:

**PowerShell:**
```powershell
Copy-Item .env.example .env
```

**Command Prompt:**
```cmd
copy .env.example .env
```

**Git Bash:**
```bash
cp .env.example .env
```

Install dependencies:
```powershell
npm install --legacy-peer-deps
```

### Step 4 — Run the Application

On Windows, environment variables are set differently. Use one of the methods below.

**Development Mode (PowerShell):**
```powershell
$env:PORT="20128"; $env:NEXT_PUBLIC_BASE_URL="http://localhost:20128"; npm run dev
```

**Development Mode (Command Prompt):**
```cmd
set PORT=20128 && set NEXT_PUBLIC_BASE_URL=http://localhost:20128 && npm run dev
```

**Production Mode (PowerShell):**
```powershell
npm run build
$env:PORT="20128"; $env:HOSTNAME="0.0.0.0"; $env:NEXT_PUBLIC_BASE_URL="http://localhost:20128"; npm run start
```

**Production Mode (Command Prompt):**
```cmd
npm run build
set PORT=20128 && set HOSTNAME=0.0.0.0 && set NEXT_PUBLIC_BASE_URL=http://localhost:20128 && npm run start
```

> **Tip:** If you want a cross-platform way to set env variables, you can install [cross-env](https://www.npmjs.com/package/cross-env):
> ```powershell
> npm install -g cross-env
> cross-env PORT=20128 NEXT_PUBLIC_BASE_URL=http://localhost:20128 npm run dev
> ```

---

## Accessing the Dashboard

Once running, open your browser and go to:

```
http://localhost:20128/dashboard
```

The API endpoint is available at:

```
http://localhost:20128/v1
```
