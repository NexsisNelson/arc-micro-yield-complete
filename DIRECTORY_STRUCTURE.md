# Directory Structure Guide

This unified repository contains both the Arc Micro-Yield smart contracts and Flutter application.

## 📁 Project Organization

### Root Level

```
arc-micro-yield-complete/
├── contracts/          # Smart Contract Backend
├── app/                # Flutter Frontend
├── docs/               # Project Documentation
├── README.md           # Main project overview
├── PROJECT_STATUS.md   # Current status
├── ROADMAP.md          # Future plans
├── LICENSE             # MIT License
└── .gitignore          # Git ignore rules
```

## 🔗 Smart Contracts: `contracts/`

### Directory Structure

```
contracts/
├── src/                             # Smart contract source code
│   ├── MicroYieldVault.sol            # Main vault (ERC4626)
│   ├── StrategyManager.sol            # Portfolio manager
│   ├── RealEstateStrategy.sol         # RE investment strategy
│   ├── InfrastructureStrategy.sol     # Infrastructure strategy
│   ├── YieldDistributor.sol           # Yield distribution
│   ├── IStrategy.sol                  # Strategy interface
│   └── MockUSDC.sol                   # Mock USDC token
├── script/                         # Deployment scripts
│   └── Deploy.s.sol                   # Main deployment script
├── test/                           # Test suite
│   ├── MicroYieldVault.t.sol          # Vault tests (20+)
│   └── Strategy.t.sol                 # Strategy tests (15+)
├── lib/                            # Dependencies
│   └── openzeppelin-contracts/        # OpenZeppelin libraries
├── foundry.toml                    # Foundry configuration
├── README.md                       # Smart contract overview
├── ARCHITECTURE.md                 # Technical architecture
├── BUGFIXES.md                     # Bug fixes documentation
├── SECURITY_ANALYSIS.md            # Security analysis
├── GETTING_STARTED.md              # Setup guide
└── API_REFERENCE.md                # Contract API docs
```

### Key Files

| File | Purpose | Lines |
|------|---------|-------|
| MicroYieldVault.sol | Main vault contract (ERC4626) | 290 |
| StrategyManager.sol | Strategy orchestration | 250 |
| RealEstateStrategy.sol | RE investments | 155 |
| InfrastructureStrategy.sol | Infra investments | 155 |
| YieldDistributor.sol | Yield distribution | 120 |
| IStrategy.sol | Strategy interface | 61 |
| MockUSDC.sol | Mock USDC token | 52 |
| Deploy.s.sol | Deployment orchestration | 230 |

### Documentation in `contracts/`

- **README.md** - Overview of smart contracts
- **ARCHITECTURE.md** - System design and flow
- **BUGFIXES.md** - Complete bug fix documentation
- **SECURITY_ANALYSIS.md** - Security review
- **GETTING_STARTED.md** - Contract development setup
- **API_REFERENCE.md** - Function and event documentation

### Quick Commands

```bash
cd contracts

# Build contracts
forge build

# Run tests
forge test -v

# Deploy to local Anvil
forge script script/Deploy.s.sol:Deploy --rpc-url http://localhost:8545 --broadcast

# Deploy to testnet
PRIVATE_KEY=<key> forge script script/Deploy.s.sol:Deploy --rpc-url <rpc> --broadcast
```

## 📱 Flutter App: `app/`

### Directory Structure

```
app/
├── lib/                             # Dart source code
│   └── main.dart                     # Application entry point
├── test/                            # Test suite
│   └── widget_test.dart               # Widget tests
├── android/                        # Android platform code
├── ios/                             # iOS platform code
├── web/                             # Web platform files
├── windows/                         # Windows platform code
├── macos/                           # macOS platform code
├── linux/                           # Linux platform code
├── pubspec.yaml                     # Dependencies & config
├── pubspec.lock                     # Locked dependencies
├── analysis_options.yaml            # Linting configuration
├── README.md                        # Flutter app overview
├── SETUP_GUIDE.md                   # Development setup
├── WEB3_INTEGRATION.md              # Web3 integration guide
└── PROJECT_SUMMARY.md               # Project summary
```

### Key Files

| File | Purpose | Type |
|------|---------|------|
| lib/main.dart | App entry point | Dart |
| test/widget_test.dart | Widget tests | Test |
| pubspec.yaml | Dependencies | Config |
| analysis_options.yaml | Linting rules | Config |

### Documentation in `app/`

- **README.md** - Quick overview
- **SETUP_GUIDE.md** - Complete development setup (1,400 lines)
- **WEB3_INTEGRATION.md** - Blockchain integration (900 lines)
- **PROJECT_SUMMARY.md** - Project summary

### Quick Commands

```bash
cd app

# Install dependencies
flutter pub get

# Run on mobile
flutter run

# Run on web
flutter run -d chrome

# Run tests
flutter test

# Code analysis
flutter analyze

# Build for release
flutter build apk --release         # Android
flutter build ios --release         # iOS
flutter build web --release         # Web
flutter build windows --release     # Windows
flutter build macos --release       # macOS
flutter build linux --release       # Linux
```

## 📚 Documentation: `docs/`

### Project-Level Documentation

```
docs/
├── ARCHITECTURE_OVERVIEW.md         # System design
├── GETTING_STARTED.md               # Quick start guide
├── DEPLOYMENT_GUIDE.md              # Deployment instructions
└── CONTRIBUTING.md                  # Contribution guidelines
```

### Quick Navigation

