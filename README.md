# TokenVesting Smart Contract

## Overview

`TokenVesting` is a Solidity smart contract that implements a standard token vesting mechanism. It allows tokens to be gradually released to a beneficiary address based on a cliff and vesting period. The vesting can optionally be revoked by the contract owner.

This contract is designed for use with ERC20-compatible tokens and ensures secure token distribution over time for investors, teams, or stakeholders.

---

## Features

- **Linear Vesting**: Gradual release of tokens over a specified duration.
- **Cliff Period**: Tokens cannot be released until the cliff time has passed.
- **Revocable Vesting**: Owner can revoke the vesting if allowed.
- **ERC20 Compatible**: Uses SafeERC20 for secure token transfers.

---

## Constructor Parameters

| Parameter        | Description                                           |
|------------------|-------------------------------------------------------|
| `beneficiary`    | Address of the beneficiary receiving the tokens       |
| `start`          | Vesting start time (Unix timestamp)                  |
| `cliffDuration`  | Duration of the cliff in seconds                      |
| `duration`       | Total vesting duration in seconds                     |
| `revocable`      | Boolean flag to allow revocation                      |

---

## Main Functions

| Function         | Description                                           |
|------------------|-------------------------------------------------------|
| `release(token)` | Transfers vested tokens to the beneficiary            |
| `revoke(token)`  | Allows the owner to revoke unvested tokens            |
| `beneficiary()`  | Returns the beneficiary address                       |
| `cliff()`        | Returns the cliff timestamp                           |
| `start()`        | Returns the start timestamp                           |
| `duration()`     | Returns the total duration                            |
| `revocable()`    | Returns true if vesting is revocable                  |
| `released(token)`| Returns amount of token already released              |
| `revoked(token)` | Returns true if the token has been revoked            |

---

## Flowchart

A detailed **flowchart** of the smart contract logic has been created to visualize:

- Contract initialization
- Token vesting flow
- Releasing and revoking logic
- Time-based condition branches


## Prerequisites

- Solidity compiler (`^0.4.24`)
- Remix IDE

---

## Installation

```bash
git clone https://github.com/your-username/token-vesting.git
```

##TEAM
Yehia Tarek - 
Sara Hendy - 
Shadwa Ahmed - 
Basel Yasser


MIT License © 2025 Yehia Tarek
