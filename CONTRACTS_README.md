# Smart Contract Section

When referencing smart contracts from the complete repository, use:

```
arc-micro-yield-complete/contracts/src/InfrastructureStrategy.sol
arc-micro-yield-complete/contracts/src/RealEstateStrategy.sol
```

To build the contracts:

```bash
cd arc-micro-yield-complete/contracts
forge build
forge test -v
```

## Smart Contracts Included

1. **MicroYieldVault.sol** - ERC4626 vault
2. **StrategyManager.sol** - Strategy orchestration  
3. **RealEstateStrategy.sol** - Real estate investments
4. **InfrastructureStrategy.sol** - Infrastructure investments
5. **YieldDistributor.sol** - Yield distribution
6. **IStrategy.sol** - Strategy interface
7. **MockUSDC.sol** - Test token

## References

For the original smart contracts repository:
- https://github.com/NexsisNelson/arc-micro-yield

For the complete unified repository:
- https://github.com/NexsisNelson/arc-micro-yield-complete
