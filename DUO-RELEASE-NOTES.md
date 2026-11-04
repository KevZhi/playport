# Playport for iPhone Duo — community test build

An unsigned IPA built from De-Os's iPhone Duo patch, shared by KevZhi so other Duo users can test without compiling Playport themselves.

## Device test

KevZhi confirms that the app installs, launches and reaches its main screen on an iPhone Duo running iOS 27.3. No game has been tested. JIT readiness, gameplay, performance, folding/rotation and virtual-controller behavior have not been verified by KevZhi.

## Download and install

Download **Playport-Duo-unsigned.ipa** below. This is an unsigned community build: sign it with your own Apple account and a sideloading tool that preserves the **Increased Memory Limit** entitlement and the **PlayportJIT app extension**. Do not remove the extension.

Enable Developer Mode on your iPhone. For the built-in JIT method, install LocalDevVPN from the App Store, allow its VPN configuration, connect it, and follow Playport's on-device pairing/setup instructions. A paid developer account alone does not activate JIT. See the bundled INSTALL-REBUILD.md and the source's docs/DEVICE.md.

## Build and attribution

- Original project: https://github.com/playportdev/playport
- iPhone Duo patch author: **De-Os** — https://github.com/playportdev/playport/pull/83
- Exact application source: `f7e27d14fd08ab289511df8bf79649785086d361`
- Binary build: https://github.com/KevZhi/playport/actions/runs/41866894102
- Build workflow revision: `a31f2c47598817815890d93b85cd9aadf2b9c277`
- Built using Xcode / iOS SDK 27.1. The Xcode Release configuration produced the author's **development app variant (S1Probe.app)**; this is not the upstream release variant.
- Unsigned IPA SHA-256: `0204ced6cead7297b4e6a01095ccc0f3d3c60a38bbcd6e280eb52fa72a868a29`

This is an **unofficial experimental prerelease**, not an upstream Playport release or a new patch authored by KevZhi. Thanks to De-Os and the Playport contributors.

## Source and licenses

The matching Corresponding Source bundle(s), component manifest, notices, build workflow and rebuild instructions are attached alongside the IPA. Third-party components retain their respective licenses. The source archive is split only if required by GitHub's asset size limit; reassemble numbered parts with `cat Playport-Duo-source.tar.part-* > Playport-Duo-source.tar`, then extract the tar archive. Compare downloaded files against SHA256SUMS.

Only the unsigned IPA is shared. No personal development certificate, provisioning profile, device pairing record, Apple SDK archive, game, or account session is included.
