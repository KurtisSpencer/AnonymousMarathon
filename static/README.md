# Anonymous Marathon Registration System

A privacy-first marathon registration and management platform built with Fully Homomorphic Encryption (FHE) using Zama's fhEVM.

## Features

- **Anonymous Registration**: Runners can register with encrypted personal data (age, experience, previous times)
- **Privacy Protection**: All sensitive data is encrypted using FHE technology
- **Real-time Leaderboards**: View race results while maintaining participant privacy
- **Smart Prize Distribution**: Automatic prize distribution to winners
- **Zero Dependencies**: Pure static HTML/CSS/JS with CDN-loaded libraries

## Deployment

### Vercel Deployment

1. Connect your GitHub repository to Vercel
2. Set the root directory to `static/`
3. Deploy automatically

### Manual Deployment

1. Upload all files in the `static/` directory to your web server
2. Update `CONTRACT_ADDRESS` in `app.js` with your deployed contract address
3. Ensure your web server serves static files

## Smart Contract

The system uses the `AnonymousMarathon.sol` contract which provides:

- Marathon creation and management
- Encrypted participant registration
- Privacy-preserving leaderboards
- Automatic prize distribution

### Contract Functions

- `createMarathon()`: Create new marathon events
- `registerForMarathon()`: Register with encrypted data
- `getMarathonInfo()`: Get marathon details
- `getLeaderboard()`: View race results

## Usage

1. **Organizers**: Create marathons with event details
2. **Runners**: Register anonymously with encrypted personal data
3. **Results**: View leaderboards with privacy protection
4. **Prizes**: Automatic distribution to top finishers

## Technology Stack

- **Frontend**: Pure HTML/CSS/JavaScript
- **Blockchain**: Ethereum/Polygon/Sepolia
- **Privacy**: Zama fhEVM (Fully Homomorphic Encryption)
- **Wallet**: MetaMask integration
- **Deployment**: Vercel-ready static files

## Setup Instructions

1. Deploy the smart contract to your chosen network
2. Update `CONTRACT_ADDRESS` in `app.js`
3. Deploy the static files to Vercel or any static hosting service
4. Connect with MetaMask to interact with the application

## Privacy Features

- Age, experience level, and previous times are encrypted
- Anonymous IDs protect participant identity
- Race times remain encrypted until official results
- No personal data is stored in plaintext

## Browser Support

- Chrome/Chromium (recommended)
- Firefox
- Safari
- Edge

Requires MetaMask or compatible Web3 wallet.