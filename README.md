 Highly-leveraged Basis Fund(HLBF) Smart Contracts

This repository contains the smart contracts for HLBF on EVM-compatible blockchains. HLBF is a money-market fund adopting leveraged basis trading strategy.

## Core Contracts

### MMFManager
The main contract that handles fund operations including:
- Subscription: Users can deposit stable coins to receive fund tokens
- Redemption: Users can burn fund tokens to receive stable coins
- Price oracle integration for token valuations
- Fee management for fund operations
- Support for both instant and delayed settlement

### FundToken
An ERC20-compliant token that represents shares in the fund:
- Implements minting and burning capabilities
- Controlled access through minter/burner roles
- Upgradeable using UUPS pattern
- Configurable decimals

### RolesAuthority
A role-based access control (RBAC) system that manages permissions:
- Supports up to 256 different roles
- Granular capability management per role
- Public and role-restricted function access
- Emergency pause functionality
- Upgradeable using UUPS pattern

