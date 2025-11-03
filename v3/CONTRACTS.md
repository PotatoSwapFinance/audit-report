# PotatoSwap V3 - Deployed Contracts

## Mainnet Deployment

### Core Contracts

| Contract | Address | Explorer | Verified |
|----------|---------|----------|----------|
| HyperindexV3Factory | *See audit report* | Block Explorer | ✅ |
| SwapV3PoolDeployer | *See audit report* | Block Explorer | ✅ |

### Periphery Contracts

| Contract | Address | Explorer | Verified |
|----------|---------|----------|----------|
| HyperindexV3Router | *See audit report* | Block Explorer | ✅ |
| NonfungiblePositionManager | *See audit report* | Block Explorer | ✅ |
| QuoterV2 | *See audit report* | Block Explorer | ✅ |
| TickLens | *See audit report* | Block Explorer | ✅ |
| TokenDescriptor | *See audit report* | Block Explorer | ✅ |

## Deployment Information

- **Compiler Version**: Solidity 0.7.6 / 0.8.x
- **Optimization**: Enabled
- **Runs**: 1,000,000 (for core contracts)

## Contract Verification

All contracts have been verified on the block explorer with:
- ✅ Source code published
- ✅ Constructor arguments documented
- ✅ Compiler settings matched
- ✅ Libraries linked correctly

## Upgrade Mechanism

**Note**: PotatoSwap V3 core contracts are **immutable** and **non-upgradeable** by design. This ensures:
- No centralized control over user funds
- Predictable behavior
- Maximum trustlessness

The factory owner has limited privileges:
- Setting protocol fees (capped)
- Enabling fee tiers
- No fund access or parameter changes to existing pools

## Additional Resources

- **Documentation**: [docs.potatoswap.io](https://docs.potatoswap.io)
- **GitHub**: [github.com/potatoswap](https://github.com/potatoswap)
- **Audit Report**: [PotatoSwap_V3_Audit_Report_2025-10-17.pdf](PotatoSwap_V3_Audit_Report_2025-10-17.pdf)

---

*Last Updated: November 3, 2025*

