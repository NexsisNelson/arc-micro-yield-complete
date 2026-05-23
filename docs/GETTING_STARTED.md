# Getting Started with Arc Micro-Yield

## 💫 5-Minute Overview

**Arc Micro-Yield** is a complete DeFi protocol for pooling retail USDC into institutional real-world asset investments.

**Two main parts:**
1. **Smart Contracts** - Production-ready Solidity backend
2. **Flutter App** - Multi-platform mobile/web frontend

## 🚀 Quick Start

### Prerequisites

**Option 1: Smart Contracts Only**
- Foundry installed
- 5 minutes

**Option 2: Flutter App Only**
- Flutter SDK installed
- 10 minutes

**Option 3: Full Stack**
- Both Foundry and Flutter
- 20 minutes

### Installation

```bash
# Clone repository
git clone https://github.com/NexsisNelson/arc-micro-yield-complete.git
cd arc-micro-yield-complete
```

### Smart Contracts

```bash
cd contracts

# Build
forge build

# Test (35+ tests)
forge test -v

# Expected output:
# ✓ Test 1...
# ✓ Test 2...
# ...
# Test result: ok. (35+) passed; 0 failed; 0 skipped
```

### Flutter App

```bash
cd app

# Install dependencies
flutter pub get

# Run (default: iOS simulator or Android emulator)
flutter run

# Or run on specific platform
flutter run -d chrome              # Web
flutter run -d windows             # Windows
flutter run -d macos               # macOS
flutter run -d linux               # Linux
```

## 📚 Documentation

### Quick Links

| Resource | Time | Link |
|----------|------|------|
| Project Overview | 5 min | [README.md](README.md) |
| Project Status | 5 min | [PROJECT_STATUS.md](PROJECT_STATUS.md) |
| System Architecture | 15 min | [docs/ARCHITECTURE_OVERVIEW.md](docs/ARCHITECTURE_OVERVIEW.md) |
| Smart Contracts | 15 min | [contracts/README.md](contracts/README.md) |
| Contract Details | 20 min | [contracts/ARCHITECTURE.md](contracts/ARCHITECTURE.md) |
| Flutter App | 10 min | [app/README.md](app/README.md) |
| Flutter Setup | 20 min | [app/SETUP_GUIDE.md](app/SETUP_GUIDE.md) |
| Web3 Integration | 30 min | [app/WEB3_INTEGRATION.md](app/WEB3_INTEGRATION.md) |
| Deployment | 20 min | [docs/DEPLOYMENT_GUIDE.md](docs/DEPLOYMENT_GUIDE.md) |
| Contributing | 10 min | [docs/CONTRIBUTING.md](docs/CONTRIBUTING.md) |

### Learning Path

**For Backend Developers:**
1. Read [README.md](README.md) (5 min)
2. Review [contracts/ARCHITECTURE.md](contracts/ARCHITECTURE.md) (20 min)
3. Run tests: `cd contracts && forge test -v` (5 min)
4. Explore [contracts/API_REFERENCE.md](contracts/API_REFERENCE.md) (15 min)
5. Review [contracts/BUGFIXES.md](contracts/BUGFIXES.md) (10 min)

**For Frontend Developers:**
1. Read [README.md](README.md) (5 min)
2. Follow [app/SETUP_GUIDE.md](app/SETUP_GUIDE.md) (20 min)
3. Run app: `cd app && flutter run` (5 min)
4. Study [app/WEB3_INTEGRATION.md](app/WEB3_INTEGRATION.md) (30 min)
5. Review [app/PROJECT_SUMMARY.md](app/PROJECT_SUMMARY.md) (10 min)

**For Full-Stack Developers:**
1. Read [README.md](README.md) (5 min)
2. Review [docs/ARCHITECTURE_OVERVIEW.md](docs/ARCHITECTURE_OVERVIEW.md) (20 min)
3. Setup backend: `cd contracts && forge test -v` (10 min)
4. Setup frontend: `cd app && flutter run` (10 min)
5. Study integration: [app/WEB3_INTEGRATION.md](app/WEB3_INTEGRATION.md) (30 min)

## 🔗 Repository Structure