| Document | Purpose | Read Time |
|----------|---------|----------|
| docs/ARCHITECTURE_OVERVIEW.md | Complete system design | 15 min |
| docs/GETTING_STARTED.md | Quick start and setup | 10 min |
| docs/DEPLOYMENT_GUIDE.md | Deployment procedures | 20 min |
| docs/CONTRIBUTING.md | Contribution process | 10 min |

## 🔗 Quick Navigation

### For Backend Developers

1. **Start**: contracts/README.md
2. **Setup**: contracts/GETTING_STARTED.md
3. **Learn**: contracts/ARCHITECTURE.md
4. **Reference**: contracts/API_REFERENCE.md
5. **Debug**: contracts/BUGFIXES.md

### For Frontend Developers

1. **Start**: app/README.md
2. **Setup**: app/SETUP_GUIDE.md
3. **Integration**: app/WEB3_INTEGRATION.md
4. **Overview**: app/PROJECT_SUMMARY.md

### For DevOps / Deployment

1. **Start**: docs/DEPLOYMENT_GUIDE.md
2. **Backend**: contracts/ (Deploy.s.sol, foundry.toml)
3. **Frontend**: app/ (build commands)
4. **Monitoring**: docs/DEPLOYMENT_GUIDE.md

### For Contributors

1. **Guidelines**: docs/CONTRIBUTING.md
2. **Setup**: docs/GETTING_STARTED.md
3. **Backend**: contracts/GETTING_STARTED.md
4. **Frontend**: app/SETUP_GUIDE.md

## 📋 Documentation Roadmap

```
Root Level (You are here)
├── README.md              - Project overview ✅
├── PROJECT_STATUS.md      - Status tracking ✅
├── ROADMAP.md             - Future plans ✅
└── DIRECTORY_STRUCTURE.md - This file ✅

contracts/
├── README.md              - Overview
├── ARCHITECTURE.md        - Design
├── BUGFIXES.md            - Fixes
├── SECURITY_ANALYSIS.md   - Security
└── API_REFERENCE.md       - API

app/
├── README.md              - Overview
├── SETUP_GUIDE.md         - Setup
├── WEB3_INTEGRATION.md    - Integration
└── PROJECT_SUMMARY.md     - Summary

docs/
├── ARCHITECTURE_OVERVIEW.md - System design
├── GETTING_STARTED.md      - Quick start
├── DEPLOYMENT_GUIDE.md     - Deployment
└── CONTRIBUTING.md         - Contributing
```

## 🛠️ Development Workflow

### Local Development

```bash
# Clone repo
git clone https://github.com/NexsisNelson/arc-micro-yield-complete.git
cd arc-micro-yield-complete

# Smart contracts
cd contracts
forge test -v
forge build

# Flutter app
cd ../app
flutter pub get
flutter run
```

### Making Changes

```bash
# Create feature branch
git checkout -b feature/amazing-feature

# Make changes
# ...

# Test changes
# For contracts: forge test -v
# For app: flutter test

# Commit
git commit -m "feat: Add amazing feature"

# Push
git push origin feature/amazing-feature

# Open PR
# (on GitHub)
```

## 📋 File Size Reference

### Smart Contracts

```
Total LOC: ~1,200
- MicroYieldVault.sol: 290 lines
- StrategyManager.sol: 250 lines
- RealEstateStrategy.sol: 155 lines
- InfrastructureStrategy.sol: 155 lines
- YieldDistributor.sol: 120 lines
- IStrategy.sol: 61 lines
- MockUSDC.sol: 52 lines
- Deploy.s.sol: 230 lines
- Tests: ~600 lines
```

### Flutter App

```
Total LOC: ~200 (core)
- lib/main.dart: 100 lines
- test/widget_test.dart: 50 lines
- Platform configs: 50 lines
- pubspec.yaml: ~100 lines
```

### Documentation

```
Total Lines: ~5,000
- Root docs: 500 lines
- contracts/: 1,500 lines
- app/: 2,000 lines
- docs/: 1,000 lines
```

## 🗣️ File Navigation Tips

### Finding Smart Contract Docs

- Contract overview? → `contracts/README.md`
- How contracts work? → `contracts/ARCHITECTURE.md`
- What bugs were fixed? → `contracts/BUGFIXES.md`
- Function reference? → `contracts/API_REFERENCE.md`
- Is it secure? → `contracts/SECURITY_ANALYSIS.md`

### Finding Flutter Docs

- App overview? → `app/README.md`
- How to setup? → `app/SETUP_GUIDE.md`
- How to use Web3? → `app/WEB3_INTEGRATION.md`
- Project summary? → `app/PROJECT_SUMMARY.md`

### Finding Project Docs

- Project status? → `PROJECT_STATUS.md`
- What's next? → `ROADMAP.md`
- How to deploy? → `docs/DEPLOYMENT_GUIDE.md`
- How to contribute? → `docs/CONTRIBUTING.md`

## 📁 Directory at a Glance

```
arc-micro-yield-complete/              # Root
├── contracts/                       # Backend (1,200 LOC)
│   ├── src/                         # 7 contracts
│   ├── test/                        # 35+ tests
│   └── README.md + docs
├── app/                            # Frontend (multi-platform)
│   ├── lib/                         # Dart code
│   ├── test/                        # Tests
│   ├── android/ ios/ web/ ...       # Platforms
│   └── README.md + guides
├── docs/                           # Project docs
├── README.md                      # Start here
├── PROJECT_STATUS.md              # Status
├── ROADMAP.md                     # Plans
└── LICENSE                        # MIT
```

---

**Last Updated**: 2026-05-23  
**Version**: 1.0.0

For detailed information, start with the **README.md** in the root or the respective subdirectories.
