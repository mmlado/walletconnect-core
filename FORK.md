# @walletconnect/core 2.21.7, telemetry off means off

The first commit is the package as published on npm, unchanged:
`npm pack @walletconnect/core@2.21.7` gives the same files (integrity
`sha512-q/Au5Ne3g4R+q4GvHR5cvRd3+ha00QZCZiCs058lmy+eDbiZd0YsautvTPJ5a2guD6UaS1k/w5e1JHgixdcgLA==`).

The second commit changes one condition in each of `dist/index.cjs.js`, `dist/index.es.js` and
`dist/index.umd.js`: `EventClient.init` sends its `INIT` event only when `telemetryEnabled` is
true. Published 2.21.7 sends it whatever `telemetryEnabled` says.

The package stays at 2.21.7 under Apache-2.0. Nothing else differs from the published release.
