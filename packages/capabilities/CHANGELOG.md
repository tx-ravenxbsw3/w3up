# Changelog

## [19.0.0](https://github.com/tx-ravenxbsw3/w3up/compare/capabilities-v18.1.0...capabilities-v19.0.0) (2025-09-29)


### ⚠ BREAKING CHANGES

* content serve authorization ([#1590](https://github.com/tx-ravenxbsw3/w3up/issues/1590))
* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344))
* add `index/add` handler ([#1421](https://github.com/tx-ravenxbsw3/w3up/issues/1421))
* restrict store API to CARs ([#1415](https://github.com/tx-ravenxbsw3/w3up/issues/1415))
* **capabilities:** `BlobMultihash` type in `@web3-storage/capabilities` renamed to `Multihash`.
* allocations storage interface now requires remove to be implemented
* return allocated bytes in `store/add` receipt ([#1213](https://github.com/tx-ravenxbsw3/w3up/issues/1213))
* coupon ([#1136](https://github.com/tx-ravenxbsw3/w3up/issues/1136))

### Features

* add "plan/create-admin-session" capability ([#1411](https://github.com/tx-ravenxbsw3/w3up/issues/1411)) ([d9662c7](https://github.com/tx-ravenxbsw3/w3up/commit/d9662c75dd138be02213931be3c8b59f08f26ad1))
* add `index/add` handler ([#1421](https://github.com/tx-ravenxbsw3/w3up/issues/1421)) ([e2eb8a7](https://github.com/tx-ravenxbsw3/w3up/commit/e2eb8a7232116c0f4169adc1e4aaf82b60daf086))
* add `initialize` method to `PlansStorage` ([#1278](https://github.com/tx-ravenxbsw3/w3up/issues/1278)) ([4ee293a](https://github.com/tx-ravenxbsw3/w3up/commit/4ee293a5d34ce9cec2a71a71e825c8e7cd00936e))
* add `subscription/list` capability ([#1088](https://github.com/tx-ravenxbsw3/w3up/issues/1088)) ([dd2c715](https://github.com/tx-ravenxbsw3/w3up/commit/dd2c715b6b3004425273d15e3a9eaa3d2f25673a))
* add a function to verify and return Abilities. ([#1252](https://github.com/tx-ravenxbsw3/w3up/issues/1252)) ([99479ec](https://github.com/tx-ravenxbsw3/w3up/commit/99479ecae8640524f798e9ad64a688ff01df7f1b))
* add blob list and remove ([#1385](https://github.com/tx-ravenxbsw3/w3up/issues/1385)) ([b4e8b40](https://github.com/tx-ravenxbsw3/w3up/commit/b4e8b401cb614e86ba636a12118c5fbf32cb5f7c))
* add blob protocol to upload-client ([#1425](https://github.com/tx-ravenxbsw3/w3up/issues/1425)) ([44bde76](https://github.com/tx-ravenxbsw3/w3up/commit/44bde7616adc94f82cfef751bcaa94cf59bf24c5))
* add blob/get ([#1484](https://github.com/tx-ravenxbsw3/w3up/issues/1484)) ([9f774cc](https://github.com/tx-ravenxbsw3/w3up/commit/9f774ccb847b0e1182b6d9a0a1ff13db03253800))
* add usage/report capability ([#1079](https://github.com/tx-ravenxbsw3/w3up/issues/1079)) ([95db863](https://github.com/tx-ravenxbsw3/w3up/commit/95db8632ce796ff698d7b016cca6e676e846eeac))
* blob, web3.storage and ucan conclude capabilities together with api handlers  ([#1342](https://github.com/tx-ravenxbsw3/w3up/issues/1342)) ([d702ecb](https://github.com/tx-ravenxbsw3/w3up/commit/d702ecb10f87159fb50bcf0b7693ec2b3d9447d4))
* **capabilities:** add `index/add` capability ([#1410](https://github.com/tx-ravenxbsw3/w3up/issues/1410)) ([4d92f6d](https://github.com/tx-ravenxbsw3/w3up/commit/4d92f6d4209338b189e883016badef2c20784944))
* change `plan/update` to `plan/set` and use existing `PlansStorage#set` to implement an invocation handler ([#1258](https://github.com/tx-ravenxbsw3/w3up/issues/1258)) ([e2b840a](https://github.com/tx-ravenxbsw3/w3up/commit/e2b840a67092dbc1b1f1dd88808a23804086ba8c))
* content serve authorization ([#1590](https://github.com/tx-ravenxbsw3/w3up/issues/1590)) ([c752277](https://github.com/tx-ravenxbsw3/w3up/commit/c752277cc07008437fc4482ea5689a1cabc92abf))
* coupon ([#1136](https://github.com/tx-ravenxbsw3/w3up/issues/1136)) ([c41320d](https://github.com/tx-ravenxbsw3/w3up/commit/c41320d6fccaa4b9fac924acae3259fd1df142e9))
* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344)) ([db98e3a](https://github.com/tx-ravenxbsw3/w3up/commit/db98e3ad7fd5ce589ab5f002a9e614341f9121ca))
* external login ([#1629](https://github.com/tx-ravenxbsw3/w3up/issues/1629)) ([638c31c](https://github.com/tx-ravenxbsw3/w3up/commit/638c31c5ae06fa73264b2fa45cd223fc2f7cc704))
* filecoin info ([#1091](https://github.com/tx-ravenxbsw3/w3up/issues/1091)) ([ad4e328](https://github.com/tx-ravenxbsw3/w3up/commit/ad4e32852f9f804163ef813bae47d2d430b6cac1))
* Generate Space proofs on the fly, on `access/claim` ([#1555](https://github.com/tx-ravenxbsw3/w3up/issues/1555)) ([45ea3e9](https://github.com/tx-ravenxbsw3/w3up/commit/45ea3e9d9ecb4285fa22fc45055c12196e1e476b))
* implement `plan/get` capability ([#1005](https://github.com/tx-ravenxbsw3/w3up/issues/1005)) ([d572f37](https://github.com/tx-ravenxbsw3/w3up/commit/d572f374c0e8a3ef1968ac14dff6632512cd2f12))
* introduce capability for changing billing plan ([#1253](https://github.com/tx-ravenxbsw3/w3up/issues/1253)) ([7366244](https://github.com/tx-ravenxbsw3/w3up/commit/73662444117378d8798eb814f8b5cbfd46b099c0))
* move aggregate information out of deals in filecoin/info ([#1192](https://github.com/tx-ravenxbsw3/w3up/issues/1192)) ([49e1363](https://github.com/tx-ravenxbsw3/w3up/commit/49e1363925acb1224e62f9ae4e9df4464cf6281d))
* publish index claim ([#1487](https://github.com/tx-ravenxbsw3/w3up/issues/1487)) ([6de2ba8](https://github.com/tx-ravenxbsw3/w3up/commit/6de2ba837e04f371a319be90a588b00608846b57))
* restrict store API to CARs ([#1415](https://github.com/tx-ravenxbsw3/w3up/issues/1415)) ([4a8bdb6](https://github.com/tx-ravenxbsw3/w3up/commit/4a8bdb69c4c7edec121ee4b53374cc30c5ee81b3))
* return allocated bytes in `store/add` receipt ([#1213](https://github.com/tx-ravenxbsw3/w3up/issues/1213)) ([a243e22](https://github.com/tx-ravenxbsw3/w3up/commit/a243e221153a8107ad92218f545d20ab1b3bd120))
* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/tx-ravenxbsw3/w3up/issues/1312)) ([5ed0f70](https://github.com/tx-ravenxbsw3/w3up/commit/5ed0f708d74745ae86c6c69c436a7dffb9c9d7c8))
* usage/record capability definition ([#1562](https://github.com/tx-ravenxbsw3/w3up/issues/1562)) ([0cb6af9](https://github.com/tx-ravenxbsw3/w3up/commit/0cb6af9ac0954e3d9ee24f63ed86a5cfa1312ef0))


### Fixes

* capabilities should export blob caps ([#1376](https://github.com/tx-ravenxbsw3/w3up/issues/1376)) ([6d9771e](https://github.com/tx-ravenxbsw3/w3up/commit/6d9771e58937960ba4760acdd5a49280d2b52c94))
* **egress/record:** rename capability ([#1572](https://github.com/tx-ravenxbsw3/w3up/issues/1572)) ([9cb5261](https://github.com/tx-ravenxbsw3/w3up/commit/9cb5261de19cb22109f03e9695adbf08b651cd63))
* **egressRecord:** Remove unnecessary multiplication for ts conversion ([#1588](https://github.com/tx-ravenxbsw3/w3up/issues/1588)) ([5609fa9](https://github.com/tx-ravenxbsw3/w3up/commit/5609fa905513806de38b9cc9db4cfce789de2070))
* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/tx-ravenxbsw3/w3up/issues/1141)) ([93980ef](https://github.com/tx-ravenxbsw3/w3up/commit/93980ef8759b01b689a017aa7ae5a06d83284948))
* migrate repo ([#1389](https://github.com/tx-ravenxbsw3/w3up/issues/1389)) ([9e18c76](https://github.com/tx-ravenxbsw3/w3up/commit/9e18c761e63c88e395b66b4f7cbadc79fc837dec))
* one more tweak to the `PlanStorage` interface ([#1280](https://github.com/tx-ravenxbsw3/w3up/issues/1280)) ([9dabd5b](https://github.com/tx-ravenxbsw3/w3up/commit/9dabd5b4118cb58ffe9897630ab9251ac9dc21d2))
* package metadata ([#1161](https://github.com/tx-ravenxbsw3/w3up/issues/1161)) ([68b41e4](https://github.com/tx-ravenxbsw3/w3up/commit/68b41e49f4e77aabe07594b22691b2febdb3ea91))
* put access.session back ([#1100](https://github.com/tx-ravenxbsw3/w3up/issues/1100)) ([747c305](https://github.com/tx-ravenxbsw3/w3up/commit/747c30553e106b81e7b80d857486d199980282af))
* rename blob and index client capabilities ([#1478](https://github.com/tx-ravenxbsw3/w3up/issues/1478)) ([ee5a89c](https://github.com/tx-ravenxbsw3/w3up/commit/ee5a89cac2248e634bd4e835270d052cdbb31aef))
* repo URLs ([#1550](https://github.com/tx-ravenxbsw3/w3up/issues/1550)) ([6fd5aa3](https://github.com/tx-ravenxbsw3/w3up/commit/6fd5aa32e9cfb5633ec662363e6a48493b1f8cf0))
* trigger capabilities release ([#1399](https://github.com/tx-ravenxbsw3/w3up/issues/1399)) ([1b664cb](https://github.com/tx-ravenxbsw3/w3up/commit/1b664cb4cd4df07fbe315df74de82140e48dd8e2))
* update data-segment dep ([d380b33](https://github.com/tx-ravenxbsw3/w3up/commit/d380b33dbb63af83bc173ed10015debf1e1ff1e4))
* upgrade @ucanto/validator with bugfix ([#1151](https://github.com/tx-ravenxbsw3/w3up/issues/1151)) ([34e6f87](https://github.com/tx-ravenxbsw3/w3up/commit/34e6f87747809083388354926c606d8fbbd3db95))
* upgrade ucanto core ([#1127](https://github.com/tx-ravenxbsw3/w3up/issues/1127)) ([40b3257](https://github.com/tx-ravenxbsw3/w3up/commit/40b32571b42ff63f37d5020299ebb013e1886286))
* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/tx-ravenxbsw3/w3up/issues/1359)) ([6ca062f](https://github.com/tx-ravenxbsw3/w3up/commit/6ca062fad73a442b81553fc79fd75923ff9e1bcf))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/tx-ravenxbsw3/w3up/issues/1533)) ([47cc600](https://github.com/tx-ravenxbsw3/w3up/commit/47cc6006b1b7316c6815dfdca0a55122f632fec3))
* **capabilities:** top level filecoin cap ([#1606](https://github.com/tx-ravenxbsw3/w3up/issues/1606)) ([bf89593](https://github.com/tx-ravenxbsw3/w3up/commit/bf89593f48fcd041e1c12d144985406f139a4a7f))
* **main:** release capabilities 11.0.1 ([#1008](https://github.com/tx-ravenxbsw3/w3up/issues/1008)) ([35a5e1f](https://github.com/tx-ravenxbsw3/w3up/commit/35a5e1f768e672c98dad1a888a46597c74d78a2a))
* **main:** release capabilities 11.1.0 ([#1026](https://github.com/tx-ravenxbsw3/w3up/issues/1026)) ([64aeaca](https://github.com/tx-ravenxbsw3/w3up/commit/64aeacad4fc38a2e104dd8e4a8a3feaa37e6f535))
* **main:** release capabilities 11.2.0 ([#1084](https://github.com/tx-ravenxbsw3/w3up/issues/1084)) ([6d4395b](https://github.com/tx-ravenxbsw3/w3up/commit/6d4395be88f02c394b1ef601257a6c880c7a1356))
* **main:** release capabilities 11.3.0 ([#1098](https://github.com/tx-ravenxbsw3/w3up/issues/1098)) ([010d083](https://github.com/tx-ravenxbsw3/w3up/commit/010d0832ee9f3a27cbc773eb440e1ab8a8f3c7a2))
* **main:** release capabilities 11.3.1 ([#1101](https://github.com/tx-ravenxbsw3/w3up/issues/1101)) ([3cf73bb](https://github.com/tx-ravenxbsw3/w3up/commit/3cf73bb7152577315e0812a88085c2017a3e9a38))
* **main:** release capabilities 11.4.0 ([#1105](https://github.com/tx-ravenxbsw3/w3up/issues/1105)) ([90f60a9](https://github.com/tx-ravenxbsw3/w3up/commit/90f60a929088bd7b430b4801dec2878d08e3703b))
* **main:** release capabilities 11.4.1 ([#1131](https://github.com/tx-ravenxbsw3/w3up/issues/1131)) ([cca7880](https://github.com/tx-ravenxbsw3/w3up/commit/cca788082fa17d0546bc350e9c6a205d98fb0573))
* **main:** release capabilities 12.0.0 ([#1137](https://github.com/tx-ravenxbsw3/w3up/issues/1137)) ([9d2ca30](https://github.com/tx-ravenxbsw3/w3up/commit/9d2ca30a5a64bcbbbf3b4d28feda113f1aa36ee6))
* **main:** release capabilities 12.0.1 ([#1147](https://github.com/tx-ravenxbsw3/w3up/issues/1147)) ([3332f01](https://github.com/tx-ravenxbsw3/w3up/commit/3332f015468746d0e7b890696aa4bd34a0dacea7))
* **main:** release capabilities 12.0.2 ([#1152](https://github.com/tx-ravenxbsw3/w3up/issues/1152)) ([9ef43c7](https://github.com/tx-ravenxbsw3/w3up/commit/9ef43c71568ad0e2b7afedeac6990c7018a9eb5c))
* **main:** release capabilities 12.0.3 ([#1163](https://github.com/tx-ravenxbsw3/w3up/issues/1163)) ([fea6b30](https://github.com/tx-ravenxbsw3/w3up/commit/fea6b30fa451d505f46d643e6eab37519b100b47))
* **main:** release capabilities 12.1.0 ([#1195](https://github.com/tx-ravenxbsw3/w3up/issues/1195)) ([503aaba](https://github.com/tx-ravenxbsw3/w3up/commit/503aabad17a8e48656e08c99035a22fd2bcbc6da))
* **main:** release capabilities 13.0.0 ([#1230](https://github.com/tx-ravenxbsw3/w3up/issues/1230)) ([48772c9](https://github.com/tx-ravenxbsw3/w3up/commit/48772c9eec7083484b22d68f7b965b299b0e9d7a))
* **main:** release capabilities 13.1.0 ([#1257](https://github.com/tx-ravenxbsw3/w3up/issues/1257)) ([bbda53b](https://github.com/tx-ravenxbsw3/w3up/commit/bbda53b6462c5d4a18a4fa9113d32dc6bf6aff4a))
* **main:** release capabilities 13.1.1 ([#1283](https://github.com/tx-ravenxbsw3/w3up/issues/1283)) ([a6d83dd](https://github.com/tx-ravenxbsw3/w3up/commit/a6d83dddf17ef231aeedf54a126da26dbf62f874))
* **main:** release capabilities 13.2.0 ([#1315](https://github.com/tx-ravenxbsw3/w3up/issues/1315)) ([15483e4](https://github.com/tx-ravenxbsw3/w3up/commit/15483e44e0c8fa790aeb1e60dc6ec472b7aa54f3))
* **main:** release capabilities 13.2.1 ([#1362](https://github.com/tx-ravenxbsw3/w3up/issues/1362)) ([db084aa](https://github.com/tx-ravenxbsw3/w3up/commit/db084aa81511848cc7edf6e0f366030c46a66360))
* **main:** release capabilities 13.3.0 ([#1366](https://github.com/tx-ravenxbsw3/w3up/issues/1366)) ([7f24a7c](https://github.com/tx-ravenxbsw3/w3up/commit/7f24a7c14392da8881676d62d4c9d408882c6962))
* **main:** release capabilities 13.3.1 ([#1377](https://github.com/tx-ravenxbsw3/w3up/issues/1377)) ([b0e78b2](https://github.com/tx-ravenxbsw3/w3up/commit/b0e78b27171ae10881a65b17dc4e106289726589))
* **main:** release capabilities 14.0.0 ([#1386](https://github.com/tx-ravenxbsw3/w3up/issues/1386)) ([24031ec](https://github.com/tx-ravenxbsw3/w3up/commit/24031ecf71fc85cf3a112da7ed37814578c01700))
* **main:** release capabilities 14.0.1 ([#1395](https://github.com/tx-ravenxbsw3/w3up/issues/1395)) ([c8e3955](https://github.com/tx-ravenxbsw3/w3up/commit/c8e3955b2220558150b54954a0419c451441ead7))
* **main:** release capabilities 14.0.2 ([#1400](https://github.com/tx-ravenxbsw3/w3up/issues/1400)) ([18ebd24](https://github.com/tx-ravenxbsw3/w3up/commit/18ebd240ef9cd8ea48f470ad03ab4b16eba9d64a))
* **main:** release capabilities 15.0.0 ([#1412](https://github.com/tx-ravenxbsw3/w3up/issues/1412)) ([9ab8cc7](https://github.com/tx-ravenxbsw3/w3up/commit/9ab8cc7438dcef824cd081649ecc85dab1c4f388))
* **main:** release capabilities 16.0.0 ([#1419](https://github.com/tx-ravenxbsw3/w3up/issues/1419)) ([b0ddfec](https://github.com/tx-ravenxbsw3/w3up/commit/b0ddfec5b3d320c1a20e17762148b4f13cae85c7))
* **main:** release capabilities 17.0.0 ([#1428](https://github.com/tx-ravenxbsw3/w3up/issues/1428)) ([171eee8](https://github.com/tx-ravenxbsw3/w3up/commit/171eee8766e0f9ae5d9d8ca3415fef298df8a7f4))
* **main:** release capabilities 17.1.0 ([#1447](https://github.com/tx-ravenxbsw3/w3up/issues/1447)) ([3808af9](https://github.com/tx-ravenxbsw3/w3up/commit/3808af98bb7d10e17faf00aa12752df1a26746be))
* **main:** release capabilities 17.1.1 ([#1483](https://github.com/tx-ravenxbsw3/w3up/issues/1483)) ([3a53e4f](https://github.com/tx-ravenxbsw3/w3up/commit/3a53e4fedab617c09b9c7231ed47a44b3b419fca))
* **main:** release capabilities 17.2.0 ([#1494](https://github.com/tx-ravenxbsw3/w3up/issues/1494)) ([219bbbc](https://github.com/tx-ravenxbsw3/w3up/commit/219bbbcfee535459e0ebf3c74607f90049b7c082))
* **main:** release capabilities 17.3.0 ([#1503](https://github.com/tx-ravenxbsw3/w3up/issues/1503)) ([4dda548](https://github.com/tx-ravenxbsw3/w3up/commit/4dda54893afced24a74a2fed0aef81ec265a3d66))
* **main:** release capabilities 17.4.0 ([#1559](https://github.com/tx-ravenxbsw3/w3up/issues/1559)) ([608ee1f](https://github.com/tx-ravenxbsw3/w3up/commit/608ee1f4a8b29de679238513b04d3a13f97b0b5c))
* **main:** release capabilities 17.4.1 ([#1574](https://github.com/tx-ravenxbsw3/w3up/issues/1574)) ([dd287ce](https://github.com/tx-ravenxbsw3/w3up/commit/dd287cea78c4a9f230406e4c517c38cdf15ce9b7))
* **main:** release capabilities 18.0.0 ([#1578](https://github.com/tx-ravenxbsw3/w3up/issues/1578)) ([36761cc](https://github.com/tx-ravenxbsw3/w3up/commit/36761cc9c348ea1e36704f5e534ffe11e36836ec))
* **main:** release capabilities 18.0.1 ([#1609](https://github.com/tx-ravenxbsw3/w3up/issues/1609)) ([42b41f1](https://github.com/tx-ravenxbsw3/w3up/commit/42b41f168a1d8a9f8b1565ade705fbea4f9a4218))
* **main:** release capabilities 18.1.0 ([#1631](https://github.com/tx-ravenxbsw3/w3up/issues/1631)) ([f88384c](https://github.com/tx-ravenxbsw3/w3up/commit/f88384c5f99c9dc96e739fd857ac120bdc1cc934))
* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/tx-ravenxbsw3/w3up/issues/1577)) ([bdaa5e2](https://github.com/tx-ravenxbsw3/w3up/commit/bdaa5e297fef7e7ddca6a63c12ab071000cc7d2b))
* no longer depends on hd-scripts, packages use/configure eslint directly, fixes warnings from npm lint script ([#1058](https://github.com/tx-ravenxbsw3/w3up/issues/1058)) ([3a99cc0](https://github.com/tx-ravenxbsw3/w3up/commit/3a99cc02941f9d563cac1838e1e67a3faa42c3de))

## [18.1.0](https://github.com/storacha/w3up/compare/capabilities-v18.0.1...capabilities-v18.1.0) (2025-02-25)


### Features

* external login ([#1629](https://github.com/storacha/w3up/issues/1629)) ([150b5d7](https://github.com/storacha/w3up/commit/150b5d7c55ca92becbabab969285497fbba86268))

## [18.0.1](https://github.com/storacha/w3up/compare/capabilities-v18.0.0...capabilities-v18.0.1) (2024-12-19)


### Other Changes

* **capabilities:** top level filecoin cap ([#1606](https://github.com/storacha/w3up/issues/1606)) ([22d0bf9](https://github.com/storacha/w3up/commit/22d0bf9e540ffb8b76eb79453c4d881195abf2ef))

## [18.0.0](https://github.com/storacha/w3up/compare/capabilities-v17.4.1...capabilities-v18.0.0) (2024-12-05)


### ⚠ BREAKING CHANGES

* content serve authorization ([#1590](https://github.com/storacha/w3up/issues/1590))

### Features

* content serve authorization ([#1590](https://github.com/storacha/w3up/issues/1590)) ([8b553a5](https://github.com/storacha/w3up/commit/8b553a53253f55a3f0a2980557fa5c3b92427f3f))


### Fixes

* **egressRecord:** Remove unnecessary multiplication for ts conversion ([#1588](https://github.com/storacha/w3up/issues/1588)) ([b7bc90e](https://github.com/storacha/w3up/commit/b7bc90e6a33b8f33dd7356794c55a77b364799ee))


### Other Changes

* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/storacha/w3up/issues/1577)) ([1482d69](https://github.com/storacha/w3up/commit/1482d69c28baff1c27b1baf5f3e5c76f844e5576))

## [17.4.1](https://github.com/storacha/w3up/compare/capabilities-v17.4.0...capabilities-v17.4.1) (2024-11-05)


### Fixes

* **egress/record:** rename capability ([#1572](https://github.com/storacha/w3up/issues/1572)) ([d28691c](https://github.com/storacha/w3up/commit/d28691c4709f4e7c5ba81e042cac9e961c273bc9))

## [17.4.0](https://github.com/storacha/w3up/compare/capabilities-v17.3.0...capabilities-v17.4.0) (2024-10-24)


### Features

* Generate Space proofs on the fly, on `access/claim` ([#1555](https://github.com/storacha/w3up/issues/1555)) ([9e2b1d4](https://github.com/storacha/w3up/commit/9e2b1d4dc721d3e61cea008719d172909c984344))
* usage/record capability definition ([#1562](https://github.com/storacha/w3up/issues/1562)) ([98c8a87](https://github.com/storacha/w3up/commit/98c8a87c52ef88da728225259e77f65733d2d7e6))

## [17.3.0](https://github.com/storacha/w3up/compare/capabilities-v17.2.0...capabilities-v17.3.0) (2024-09-23)


### Features

* publish index claim ([#1487](https://github.com/storacha/w3up/issues/1487)) ([237b0c6](https://github.com/storacha/w3up/commit/237b0c6cda70ae3e156bac8a011a2739b346ae4b))


### Fixes

* repo URLs ([#1550](https://github.com/storacha/w3up/issues/1550)) ([e02ddf3](https://github.com/storacha/w3up/commit/e02ddf3696553b03f8d2f7316de0a99a9303a60f))
* update data-segment dep ([228ff79](https://github.com/storacha/w3up/commit/228ff7933219a0bf9ead371bb845d20a4859fda5))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/storacha/w3up/issues/1533)) ([07970ef](https://github.com/storacha/w3up/commit/07970efd443149158ebbfb2c4e745b5007eb9407))

## [17.2.0](https://github.com/w3s-project/w3up/compare/capabilities-v17.1.1...capabilities-v17.2.0) (2024-06-04)


### Features

* add blob/get ([#1484](https://github.com/w3s-project/w3up/issues/1484)) ([328039d](https://github.com/w3s-project/w3up/commit/328039d8a29fec3c1bbab28d1bb9de1643f54f71))

## [17.1.1](https://github.com/w3s-project/w3up/compare/capabilities-v17.1.0...capabilities-v17.1.1) (2024-05-30)


### Fixes

* rename blob and index client capabilities ([#1478](https://github.com/w3s-project/w3up/issues/1478)) ([17e3a31](https://github.com/w3s-project/w3up/commit/17e3a3161c6585b1844abcf7ed27252fa8580870))

## [17.1.0](https://github.com/w3s-project/w3up/compare/capabilities-v17.0.0...capabilities-v17.1.0) (2024-05-14)


### Features

* add "plan/create-admin-session" capability ([#1411](https://github.com/w3s-project/w3up/issues/1411)) ([50eeeb5](https://github.com/w3s-project/w3up/commit/50eeeb502335ba0413318b5047869a275901824b))
* add blob protocol to upload-client ([#1425](https://github.com/w3s-project/w3up/issues/1425)) ([49aef56](https://github.com/w3s-project/w3up/commit/49aef564a726d34dbbedbd83f5366d9320180f99))

## [17.0.0](https://github.com/w3s-project/w3up/compare/capabilities-v16.0.0...capabilities-v17.0.0) (2024-05-01)


### ⚠ BREAKING CHANGES

* add `index/add` handler ([#1421](https://github.com/w3s-project/w3up/issues/1421))

### Features

* add `index/add` handler ([#1421](https://github.com/w3s-project/w3up/issues/1421)) ([cbe9524](https://github.com/w3s-project/w3up/commit/cbe952451b719fe7ae2f7480d26865eca80aba55))

## [16.0.0](https://github.com/w3s-project/w3up/compare/capabilities-v15.0.0...capabilities-v16.0.0) (2024-04-26)


### ⚠ BREAKING CHANGES

* restrict store API to CARs ([#1415](https://github.com/w3s-project/w3up/issues/1415))

### Features

* restrict store API to CARs ([#1415](https://github.com/w3s-project/w3up/issues/1415)) ([e53aa87](https://github.com/w3s-project/w3up/commit/e53aa87780446458ef9a19c88877073c1470d50e))

## [15.0.0](https://github.com/w3s-project/w3up/compare/capabilities-v14.0.2...capabilities-v15.0.0) (2024-04-26)


### ⚠ BREAKING CHANGES

* **capabilities:** `BlobMultihash` type in `@web3-storage/capabilities` renamed to `Multihash`.

### Features

* **capabilities:** add `index/add` capability ([#1410](https://github.com/w3s-project/w3up/issues/1410)) ([1b71b89](https://github.com/w3s-project/w3up/commit/1b71b89ed989cde8ef4bf35c1ebc333872cbc54c))

## [14.0.2](https://github.com/w3s-project/w3up/compare/capabilities-v14.0.1...capabilities-v14.0.2) (2024-04-24)


### Fixes

* trigger capabilities release ([#1399](https://github.com/w3s-project/w3up/issues/1399)) ([7d9ab35](https://github.com/w3s-project/w3up/commit/7d9ab354d194b751bb7f34ffa2f74e7465cb40e2))

## [14.0.1](https://github.com/w3s-project/w3up/compare/capabilities-v14.0.0...capabilities-v14.0.1) (2024-04-23)


### Fixes

* migrate repo ([#1389](https://github.com/w3s-project/w3up/issues/1389)) ([475a287](https://github.com/w3s-project/w3up/commit/475a28743ff9f7138b46dfe4227d3c80ed75a6a2))

## [14.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v13.3.1...capabilities-v14.0.0) (2024-04-23)


### ⚠ BREAKING CHANGES

* allocations storage interface now requires remove to be implemented

### Features

* add blob list and remove ([#1385](https://github.com/web3-storage/w3up/issues/1385)) ([2f69946](https://github.com/web3-storage/w3up/commit/2f6994600e8cc0f70cedc5afe06003a2a0b70af3))

## [13.3.1](https://github.com/web3-storage/w3up/compare/capabilities-v13.3.0...capabilities-v13.3.1) (2024-04-16)


### Fixes

* capabilities should export blob caps ([#1376](https://github.com/web3-storage/w3up/issues/1376)) ([460729e](https://github.com/web3-storage/w3up/commit/460729ec296ac2656b264af442b6d3bc25aa8847))

## [13.3.0](https://github.com/web3-storage/w3up/compare/capabilities-v13.2.1...capabilities-v13.3.0) (2024-04-12)


### Features

* blob, web3.storage and ucan conclude capabilities together with api handlers  ([#1342](https://github.com/web3-storage/w3up/issues/1342)) ([00735a8](https://github.com/web3-storage/w3up/commit/00735a80dfddbe86359af78ed9bd182f4804691f))

## [13.2.1](https://github.com/web3-storage/w3up/compare/capabilities-v13.2.0...capabilities-v13.2.1) (2024-04-12)


### Fixes

* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/web3-storage/w3up/issues/1359)) ([87ca098](https://github.com/web3-storage/w3up/commit/87ca098186fe204ff3409a2684719f1c54148c97))

## [13.2.0](https://github.com/web3-storage/w3up/compare/capabilities-v13.1.1...capabilities-v13.2.0) (2024-03-21)


### Features

* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/web3-storage/w3up/issues/1312)) ([d6978d7](https://github.com/web3-storage/w3up/commit/d6978d7ab299be76987c6533d18e6857f6998fe6))

## [13.1.1](https://github.com/web3-storage/w3up/compare/capabilities-v13.1.0...capabilities-v13.1.1) (2024-01-29)


### Fixes

* one more tweak to the `PlanStorage` interface ([#1280](https://github.com/web3-storage/w3up/issues/1280)) ([5a44565](https://github.com/web3-storage/w3up/commit/5a44565feb33fc08102cd2559a2f22fb0476e86b))

## [13.1.0](https://github.com/web3-storage/w3up/compare/capabilities-v13.0.0...capabilities-v13.1.0) (2024-01-25)


### Features

* add `initialize` method to `PlansStorage` ([#1278](https://github.com/web3-storage/w3up/issues/1278)) ([6792126](https://github.com/web3-storage/w3up/commit/6792126d63a1e983713c3886eeba64038cb7cf34))
* add a function to verify and return Abilities. ([#1252](https://github.com/web3-storage/w3up/issues/1252)) ([2f026a2](https://github.com/web3-storage/w3up/commit/2f026a2483a4f323c4e2c6a8a8cb10afd92e21c4))
* change `plan/update` to `plan/set` and use existing `PlansStorage#set` to implement an invocation handler ([#1258](https://github.com/web3-storage/w3up/issues/1258)) ([1ccbfe9](https://github.com/web3-storage/w3up/commit/1ccbfe9f84ae5b2e99e315c92d15d2b54e9723ba))
* introduce capability for changing billing plan ([#1253](https://github.com/web3-storage/w3up/issues/1253)) ([d33b3a9](https://github.com/web3-storage/w3up/commit/d33b3a9f72a5e7a738d2a084eb19388fa70d9433))

## [13.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v12.1.0...capabilities-v13.0.0) (2023-12-07)


### ⚠ BREAKING CHANGES

* return allocated bytes in `store/add` receipt ([#1213](https://github.com/web3-storage/w3up/issues/1213))

### Features

* return allocated bytes in `store/add` receipt ([#1213](https://github.com/web3-storage/w3up/issues/1213)) ([5d52e44](https://github.com/web3-storage/w3up/commit/5d52e447c14e7f7fd334e7ff575e032b7b0d89d7))

## [12.1.0](https://github.com/web3-storage/w3up/compare/capabilities-v12.0.3...capabilities-v12.1.0) (2023-11-28)


### Features

* move aggregate information out of deals in filecoin/info ([#1192](https://github.com/web3-storage/w3up/issues/1192)) ([18dc590](https://github.com/web3-storage/w3up/commit/18dc590ad50a023ef3094bfc1a2d729459e5d68e))

## [12.0.3](https://github.com/web3-storage/w3up/compare/capabilities-v12.0.2...capabilities-v12.0.3) (2023-11-22)


### Fixes

* package metadata ([#1161](https://github.com/web3-storage/w3up/issues/1161)) ([b8a1cc2](https://github.com/web3-storage/w3up/commit/b8a1cc2e125a91be582998bda295e1ae1caab087))

## [12.0.2](https://github.com/web3-storage/w3up/compare/capabilities-v12.0.1...capabilities-v12.0.2) (2023-11-16)


### Bug Fixes

* upgrade @ucanto/validator with bugfix ([#1151](https://github.com/web3-storage/w3up/issues/1151)) ([d4e961b](https://github.com/web3-storage/w3up/commit/d4e961bab09e88245e7d9323146849271e78eb57))

## [12.0.1](https://github.com/web3-storage/w3up/compare/capabilities-v12.0.0...capabilities-v12.0.1) (2023-11-15)


### Bug Fixes

* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/web3-storage/w3up/issues/1141)) ([0b8d3f3](https://github.com/web3-storage/w3up/commit/0b8d3f3b52918b1b4d3b76ea6fea3fb0c837cd73))

## [12.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v11.4.1...capabilities-v12.0.0) (2023-11-15)


### ⚠ BREAKING CHANGES

* coupon ([#1136](https://github.com/web3-storage/w3up/issues/1136))

### Features

* coupon ([#1136](https://github.com/web3-storage/w3up/issues/1136)) ([1b94f2d](https://github.com/web3-storage/w3up/commit/1b94f2d3f6538d717d38b21dcb76657fd1f3e268))

## [11.4.1](https://github.com/web3-storage/w3up/compare/capabilities-v11.4.0...capabilities-v11.4.1) (2023-11-15)


### Bug Fixes

* upgrade ucanto core ([#1127](https://github.com/web3-storage/w3up/issues/1127)) ([5ce4d22](https://github.com/web3-storage/w3up/commit/5ce4d2292d7e980da4a2ea0f1583f608a81157d2))

## [11.4.0](https://github.com/web3-storage/w3up/compare/capabilities-v11.3.1...capabilities-v11.4.0) (2023-11-09)


### Features

* add `subscription/list` capability ([#1088](https://github.com/web3-storage/w3up/issues/1088)) ([471d7e5](https://github.com/web3-storage/w3up/commit/471d7e5db24e12a06c1c52ae76bf95ff9471bac8))

## [11.3.1](https://github.com/web3-storage/w3up/compare/capabilities-v11.3.0...capabilities-v11.3.1) (2023-11-08)


### Bug Fixes

* put access.session back ([#1100](https://github.com/web3-storage/w3up/issues/1100)) ([10a1a4b](https://github.com/web3-storage/w3up/commit/10a1a4bfc5ec79ea0b7b2049fd7d1953ca0810ef))

## [11.3.0](https://github.com/web3-storage/w3up/compare/capabilities-v11.2.0...capabilities-v11.3.0) (2023-11-08)


### Features

* filecoin info ([#1091](https://github.com/web3-storage/w3up/issues/1091)) ([adb2442](https://github.com/web3-storage/w3up/commit/adb24424d1faf50daf2339b77c22fdd44faa236a))

## [11.2.0](https://github.com/web3-storage/w3up/compare/capabilities-v11.1.0...capabilities-v11.2.0) (2023-11-07)


### Features

* add usage/report capability ([#1079](https://github.com/web3-storage/w3up/issues/1079)) ([6418b4b](https://github.com/web3-storage/w3up/commit/6418b4b22329a118fb258928bd9a6a45ced5ce45))

## [11.1.0](https://github.com/web3-storage/w3up/compare/capabilities-v11.0.1...capabilities-v11.1.0) (2023-10-27)


### Features

* implement `plan/get` capability ([#1005](https://github.com/web3-storage/w3up/issues/1005)) ([f0456d2](https://github.com/web3-storage/w3up/commit/f0456d2e2aab462666810e22abd7dfb7e1ce21be))

## [11.0.1](https://github.com/web3-storage/w3up/compare/capabilities-v11.0.0...capabilities-v11.0.1) (2023-10-25)


### Bug Fixes

* fix arethetypesworking errors in all packages ([#1004](https://github.com/web3-storage/w3up/issues/1004)) ([2e2936a](https://github.com/web3-storage/w3up/commit/2e2936a3831389dd13be5be5146a04e2b15553c5))

## [11.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v10.2.0...capabilities-v11.0.0) (2023-10-24)


### ⚠ BREAKING CHANGES

* see latest specs https://github.com/web3-storage/specs/blob/cbdb706f18567900c5c24d7fb16ccbaf93d0d023/w3-filecoin.md
* filecoin client to use new capabilities
* filecoin capabilities

### Bug Fixes

* add missing ContentNotFound definition for filecoin offer failure ([c0b97bf](https://github.com/web3-storage/w3up/commit/c0b97bf42d87b49d7de11119f9eb6166ab8d97d0))
* add missing filecoin submit success and failure types ([c0b97bf](https://github.com/web3-storage/w3up/commit/c0b97bf42d87b49d7de11119f9eb6166ab8d97d0))
* client tests ([b0d9c3f](https://github.com/web3-storage/w3up/commit/b0d9c3f258d37701487ef02f70a93e2dd1a18775))
* type errors ([c0b97bf](https://github.com/web3-storage/w3up/commit/c0b97bf42d87b49d7de11119f9eb6166ab8d97d0))
* upgrade ucanto in filecoin api ([c95fb54](https://github.com/web3-storage/w3up/commit/c95fb54cdb04f50ff78e5113e70d73c1cd6d8b47))


### Code Refactoring

* filecoin api services events and tests ([#974](https://github.com/web3-storage/w3up/issues/974)) ([953537b](https://github.com/web3-storage/w3up/commit/953537bcb98d94b9e9655797a7f9026643ab949f))
* filecoin capabilities ([c0b97bf](https://github.com/web3-storage/w3up/commit/c0b97bf42d87b49d7de11119f9eb6166ab8d97d0))
* filecoin client to use new capabilities ([b0d9c3f](https://github.com/web3-storage/w3up/commit/b0d9c3f258d37701487ef02f70a93e2dd1a18775))

## [10.2.0](https://github.com/web3-storage/w3up/compare/capabilities-v10.1.0...capabilities-v10.2.0) (2023-10-19)


### Features

* add `store/get` and `upload/get` capabilities ([#942](https://github.com/web3-storage/w3up/issues/942)) ([40c79eb](https://github.com/web3-storage/w3up/commit/40c79eb8f246775b9e1828240f271fa75ef696be))

## [10.1.0](https://github.com/web3-storage/w3up/compare/capabilities-v10.0.0...capabilities-v10.1.0) (2023-10-18)


### Features

* add revocation to access-client and w3up-client ([#975](https://github.com/web3-storage/w3up/issues/975)) ([6c877aa](https://github.com/web3-storage/w3up/commit/6c877aac78eddb924e999dc3270cba010e48e30a))

## [10.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v9.5.0...capabilities-v10.0.0) (2023-10-12)


### ⚠ BREAKING CHANGES

* Returning the `size` means that we need to fetch the stored item beforehand, and if it does not exist throw a `StoreItemNotFound` error. This is a change from the current behaviour which returns successfully even if the item is not present in the space.

### Features

* add size to `store/remove` receipt ([#969](https://github.com/web3-storage/w3up/issues/969)) ([d2100eb](https://github.com/web3-storage/w3up/commit/d2100eb0ffa5968c326d58d583a258187f9119eb))

## [9.5.0](https://github.com/web3-storage/w3up/compare/capabilities-v9.4.0...capabilities-v9.5.0) (2023-10-10)


### Features

* revocation handler ([#960](https://github.com/web3-storage/w3up/issues/960)) ([91f52c6](https://github.com/web3-storage/w3up/commit/91f52c6d35e4aea2a98c75d8b95ff61cdffac452))


### Bug Fixes

* upgrade to latest ts ([#962](https://github.com/web3-storage/w3up/issues/962)) ([711e3f7](https://github.com/web3-storage/w3up/commit/711e3f73f6905fde0d929952fff70be845a55fa1))

## [9.4.0](https://github.com/web3-storage/w3up/compare/capabilities-v9.3.0...capabilities-v9.4.0) (2023-10-10)


### Features

* define ucan/revoke capability ([#943](https://github.com/web3-storage/w3up/issues/943)) ([5d957ef](https://github.com/web3-storage/w3up/commit/5d957ef1e644557f557dc45a048150d73894e801))
* upgrade to ucanto@9 ([#951](https://github.com/web3-storage/w3up/issues/951)) ([d72faf1](https://github.com/web3-storage/w3up/commit/d72faf1bb07dd11462ae6dff8ee0469f8ae7e9e7))

## [9.3.0](https://github.com/web3-storage/w3up/compare/capabilities-v9.2.1...capabilities-v9.3.0) (2023-09-13)


### Features

* implement `admin/upload/inspect` and `admin/store/inspect` capabilities ([#918](https://github.com/web3-storage/w3up/issues/918)) ([5616a12](https://github.com/web3-storage/w3up/commit/5616a12125500a1d5ee41f0504812d82c0451852))

## [9.2.1](https://github.com/web3-storage/w3up/compare/capabilities-v9.2.0...capabilities-v9.2.1) (2023-08-30)


### Bug Fixes

* w3filecoin spec separate capabilities to queue and enqueue ([#856](https://github.com/web3-storage/w3up/issues/856)) ([6bf9142](https://github.com/web3-storage/w3up/commit/6bf9142636fa65367faed8414c50beb9c1791726)), closes [#855](https://github.com/web3-storage/w3up/issues/855)

## [9.2.0](https://github.com/web3-storage/w3up/compare/capabilities-v9.1.0...capabilities-v9.2.0) (2023-08-22)


### Features

* change "total" to "limit" ([#867](https://github.com/web3-storage/w3up/issues/867)) ([8295070](https://github.com/web3-storage/w3up/commit/8295070c8fbbc508da2cfe6f32846090a530f282))

## [9.1.0](https://github.com/web3-storage/w3up/compare/capabilities-v9.0.1...capabilities-v9.1.0) (2023-08-22)


### Features

* add subscriptions to CustomerGetSuccess ([#863](https://github.com/web3-storage/w3up/issues/863)) ([dd2e77c](https://github.com/web3-storage/w3up/commit/dd2e77c51d84a517cb50ff05199b8eebf9223bf2))

## [9.0.1](https://github.com/web3-storage/w3up/compare/capabilities-v9.0.0...capabilities-v9.0.1) (2023-08-10)


### Bug Fixes

* upgrade data segment ([#850](https://github.com/web3-storage/w3up/issues/850)) ([fba281f](https://github.com/web3-storage/w3up/commit/fba281f8cd3ce2a0a00ffd50a4a73d7701b489ce))

## [9.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v8.0.0...capabilities-v9.0.0) (2023-08-09)


### ⚠ BREAKING CHANGES

* introduce new administrative capabilities ([#832](https://github.com/web3-storage/w3up/issues/832))

### Features

* introduce new administrative capabilities ([#832](https://github.com/web3-storage/w3up/issues/832)) ([7b8037a](https://github.com/web3-storage/w3up/commit/7b8037a6ab92f830af4aa7ba07a91bc2a20c0d8c))

## [8.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v7.0.0...capabilities-v8.0.0) (2023-08-09)


### ⚠ BREAKING CHANGES

* update aggregation capabilitites to use height instead of size together with client and api ([#831](https://github.com/web3-storage/w3up/issues/831))

### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))


### Bug Fixes

* update aggregation capabilitites to use height instead of size together with client and api ([#831](https://github.com/web3-storage/w3up/issues/831)) ([31730f0](https://github.com/web3-storage/w3up/commit/31730f0cb37b16f12f778ee8d2ecb5693bb2cd23))

## [7.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v6.0.1...capabilities-v7.0.0) (2023-07-06)


### ⚠ BREAKING CHANGES

* aggregate capabilities now have different nb properties and aggregate client api was simplified

### Bug Fixes

* update aggregate spec in client and api ([#824](https://github.com/web3-storage/w3up/issues/824)) ([ebefd88](https://github.com/web3-storage/w3up/commit/ebefd889a028f325690370db8043c7b9e9fdf7bb))

## [6.0.1](https://github.com/web3-storage/w3up/compare/capabilities-v6.0.0...capabilities-v6.0.1) (2023-06-09)


### Bug Fixes

* specify module types in exports ([#814](https://github.com/web3-storage/w3up/issues/814)) ([d64f1b6](https://github.com/web3-storage/w3up/commit/d64f1b6b91c87287e04fabed384041e2dff0efca))

## [6.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v5.0.1...capabilities-v6.0.0) (2023-06-07)


### ⚠ BREAKING CHANGES

* merge `@web3-storage/access-api` into `@web3-storage/upload-api` ([#790](https://github.com/web3-storage/w3up/issues/790))

### Features

* merge `@web3-storage/access-api` into `@web3-storage/upload-api` ([#790](https://github.com/web3-storage/w3up/issues/790)) ([4f6ddb6](https://github.com/web3-storage/w3up/commit/4f6ddb690c365a42a3dc4c5c6898e4999bd0f868))
* w3 aggregate protocol client and api implementation ([#787](https://github.com/web3-storage/w3up/issues/787)) ([b58069d](https://github.com/web3-storage/w3up/commit/b58069d7960efe09283f3b23fed77515b62d4639))

## [5.0.1](https://github.com/web3-storage/w3up/compare/capabilities-v5.0.0...capabilities-v5.0.1) (2023-05-23)


### Bug Fixes

* upgrade remaining ucanto deps ([#798](https://github.com/web3-storage/w3up/issues/798)) ([7211501](https://github.com/web3-storage/w3up/commit/72115010663a62140127cdeed21f2dc37f59da08))
* upgrade ucanto to 8 ([#794](https://github.com/web3-storage/w3up/issues/794)) ([00b011d](https://github.com/web3-storage/w3up/commit/00b011d87f628d4b3040398ca6cba567a69713ff))

## [5.0.0](https://github.com/web3-storage/w3up/compare/capabilities-v4.0.1...capabilities-v5.0.0) (2023-05-02)


### ⚠ BREAKING CHANGES

* upgrade to ucanto7.x.x ([#774](https://github.com/web3-storage/w3up/issues/774))

### Features

* upgrade to ucanto7.x.x ([#774](https://github.com/web3-storage/w3up/issues/774)) ([0cc6e66](https://github.com/web3-storage/w3up/commit/0cc6e66a80476e05c75bea94c1bee9bd12cbacf5))

## [4.0.1](https://github.com/web3-storage/w3protocol/compare/capabilities-v4.0.0...capabilities-v4.0.1) (2023-03-27)


### Features

* allow multiple providers ([#595](https://github.com/web3-storage/w3protocol/issues/595)) ([96c5a2e](https://github.com/web3-storage/w3protocol/commit/96c5a2e5a03432d8483d044ae10f6f3e03c2710c))


### Miscellaneous Chores

* **access-client:** release 11.0.0-rc.0 ([#573](https://github.com/web3-storage/w3protocol/issues/573)) ([be4386d](https://github.com/web3-storage/w3protocol/commit/be4386d66ceea393f289adb3c79273c250542807))

## [4.0.0](https://github.com/web3-storage/w3protocol/compare/capabilities-v3.2.0...capabilities-v4.0.0) (2023-03-17)


### ⚠ BREAKING CHANGES

* implement new account-based multi-device flow ([#433](https://github.com/web3-storage/w3protocol/issues/433))

### Features

* define `access/confirm` handler and use it in ucanto-test-utils registerSpaces + validate-email handler ([#530](https://github.com/web3-storage/w3protocol/issues/530)) ([b1bbc90](https://github.com/web3-storage/w3protocol/commit/b1bbc907c96cfc7788f50fb0c154d9b54894e03e))
* implement new account-based multi-device flow ([#433](https://github.com/web3-storage/w3protocol/issues/433)) ([1ddc6a0](https://github.com/web3-storage/w3protocol/commit/1ddc6a0c53f8cdb6837a315d8aaf567100dfb8d7))
* provision provider type is now the DID of the w3s service ([#528](https://github.com/web3-storage/w3protocol/issues/528)) ([6a72855](https://github.com/web3-storage/w3protocol/commit/6a72855db4d6e838e9948f3951fdb5ef324eec95))

## [3.2.0](https://github.com/web3-storage/w3protocol/compare/capabilities-v3.1.0...capabilities-v3.2.0) (2023-03-08)


### Features

* upgrade to new ucanto ([#498](https://github.com/web3-storage/w3protocol/issues/498)) ([dcb41a9](https://github.com/web3-storage/w3protocol/commit/dcb41a9981c2b6bebbdbd29debcad9f510383680))

## [3.1.0](https://github.com/web3-storage/w3protocol/compare/capabilities-v3.0.0...capabilities-v3.1.0) (2023-03-04)


### Features

* access-api handles provider/add invocations ([#462](https://github.com/web3-storage/w3protocol/issues/462)) ([5fb56f7](https://github.com/web3-storage/w3protocol/commit/5fb56f794529f3d4de2b4597c47503002767fabb))
* includes proofs chains in the delegated authorization chain ([#467](https://github.com/web3-storage/w3protocol/issues/467)) ([5144293](https://github.com/web3-storage/w3protocol/commit/5144293deabd9d5380448ae288e089ef2652def7))

## [3.0.0](https://github.com/web3-storage/w3protocol/compare/capabilities-v2.3.0...capabilities-v3.0.0) (2023-03-01)


### ⚠ BREAKING CHANGES

* upgrade capabilities to latest ucanto ([#463](https://github.com/web3-storage/w3protocol/issues/463))

### Features

* handle access/delegate invocations without error ([#427](https://github.com/web3-storage/w3protocol/issues/427)) ([4f0bd1c](https://github.com/web3-storage/w3protocol/commit/4f0bd1c1cd3cfb1c848892ad418c6d7b2197045a))
* upgrade capabilities to latest ucanto ([#463](https://github.com/web3-storage/w3protocol/issues/463)) ([2d786ee](https://github.com/web3-storage/w3protocol/commit/2d786ee81a6eb72c4782548ad3e3796fe3947fa5))


### Bug Fixes

* allow injecting email ([#466](https://github.com/web3-storage/w3protocol/issues/466)) ([e19847f](https://github.com/web3-storage/w3protocol/commit/e19847fef804fed33f709ec8b78640fff21ca01e))

## [2.3.0](https://github.com/web3-storage/w3protocol/compare/capabilities-v2.2.0...capabilities-v2.3.0) (2023-02-10)


### Features

* add `pre` caveat to `store/list` and `upload/list` ([#423](https://github.com/web3-storage/w3protocol/issues/423)) ([a0f6d28](https://github.com/web3-storage/w3protocol/commit/a0f6d2834b900c4522fe71da473e4b43760502fd))
* add access/delegate capability parser exported from @web3-storage/capabilities ([#420](https://github.com/web3-storage/w3protocol/issues/420)) ([e8e2b1a](https://github.com/web3-storage/w3protocol/commit/e8e2b1a7606ce82bc346517d875de5244d240229))
* add support for access/authorize and update ([#392](https://github.com/web3-storage/w3protocol/issues/392)) ([9c8ca0b](https://github.com/web3-storage/w3protocol/commit/9c8ca0b385c940c8f0c21ee9edde093d2dcab8b8)), closes [#386](https://github.com/web3-storage/w3protocol/issues/386)
* define access/claim in @web3-storage/capabilities ([#409](https://github.com/web3-storage/w3protocol/issues/409)) ([4d72ba3](https://github.com/web3-storage/w3protocol/commit/4d72ba3a1ce2564cda13c62137967613b18334a7))

## [2.2.0](https://github.com/web3-storage/w3protocol/compare/capabilities-v2.1.0...capabilities-v2.2.0) (2023-01-30)


### Features

* access-api forwards store/ and upload/ invocations to upload-api ([#334](https://github.com/web3-storage/w3protocol/issues/334)) ([b773376](https://github.com/web3-storage/w3protocol/commit/b77337692d9e4580031c429c429d4055d6f6ebff))
* **capabilities:** implement access/authorize and ./update caps ([#387](https://github.com/web3-storage/w3protocol/issues/387)) ([4242ce0](https://github.com/web3-storage/w3protocol/commit/4242ce046b8e95c43dbf33a139bb98b682eeb198)), closes [#385](https://github.com/web3-storage/w3protocol/issues/385)
* embedded key resolution ([#312](https://github.com/web3-storage/w3protocol/issues/312)) ([4da91d5](https://github.com/web3-storage/w3protocol/commit/4da91d5f7f798d0d46c4df2aaf224610a8760d9e))
* update @ucanto/* to ~4.2.3 ([#405](https://github.com/web3-storage/w3protocol/issues/405)) ([50c0c80](https://github.com/web3-storage/w3protocol/commit/50c0c80789c26b777e854b7208b7391499d2ef18))
* update access-api ucanto proxy to not need a signer ([#390](https://github.com/web3-storage/w3protocol/issues/390)) ([71cbeb7](https://github.com/web3-storage/w3protocol/commit/71cbeb718d0a5132b97efa1173a5aaf9c75cbe80))


### Bug Fixes

* fix client cli service did resolve ([#292](https://github.com/web3-storage/w3protocol/issues/292)) ([6be9608](https://github.com/web3-storage/w3protocol/commit/6be9608a907665a8123938ef804bebfffc5c7232))

## [2.1.0](https://github.com/web3-storage/w3protocol/compare/capabilities-v2.0.0...capabilities-v2.1.0) (2022-12-13)


### Features

* sync encode/decode delegations ([#276](https://github.com/web3-storage/w3protocol/issues/276)) ([ab981fb](https://github.com/web3-storage/w3protocol/commit/ab981fb6e33799153022c0f6d06c282917e7af7c))


### Bug Fixes

* make d1 spaces.metadata nullable and change to kysely ([#284](https://github.com/web3-storage/w3protocol/issues/284)) ([c8a9ce5](https://github.com/web3-storage/w3protocol/commit/c8a9ce544226b3c8456d45b15e29cec84894aeb8)), closes [#280](https://github.com/web3-storage/w3protocol/issues/280)

## [2.0.0](https://github.com/web3-storage/w3protocol/compare/capabilities-v1.0.0...capabilities-v2.0.0) (2022-12-07)


### ⚠ BREAKING CHANGES

* upgrade access-api @ucanto/* and @ipld/dag-ucan major versions ([#246](https://github.com/web3-storage/w3protocol/issues/246))
* upgrade to `@ucanto/{interface,principal}`@^4.0.0 ([#238](https://github.com/web3-storage/w3protocol/issues/238))
* follow up on the capabilities extract ([#239](https://github.com/web3-storage/w3protocol/issues/239))

### Features

* **access-client:** cli and recover ([#207](https://github.com/web3-storage/w3protocol/issues/207)) ([adb3a8d](https://github.com/web3-storage/w3protocol/commit/adb3a8d61d42b31f106e86b95faa3e442f5dc2c7))
* follow up on the capabilities extract ([#239](https://github.com/web3-storage/w3protocol/issues/239)) ([ef5e779](https://github.com/web3-storage/w3protocol/commit/ef5e77922b67155f0c3e5cb37c12e32f9a56cce1))
* Revert "feat!: upgrade to `@ucanto/{interface,principal}`@^4.0.0" ([#245](https://github.com/web3-storage/w3protocol/issues/245)) ([c182bbe](https://github.com/web3-storage/w3protocol/commit/c182bbe5e8c5a7d5c74b10cbf4b7a45b51e9b184))
* upgrade access-api @ucanto/* and @ipld/dag-ucan major versions ([#246](https://github.com/web3-storage/w3protocol/issues/246)) ([5e663d1](https://github.com/web3-storage/w3protocol/commit/5e663d12ccea7d21cc8e7c36869f144a08eaa1b0))
* upgrade to `@ucanto/{interface,principal}`@^4.0.0 ([#238](https://github.com/web3-storage/w3protocol/issues/238)) ([2f3bab8](https://github.com/web3-storage/w3protocol/commit/2f3bab8924fe7f34a5db64d2521730fc85739d3a))


### Bug Fixes

* fix Access API cannot get space/info [#243](https://github.com/web3-storage/w3protocol/issues/243) ([#255](https://github.com/web3-storage/w3protocol/issues/255)) ([1bacd54](https://github.com/web3-storage/w3protocol/commit/1bacd544da803c43cf85043ecdada4dee2b3e2d3))
* generated typdefs ([#258](https://github.com/web3-storage/w3protocol/issues/258)) ([2af1b76](https://github.com/web3-storage/w3protocol/commit/2af1b76057476d2510d98a0b99a95f820cf4d344))

## 1.0.0 (2022-12-01)


### Bug Fixes

* add exports to packages/capabilities/readme.md, add workflow to check for conventional-commits names in PRs ([#233](https://github.com/web3-storage/w3protocol/issues/233)) ([da63284](https://github.com/web3-storage/w3protocol/commit/da6328467a198e3197bf20219aa2fa3bbe047d65))
