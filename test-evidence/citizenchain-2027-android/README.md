# CitizenChain Android network-icon QA

Verified on 2026-11-02 using MetaMask Mobile 8.20.0, ARM64 main/dev Release, from PR #38615 source commit 7c9c7ebe6f95c48ef47f656a2cc7e56282fd33dd. The isolated Android emulator runs API 36.1.

Network: CitizenChain; RPC https://nrcrpc.crcfrcn.com/; chain ID 2027 (0x7eb); symbol GMB. The endpoint returned 0x7eb for eth_chainId.

Actual UI checks passed:
- Settings/Networks shows the CitizenChain logo in the saved custom-network row (network-list.png).
- Tokens/Networks/Custom shows the CitizenChain logo in the selector (selector.png).
- Selecting CitizenChain shows the logo in the selected-network control and the GMB network badge.
- Switching to Ethereum and back preserves both CitizenChain network images (selected.png).

These are original emulator PNG captures exported through Android Studio, without image editing. The wallet was newly created for this test and had no funds; no transaction was signed or submitted. iOS and Chrome wallet UI are not covered by these captures.

APK SHA-256: 46500679863606ae6134dbc8f66b6c895f3fb250cebb4b09752fd932a41777b9.
