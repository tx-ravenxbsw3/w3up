# Changelog

## [4.0.0](https://github.com/tx-ravenxbsw3/w3up/compare/filecoin-client-v3.3.5...filecoin-client-v4.0.0) (2025-09-29)


### ⚠ BREAKING CHANGES

* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344))
* upgrade data segment v4 ([#996](https://github.com/tx-ravenxbsw3/w3up/issues/996))

### Features

* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344)) ([db98e3a](https://github.com/tx-ravenxbsw3/w3up/commit/db98e3ad7fd5ce589ab5f002a9e614341f9121ca))
* filecoin info ([#1091](https://github.com/tx-ravenxbsw3/w3up/issues/1091)) ([ad4e328](https://github.com/tx-ravenxbsw3/w3up/commit/ad4e32852f9f804163ef813bae47d2d430b6cac1))
* move aggregate information out of deals in filecoin/info ([#1192](https://github.com/tx-ravenxbsw3/w3up/issues/1192)) ([49e1363](https://github.com/tx-ravenxbsw3/w3up/commit/49e1363925acb1224e62f9ae4e9df4464cf6281d))
* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/tx-ravenxbsw3/w3up/issues/1312)) ([5ed0f70](https://github.com/tx-ravenxbsw3/w3up/commit/5ed0f708d74745ae86c6c69c436a7dffb9c9d7c8))


### Fixes

* filecoin test use blob ([#1422](https://github.com/tx-ravenxbsw3/w3up/issues/1422)) ([bb37641](https://github.com/tx-ravenxbsw3/w3up/commit/bb37641d5641d3bff879187597b02ae3d1e18674))
* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/tx-ravenxbsw3/w3up/issues/1141)) ([93980ef](https://github.com/tx-ravenxbsw3/w3up/commit/93980ef8759b01b689a017aa7ae5a06d83284948))
* migrate repo ([#1389](https://github.com/tx-ravenxbsw3/w3up/issues/1389)) ([9e18c76](https://github.com/tx-ravenxbsw3/w3up/commit/9e18c761e63c88e395b66b4f7cbadc79fc837dec))
* package metadata ([#1161](https://github.com/tx-ravenxbsw3/w3up/issues/1161)) ([68b41e4](https://github.com/tx-ravenxbsw3/w3up/commit/68b41e49f4e77aabe07594b22691b2febdb3ea91))
* receipt chain has wrong CID because no expiration is set ([#1060](https://github.com/tx-ravenxbsw3/w3up/issues/1060)) ([ef4f886](https://github.com/tx-ravenxbsw3/w3up/commit/ef4f8863bd64e0a7941278b850db74efd10b0c7f))
* repo URLs ([#1550](https://github.com/tx-ravenxbsw3/w3up/issues/1550)) ([6fd5aa3](https://github.com/tx-ravenxbsw3/w3up/commit/6fd5aa32e9cfb5633ec662363e6a48493b1f8cf0))
* touch filecoin-client README as fix conventional commits in order to trigger release-please patch version ([372eea6](https://github.com/tx-ravenxbsw3/w3up/commit/372eea63c6aa5c5a26b2a5ce8460bef2f13f143e))
* upgrade data segment v4 ([#996](https://github.com/tx-ravenxbsw3/w3up/issues/996)) ([04b4d1e](https://github.com/tx-ravenxbsw3/w3up/commit/04b4d1e3293dce859a43b433ac76447b4a22b2e0))
* upgrade filecoin client deal tracker principal ([#1092](https://github.com/tx-ravenxbsw3/w3up/issues/1092)) ([7f95439](https://github.com/tx-ravenxbsw3/w3up/commit/7f95439a5dab0c982040110d805733622e4ed44e))
* upgrade ucanto core ([#1127](https://github.com/tx-ravenxbsw3/w3up/issues/1127)) ([40b3257](https://github.com/tx-ravenxbsw3/w3up/commit/40b32571b42ff63f37d5020299ebb013e1886286))
* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/tx-ravenxbsw3/w3up/issues/1359)) ([6ca062f](https://github.com/tx-ravenxbsw3/w3up/commit/6ca062fad73a442b81553fc79fd75923ff9e1bcf))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/tx-ravenxbsw3/w3up/issues/1533)) ([47cc600](https://github.com/tx-ravenxbsw3/w3up/commit/47cc6006b1b7316c6815dfdca0a55122f632fec3))
* **main:** release filecoin-client 2.0.2 ([#1017](https://github.com/tx-ravenxbsw3/w3up/issues/1017)) ([0582bb1](https://github.com/tx-ravenxbsw3/w3up/commit/0582bb11dae2d8261528edac8f241aad0f47e9c6))
* **main:** release filecoin-client 3.0.0 ([#1019](https://github.com/tx-ravenxbsw3/w3up/issues/1019)) ([8514228](https://github.com/tx-ravenxbsw3/w3up/commit/851422827334969a1435aad9d84cbee53e468ca4))
* **main:** release filecoin-client 3.0.1 ([#1062](https://github.com/tx-ravenxbsw3/w3up/issues/1062)) ([07f66b2](https://github.com/tx-ravenxbsw3/w3up/commit/07f66b28ce96298571acd9b3a2556bf002ea07a1))
* **main:** release filecoin-client 3.0.2 ([#1093](https://github.com/tx-ravenxbsw3/w3up/issues/1093)) ([cc9d3dc](https://github.com/tx-ravenxbsw3/w3up/commit/cc9d3dc86bdcac9a218c4ad73197093c60cc48ef))
* **main:** release filecoin-client 3.1.0 ([#1097](https://github.com/tx-ravenxbsw3/w3up/issues/1097)) ([af7257c](https://github.com/tx-ravenxbsw3/w3up/commit/af7257c35816428e9d184e16fae9a4e7a2c463ce))
* **main:** release filecoin-client 3.1.1 ([#1130](https://github.com/tx-ravenxbsw3/w3up/issues/1130)) ([66b391b](https://github.com/tx-ravenxbsw3/w3up/commit/66b391bea534e1c979b46808f34aff1508fd98b6))
* **main:** release filecoin-client 3.1.2 ([#1146](https://github.com/tx-ravenxbsw3/w3up/issues/1146)) ([2bf2095](https://github.com/tx-ravenxbsw3/w3up/commit/2bf2095f3247232bddb9870edf724b2e1bedaf60))
* **main:** release filecoin-client 3.1.3 ([#1162](https://github.com/tx-ravenxbsw3/w3up/issues/1162)) ([9ccf320](https://github.com/tx-ravenxbsw3/w3up/commit/9ccf3203a35c924f6663f064375096af919447a0))
* **main:** release filecoin-client 3.2.0 ([#1197](https://github.com/tx-ravenxbsw3/w3up/issues/1197)) ([e878326](https://github.com/tx-ravenxbsw3/w3up/commit/e8783262e79e4d6d5bc1e5dbf01b09ed47e388ff))
* **main:** release filecoin-client 3.3.0 ([#1317](https://github.com/tx-ravenxbsw3/w3up/issues/1317)) ([de5ea0e](https://github.com/tx-ravenxbsw3/w3up/commit/de5ea0e3f6e030290fd624659b69eeb6d1477c14))
* **main:** release filecoin-client 3.3.1 ([#1361](https://github.com/tx-ravenxbsw3/w3up/issues/1361)) ([4c9410a](https://github.com/tx-ravenxbsw3/w3up/commit/4c9410a7dfe5176718695fc9d2a4ae44ff2aa858))
* **main:** release filecoin-client 3.3.2 ([#1397](https://github.com/tx-ravenxbsw3/w3up/issues/1397)) ([a23f5a8](https://github.com/tx-ravenxbsw3/w3up/commit/a23f5a8d7b9b3fcd04aa9428f3b1e3829ebb6799))
* **main:** release filecoin-client 3.3.3 ([#1423](https://github.com/tx-ravenxbsw3/w3up/issues/1423)) ([25f65c0](https://github.com/tx-ravenxbsw3/w3up/commit/25f65c07497e9dbb3cf73242811bbaecebe20d52))
* **main:** release filecoin-client 3.3.4 ([#1539](https://github.com/tx-ravenxbsw3/w3up/issues/1539)) ([b817d1f](https://github.com/tx-ravenxbsw3/w3up/commit/b817d1fe63fcb45dcd6c28f39dedaac2d20f2e19))
* **main:** release filecoin-client 3.3.5 ([#1579](https://github.com/tx-ravenxbsw3/w3up/issues/1579)) ([514cac5](https://github.com/tx-ravenxbsw3/w3up/commit/514cac594cf83957bf07e0a6ec47bedd9fc571e2))
* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/tx-ravenxbsw3/w3up/issues/1577)) ([bdaa5e2](https://github.com/tx-ravenxbsw3/w3up/commit/bdaa5e297fef7e7ddca6a63c12ab071000cc7d2b))
* no longer depends on hd-scripts, packages use/configure eslint directly, fixes warnings from npm lint script ([#1058](https://github.com/tx-ravenxbsw3/w3up/issues/1058)) ([3a99cc0](https://github.com/tx-ravenxbsw3/w3up/commit/3a99cc02941f9d563cac1838e1e67a3faa42c3de))

## [3.3.5](https://github.com/storacha/w3up/compare/filecoin-client-v3.3.4...filecoin-client-v3.3.5) (2024-12-09)


### Other Changes

* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/storacha/w3up/issues/1577)) ([1482d69](https://github.com/storacha/w3up/commit/1482d69c28baff1c27b1baf5f3e5c76f844e5576))

## [3.3.4](https://github.com/storacha/w3up/compare/filecoin-client-v3.3.3...filecoin-client-v3.3.4) (2024-09-23)


### Fixes

* repo URLs ([#1550](https://github.com/storacha/w3up/issues/1550)) ([e02ddf3](https://github.com/storacha/w3up/commit/e02ddf3696553b03f8d2f7316de0a99a9303a60f))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/storacha/w3up/issues/1533)) ([07970ef](https://github.com/storacha/w3up/commit/07970efd443149158ebbfb2c4e745b5007eb9407))

## [3.3.3](https://github.com/w3s-project/w3up/compare/filecoin-client-v3.3.2...filecoin-client-v3.3.3) (2024-04-30)


### Fixes

* filecoin test use blob ([#1422](https://github.com/w3s-project/w3up/issues/1422)) ([359c0b7](https://github.com/w3s-project/w3up/commit/359c0b736cad8e4375d75af4f60e97e20057e7aa))

## [3.3.2](https://github.com/w3s-project/w3up/compare/filecoin-client-v3.3.1...filecoin-client-v3.3.2) (2024-04-24)


### Fixes

* migrate repo ([#1389](https://github.com/w3s-project/w3up/issues/1389)) ([475a287](https://github.com/w3s-project/w3up/commit/475a28743ff9f7138b46dfe4227d3c80ed75a6a2))

## [3.3.1](https://github.com/web3-storage/w3up/compare/filecoin-client-v3.3.0...filecoin-client-v3.3.1) (2024-04-12)


### Fixes

* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/web3-storage/w3up/issues/1359)) ([87ca098](https://github.com/web3-storage/w3up/commit/87ca098186fe204ff3409a2684719f1c54148c97))

## [3.3.0](https://github.com/web3-storage/w3up/compare/filecoin-client-v3.2.0...filecoin-client-v3.3.0) (2024-03-21)


### Features

* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/web3-storage/w3up/issues/1312)) ([d6978d7](https://github.com/web3-storage/w3up/commit/d6978d7ab299be76987c6533d18e6857f6998fe6))

## [3.2.0](https://github.com/web3-storage/w3up/compare/filecoin-client-v3.1.3...filecoin-client-v3.2.0) (2023-11-29)


### Features

* move aggregate information out of deals in filecoin/info ([#1192](https://github.com/web3-storage/w3up/issues/1192)) ([18dc590](https://github.com/web3-storage/w3up/commit/18dc590ad50a023ef3094bfc1a2d729459e5d68e))

## [3.1.3](https://github.com/web3-storage/w3up/compare/filecoin-client-v3.1.2...filecoin-client-v3.1.3) (2023-11-28)


### Fixes

* package metadata ([#1161](https://github.com/web3-storage/w3up/issues/1161)) ([b8a1cc2](https://github.com/web3-storage/w3up/commit/b8a1cc2e125a91be582998bda295e1ae1caab087))

## [3.1.2](https://github.com/web3-storage/w3up/compare/filecoin-client-v3.1.1...filecoin-client-v3.1.2) (2023-11-16)


### Bug Fixes

* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/web3-storage/w3up/issues/1141)) ([0b8d3f3](https://github.com/web3-storage/w3up/commit/0b8d3f3b52918b1b4d3b76ea6fea3fb0c837cd73))

## [3.1.1](https://github.com/web3-storage/w3up/compare/filecoin-client-v3.1.0...filecoin-client-v3.1.1) (2023-11-15)


### Bug Fixes

* upgrade ucanto core ([#1127](https://github.com/web3-storage/w3up/issues/1127)) ([5ce4d22](https://github.com/web3-storage/w3up/commit/5ce4d2292d7e980da4a2ea0f1583f608a81157d2))

## [3.1.0](https://github.com/web3-storage/w3up/compare/filecoin-client-v3.0.2...filecoin-client-v3.1.0) (2023-11-08)


### Features

* filecoin info ([#1091](https://github.com/web3-storage/w3up/issues/1091)) ([adb2442](https://github.com/web3-storage/w3up/commit/adb24424d1faf50daf2339b77c22fdd44faa236a))

## [3.0.2](https://github.com/web3-storage/w3up/compare/filecoin-client-v3.0.1...filecoin-client-v3.0.2) (2023-11-08)


### Bug Fixes

* upgrade filecoin client deal tracker principal ([#1092](https://github.com/web3-storage/w3up/issues/1092)) ([cde7113](https://github.com/web3-storage/w3up/commit/cde71134ab8fdd4a72e3764da30ae0a414a8690b))

## [3.0.1](https://github.com/web3-storage/w3up/compare/filecoin-client-v3.0.0...filecoin-client-v3.0.1) (2023-11-03)


### Bug Fixes

* receipt chain has wrong CID because no expiration is set ([#1060](https://github.com/web3-storage/w3up/issues/1060)) ([dfb46d8](https://github.com/web3-storage/w3up/commit/dfb46d8185c684a18452e1325abcf74d59c48159))

## [3.0.0](https://github.com/web3-storage/w3up/compare/filecoin-client-v2.0.2...filecoin-client-v3.0.0) (2023-10-26)


### ⚠ BREAKING CHANGES

* upgrade data segment v4 ([#996](https://github.com/web3-storage/w3up/issues/996))

### Bug Fixes

* upgrade data segment v4 ([#996](https://github.com/web3-storage/w3up/issues/996)) ([348e4b0](https://github.com/web3-storage/w3up/commit/348e4b065909e48ab1e97c0eaee9fa0b5ad2e223))

## [2.0.2](https://github.com/web3-storage/w3up/compare/filecoin-client-v2.0.1...filecoin-client-v2.0.2) (2023-10-25)


### Bug Fixes

* touch filecoin-client README as fix conventional commits in order to trigger release-please patch version ([65245ef](https://github.com/web3-storage/w3up/commit/65245effd6c7e06c4d3b495e03a598e557a98c8e))

## [2.0.1](https://github.com/web3-storage/w3up/compare/filecoin-client-v2.0.0...filecoin-client-v2.0.1) (2023-10-25)


### Bug Fixes

* fix arethetypesworking errors in all packages ([#1004](https://github.com/web3-storage/w3up/issues/1004)) ([2e2936a](https://github.com/web3-storage/w3up/commit/2e2936a3831389dd13be5be5146a04e2b15553c5))
* package.json files excludes 'src' and includes .js and .js.map in dist for packages that now export their module from dist  ([#1012](https://github.com/web3-storage/w3up/issues/1012)) ([d2537de](https://github.com/web3-storage/w3up/commit/d2537deed533a39f39e312a1dfcfbd048e1d83e5))

## [2.0.0](https://github.com/web3-storage/w3up/compare/filecoin-client-v1.4.0...filecoin-client-v2.0.0) (2023-10-24)


### ⚠ BREAKING CHANGES

* see latest specs https://github.com/web3-storage/specs/blob/cbdb706f18567900c5c24d7fb16ccbaf93d0d023/w3-filecoin.md
* filecoin client to use new capabilities

### Bug Fixes

* client tests ([b0d9c3f](https://github.com/web3-storage/w3up/commit/b0d9c3f258d37701487ef02f70a93e2dd1a18775))
* upgrade ucanto in filecoin api ([c95fb54](https://github.com/web3-storage/w3up/commit/c95fb54cdb04f50ff78e5113e70d73c1cd6d8b47))


### Code Refactoring

* filecoin api services events and tests ([#974](https://github.com/web3-storage/w3up/issues/974)) ([953537b](https://github.com/web3-storage/w3up/commit/953537bcb98d94b9e9655797a7f9026643ab949f))
* filecoin client to use new capabilities ([b0d9c3f](https://github.com/web3-storage/w3up/commit/b0d9c3f258d37701487ef02f70a93e2dd1a18775))

## [1.4.0](https://github.com/web3-storage/w3up/compare/filecoin-client-v1.3.0...filecoin-client-v1.4.0) (2023-10-11)


### Features

* upgrade to ucanto@9 ([#951](https://github.com/web3-storage/w3up/issues/951)) ([d72faf1](https://github.com/web3-storage/w3up/commit/d72faf1bb07dd11462ae6dff8ee0469f8ae7e9e7))


### Bug Fixes

* upgrade to latest ts ([#962](https://github.com/web3-storage/w3up/issues/962)) ([711e3f7](https://github.com/web3-storage/w3up/commit/711e3f73f6905fde0d929952fff70be845a55fa1))

## [1.3.0](https://github.com/web3-storage/w3up/compare/filecoin-client-v1.2.2...filecoin-client-v1.3.0) (2023-08-30)


### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))


### Bug Fixes

* upgrade data segment ([#850](https://github.com/web3-storage/w3up/issues/850)) ([fba281f](https://github.com/web3-storage/w3up/commit/fba281f8cd3ce2a0a00ffd50a4a73d7701b489ce))
* w3filecoin spec separate capabilities to queue and enqueue ([#856](https://github.com/web3-storage/w3up/issues/856)) ([6bf9142](https://github.com/web3-storage/w3up/commit/6bf9142636fa65367faed8414c50beb9c1791726)), closes [#855](https://github.com/web3-storage/w3up/issues/855)

## [1.2.1](https://github.com/web3-storage/w3up/compare/filecoin-client-v1.2.0...filecoin-client-v1.2.1) (2023-08-30)


### Bug Fixes

* w3filecoin spec separate capabilities to queue and enqueue ([#856](https://github.com/web3-storage/w3up/issues/856)) ([6bf9142](https://github.com/web3-storage/w3up/commit/6bf9142636fa65367faed8414c50beb9c1791726)), closes [#855](https://github.com/web3-storage/w3up/issues/855)

## [1.2.0](https://github.com/web3-storage/w3up/compare/filecoin-client-v1.1.0...filecoin-client-v1.2.0) (2023-08-10)


### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))


### Bug Fixes

* upgrade data segment ([#850](https://github.com/web3-storage/w3up/issues/850)) ([fba281f](https://github.com/web3-storage/w3up/commit/fba281f8cd3ce2a0a00ffd50a4a73d7701b489ce))

## 1.0.0 (2023-08-10)


### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))


### Bug Fixes

* upgrade data segment ([#850](https://github.com/web3-storage/w3up/issues/850)) ([fba281f](https://github.com/web3-storage/w3up/commit/fba281f8cd3ce2a0a00ffd50a4a73d7701b489ce))

## [1.1.0](https://github.com/web3-storage/w3up/compare/filecoin-client-v1.0.0...filecoin-client-v1.1.0) (2023-08-09)


### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))