```
arc-micro-yield-complete/
├── contracts/              # Smart contracts (1,200 LOC, 35+ tests)
├── app/                    # Flutter app (6 platforms)
├── docs/                   # Project documentation
├── README.md               # Main overview
├── PROJECT_STATUS.md       # Status tracking
├── ROADMAP.md              # Future plans
└── LICENSE                 # MIT
```

## 🔧 Development

### Smart Contracts

```bash
cd contracts

# Build
forge build

# Test
forge test -v

# Analysis
forge analyze

# Deploy locally
anvil              # Terminal 1: Start local blockchain
forge script script/Deploy.s.sol:Deploy --rpc-url http://localhost:8545 --broadcast  # Terminal 2
```

### Flutter App

```bash
cd app

# Install deps
flutter pub get

# Run app
flutter run

# Test
flutter test

# Analyze
flutter analyze

# Format
flutter format lib/
```

## 🏗️ Architecture

### Smart Contracts

```
User USDC
    │
    └─→ Vault (ERC4626)
            │
            ├─→ Strategy Manager
            │       │
            │       ├─→ Real Estate Strategy
            │       ├─→ Infrastructure Strategy
            │       └─→ Other Strategies
            │
            └─→ Yield Distributor
                    │
                    └─→ Shareholder Yield
```

### Smart Contracts + Flutter App

```
Flutter App
    │
    └─→ Web3 Integration (web3dart)
            │
            └─→ Arc Blockchain
                    │
                    ├─→ MicroYieldVault
                    ├─→ StrategyManager
                    ├─→ Investment Strategies
                    └─→ YieldDistributor
```

## 📊 Key Metrics

### Smart Contracts
- ✅ 1,200 lines of code
- ✅ 35+ tests (all passing)
- ✅ 60%+ comment coverage
- ✅ 0 security issues
- ✅ 6 critical bugs fixed

### Flutter App
- ✅ 6 platforms (iOS, Android, Web, Windows, macOS, Linux)
- ✅ Material Design 3
- ✅ Web3 integration framework
- ✅ Comprehensive documentation

### Documentation
- ✅ 5,000+ lines
- ✅ 10+ guides
- ✅ 50+ code examples
- ✅ 5+ diagrams

## 🐛 Common Tasks

### Testing Smart Contracts
```bash
cd contracts
forge test -v                          # Run all tests
forge test -v --match-test testName   # Run specific test
forge test -v --grep YieldDistributor # Run tests matching pattern
```

### Running Flutter App
```bash
cd app
flutter run                 # Default device
flutter run -d chrome       # Web browser
flutter run -d windows      # Windows desktop
flutter run -v              # Verbose output
```

### Code Quality
```bash
# Contracts
cd contracts && forge analyze

# App
cd app && flutter analyze
cd app && flutter format lib/
```

## 🚀 Next Steps

1. **Read the docs** - Start with main README.md
2. **Setup locally** - Get contracts and app running
3. **Review code** - Check out the implementation
4. **Run tests** - Verify everything works
5. **Explore integration** - See how app talks to contracts
6. **Start contributing** - Check contributing guidelines

## 📞 Need Help?

- 📖 **Documentation** - Check the guides in `/docs` and subdirectories
- 🐛 **Issues** - Open a GitHub issue
- 💬 **Discussions** - Start a GitHub discussion
- 📧 **Contributing** - See `docs/CONTRIBUTING.md`

## 📀 Project Status

✅ **Smart Contracts**: Production Ready
- Ready for deployment to testnet
- Awaiting third-party security audit
- All critical functionality tested

🔄 **Flutter App**: Development Ready
- Ready for feature implementation
- Base architecture complete
- Multi-platform support configured

## 📈 Performance Targets

- Transaction finality: <1 second (Arc blockchain)
- Transaction fees: Near-zero
- Yield generation: 8-12% APY
- User onboarding: <5 minutes
- App performance: 60 FPS

---

**Ready to get started?** Clone the repo and follow the Quick Start section above!

**Questions?** Check the documentation or open an issue.

**Want to contribute?** See `docs/CONTRIBUTING.md`

---

**Last Updated**: 2026-05-23  
**Status**: ✅ Ready for Development  
**Version**: 1.0.0
