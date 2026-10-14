# IPA Signer Local

Local-only Next.js prototype for basic IPA and signing-asset upload checks.

## Requirements

- macOS on Apple Silicon or Intel
- Node.js 20.9+ (Node 22 LTS is a good choice)

## Install

```bash
npm install
npm run dev
```

Open http://127.0.0.1:3000.

## Important limitations

This is a UI and basic file-inspection prototype. It does **not**:
- validate Apple certificate revocation status
- decrypt or validate the P12 certificate/password
- parse or validate the mobile provisioning profile
- sign, re-sign, or export an IPA

Never upload private keys or certificate passwords to a service you do not control. Use only signing assets you are authorized to use. Do not expose this dev server to a public network.
