# PotatoSwap V2 - Deployed Contracts

## Mainnet Deployment

### Core Contracts

| Contract | Address | Explorer | Verified |
|----------|---------|----------|----------|
| HyperindexV2Factory | *See audit report* | Block Explorer | ✅ |
| HyperindexV2Router02 | *See audit report* | Block Explorer | ✅ |

### Example Trading Pairs

Trading pairs are created permissionlessly through the factory contract. Major pairs include:
- POTATO/WETH
- USDC/WETH
- USDT/USDC

All pair contracts use the same verified template deployed through the factory.

## Deployment Information

- **Compiler Version**: Solidity 0.6.x / 0.8.x
- **Optimization**: Enabled
- **Runs**: 200

## Contract Verification

All contracts have been verified on the block explorer with:
- ✅ Source code published
- ✅ Constructor arguments documented
- ✅ Compiler settings matched
- ✅ Libraries linked correctly

## Upgrade Mechanism

**Non-upgradeable** - Core AMM contracts (Factory, Pairs, Router) are immutable to ensure trustlessness and maximum security.

## Contract Ownership

### Factory Owner Capabilities
- Create new pairs (permissionless)
- Set protocol fee recipient
- Enable/disable protocol fees

### Router Capabilities
- No owner privileges
- Stateless contract
- Permissionless usage

## V2 vs V3

| Feature | V2 | V3 |
|---------|----|----|
| Liquidity Model | Full range (x*y=k) | Concentrated |
| Capital Efficiency | Standard | High |
| Position Management | Fungible LP tokens | NFT positions |
| Fee Tiers | Fixed (0.3%) | Multiple tiers |
| Active Development | Maintenance | Active |

## Additional Resources

- **Documentation**: [docs.potatoswap.io/v2](https://docs.potatoswap.io/v2)
- **GitHub**: [github.com/potatoswap](https://github.com/potatoswap)
- **Audit Report**: [PotatoSwap_V2_Core_Blocksec.pdf](PotatoSwap_V2_Core_Blocksec.pdf)

---

*Last Updated: November 3, 2025*

