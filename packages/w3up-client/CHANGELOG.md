# Changelog

## [18.0.0](https://github.com/tx-ravenxbsw3/w3up/compare/w3up-client-v17.3.0...w3up-client-v18.0.0) (2025-09-29)


### ⚠ BREAKING CHANGES

* content serve authorization ([#1590](https://github.com/tx-ravenxbsw3/w3up/issues/1590))
* allow invocation configuration to be generated on demand ([#1507](https://github.com/tx-ravenxbsw3/w3up/issues/1507))
* `AllocationsStorage` and `BlobsStorage` methods not take `MultihashDigest` types instead of `Uint8Array`s.
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/tx-ravenxbsw3/w3up/issues/1444))
* delegated capabilities required to use `uploadFile`, `uploadDirectory` and `uploadCAR` have changed. In order to use these methods your agent will now need to be delegated `blob/add`, `index/add`, `filecoin/offer` and `upload/add` capabilities. Note: no code changes are required.
* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344))
* restrict store API to CARs ([#1415](https://github.com/tx-ravenxbsw3/w3up/issues/1415))
* return allocated bytes in `store/add` receipt ([#1213](https://github.com/tx-ravenxbsw3/w3up/issues/1213))
* coupon ([#1136](https://github.com/tx-ravenxbsw3/w3up/issues/1136))
* tweak readmes to get release-please to bump major version ([#1102](https://github.com/tx-ravenxbsw3/w3up/issues/1102))

### Features

* account.plan.get method ([#1117](https://github.com/tx-ravenxbsw3/w3up/issues/1117)) ([f3b6269](https://github.com/tx-ravenxbsw3/w3up/commit/f3b62699d053c901c0de31fe4790199cd211131e))
* add "plan/create-admin-session" capability ([#1411](https://github.com/tx-ravenxbsw3/w3up/issues/1411)) ([d9662c7](https://github.com/tx-ravenxbsw3/w3up/commit/d9662c75dd138be02213931be3c8b59f08f26ad1))
* add `set` method to `AccountPlan` ([#1281](https://github.com/tx-ravenxbsw3/w3up/issues/1281)) ([d578c7c](https://github.com/tx-ravenxbsw3/w3up/commit/d578c7c11a1fa397b5354f31df80459fb2da63b4))
* add `subscription/list` capability ([#1088](https://github.com/tx-ravenxbsw3/w3up/issues/1088)) ([dd2c715](https://github.com/tx-ravenxbsw3/w3up/commit/dd2c715b6b3004425273d15e3a9eaa3d2f25673a))
* add a function to verify and return Abilities. ([#1252](https://github.com/tx-ravenxbsw3/w3up/issues/1252)) ([99479ec](https://github.com/tx-ravenxbsw3/w3up/commit/99479ecae8640524f798e9ad64a688ff01df7f1b))
* add blob protocol to upload-client ([#1425](https://github.com/tx-ravenxbsw3/w3up/issues/1425)) ([44bde76](https://github.com/tx-ravenxbsw3/w3up/commit/44bde7616adc94f82cfef751bcaa94cf59bf24c5))
* add blob/get ([#1484](https://github.com/tx-ravenxbsw3/w3up/issues/1484)) ([9f774cc](https://github.com/tx-ravenxbsw3/w3up/commit/9f774ccb847b0e1182b6d9a0a1ff13db03253800))
* add pre-built browser bundle ([#1586](https://github.com/tx-ravenxbsw3/w3up/issues/1586)) ([85cc52d](https://github.com/tx-ravenxbsw3/w3up/commit/85cc52da4e81c3ab2b6ba138e6443dd7866d4cae))
* add remove high level function to client ([#1248](https://github.com/tx-ravenxbsw3/w3up/issues/1248)) ([8cc2289](https://github.com/tx-ravenxbsw3/w3up/commit/8cc22893d6d9f27d0567b8ae801e785f41aa1453))
* add store.get and upload.get to clients ([#1178](https://github.com/tx-ravenxbsw3/w3up/issues/1178)) ([b118eff](https://github.com/tx-ravenxbsw3/w3up/commit/b118effaf5d899257d337e3740ef9a25772925c8))
* add usage/report capability ([#1079](https://github.com/tx-ravenxbsw3/w3up/issues/1079)) ([95db863](https://github.com/tx-ravenxbsw3/w3up/commit/95db8632ce796ff698d7b016cca6e676e846eeac))
* allow invocation configuration to be generated on demand ([#1507](https://github.com/tx-ravenxbsw3/w3up/issues/1507)) ([f48dd12](https://github.com/tx-ravenxbsw3/w3up/commit/f48dd122c4493a8f393482a91362c394d9e2fc60))
* **client:** optional account recovery ([#1546](https://github.com/tx-ravenxbsw3/w3up/issues/1546)) ([c92be31](https://github.com/tx-ravenxbsw3/w3up/commit/c92be31c0134251c9372c340548fa6c09434d369))
* configure UnixFS encoder ([#1509](https://github.com/tx-ravenxbsw3/w3up/issues/1509)) ([e2ebac5](https://github.com/tx-ravenxbsw3/w3up/commit/e2ebac52412e25d097a7f77fb933fc64110eb027))
* content serve authorization ([#1590](https://github.com/tx-ravenxbsw3/w3up/issues/1590)) ([c752277](https://github.com/tx-ravenxbsw3/w3up/commit/c752277cc07008437fc4482ea5689a1cabc92abf))
* coupon ([#1136](https://github.com/tx-ravenxbsw3/w3up/issues/1136)) ([c41320d](https://github.com/tx-ravenxbsw3/w3up/commit/c41320d6fccaa4b9fac924acae3259fd1df142e9))
* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344)) ([db98e3a](https://github.com/tx-ravenxbsw3/w3up/commit/db98e3ad7fd5ce589ab5f002a9e614341f9121ca))
* export Account so we can use it in w3ui ([#1116](https://github.com/tx-ravenxbsw3/w3up/issues/1116)) ([c17a5b3](https://github.com/tx-ravenxbsw3/w3up/commit/c17a5b3d49cdb01abbf5115a8a902142c2c1f273))
* export PlanSet{Success|Failure} from w3up-client ([#1291](https://github.com/tx-ravenxbsw3/w3up/issues/1291)) ([5c5d17b](https://github.com/tx-ravenxbsw3/w3up/commit/5c5d17b3c02cc832ead98b966891ead46ec25847))
* expose accounts list on client instance ([#1109](https://github.com/tx-ravenxbsw3/w3up/issues/1109)) ([a9b64dd](https://github.com/tx-ravenxbsw3/w3up/commit/a9b64ddd1f899ad6929e3b3748feb53d0db43732))
* expose OwnedSpace and SharedSpace from access-client ([#1244](https://github.com/tx-ravenxbsw3/w3up/issues/1244)) ([a62f513](https://github.com/tx-ravenxbsw3/w3up/commit/a62f5135ac4cfcb06f0b6841b8aad3d154b48815))
* external login ([#1629](https://github.com/tx-ravenxbsw3/w3up/issues/1629)) ([638c31c](https://github.com/tx-ravenxbsw3/w3up/commit/638c31c5ae06fa73264b2fa45cd223fc2f7cc704))
* filecoin info ([#1091](https://github.com/tx-ravenxbsw3/w3up/issues/1091)) ([ad4e328](https://github.com/tx-ravenxbsw3/w3up/commit/ad4e32852f9f804163ef813bae47d2d430b6cac1))
* generate sharded DAG index on client and invoke w `index/add` ([#1451](https://github.com/tx-ravenxbsw3/w3up/issues/1451)) ([a1b3ee0](https://github.com/tx-ravenxbsw3/w3up/commit/a1b3ee0f3e82a92008d0ebb4bb386a5680ca70c1))
* get receipt support in client ([#1135](https://github.com/tx-ravenxbsw3/w3up/issues/1135)) ([c29950e](https://github.com/tx-ravenxbsw3/w3up/commit/c29950e7bb2d2744c1741c93774a06634b61957e))
* move aggregate information out of deals in filecoin/info ([#1192](https://github.com/tx-ravenxbsw3/w3up/issues/1192)) ([49e1363](https://github.com/tx-ravenxbsw3/w3up/commit/49e1363925acb1224e62f9ae4e9df4464cf6281d))
* port of https://github.com/storacha/upload-service/commit/2c12c23d13d14e9f1b79c34b8169f20975d431f7 ([#1641](https://github.com/tx-ravenxbsw3/w3up/issues/1641)) ([a7f964b](https://github.com/tx-ravenxbsw3/w3up/commit/a7f964b76442a66b9c94acd219fe3c099c999d82))
* re-export Store implementations from w3up-client ([#1266](https://github.com/tx-ravenxbsw3/w3up/issues/1266)) ([e803180](https://github.com/tx-ravenxbsw3/w3up/commit/e8031808fc0cc18affed63dad3cc8aabc02ee792))
* restrict store API to CARs ([#1415](https://github.com/tx-ravenxbsw3/w3up/issues/1415)) ([4a8bdb6](https://github.com/tx-ravenxbsw3/w3up/commit/4a8bdb69c4c7edec121ee4b53374cc30c5ee81b3))
* return allocated bytes in `store/add` receipt ([#1213](https://github.com/tx-ravenxbsw3/w3up/issues/1213)) ([a243e22](https://github.com/tx-ravenxbsw3/w3up/commit/a243e221153a8107ad92218f545d20ab1b3bd120))
* sharing spaces ([#1551](https://github.com/tx-ravenxbsw3/w3up/issues/1551)) ([866fc5d](https://github.com/tx-ravenxbsw3/w3up/commit/866fc5d4baedb90df2f48985d0b6a09034755c52))
* strictly require nodejs version ([#1264](https://github.com/tx-ravenxbsw3/w3up/issues/1264)) ([14c5b5b](https://github.com/tx-ravenxbsw3/w3up/commit/14c5b5b52b98ab256db72cf550bfeb750f522697))
* tweak readmes to get release-please to bump major version ([#1102](https://github.com/tx-ravenxbsw3/w3up/issues/1102)) ([88d2046](https://github.com/tx-ravenxbsw3/w3up/commit/88d2046db29013ac8df45d263860e7e2e059f291))
* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/tx-ravenxbsw3/w3up/issues/1312)) ([5ed0f70](https://github.com/tx-ravenxbsw3/w3up/commit/5ed0f708d74745ae86c6c69c436a7dffb9c9d7c8))
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/tx-ravenxbsw3/w3up/issues/1444)) ([bd4885b](https://github.com/tx-ravenxbsw3/w3up/commit/bd4885b3a88216cd3402749bd03fa4682e5a7495))
* usage/record capability definition ([#1562](https://github.com/tx-ravenxbsw3/w3up/issues/1562)) ([0cb6af9](https://github.com/tx-ravenxbsw3/w3up/commit/0cb6af9ac0954e3d9ee24f63ed86a5cfa1312ef0))
* utility exports for better UX ([#1505](https://github.com/tx-ravenxbsw3/w3up/issues/1505)) ([eb5736c](https://github.com/tx-ravenxbsw3/w3up/commit/eb5736cf8323bce7438309f3679fa82308e49f9e))
* w3up client login ([#1120](https://github.com/tx-ravenxbsw3/w3up/issues/1120)) ([171e5ab](https://github.com/tx-ravenxbsw3/w3up/commit/171e5ab18c004f79501bfecd54287a0ebae5906e))
* w3up-client new release ([#1569](https://github.com/tx-ravenxbsw3/w3up/issues/1569)) ([0a7a380](https://github.com/tx-ravenxbsw3/w3up/commit/0a7a380d2e9a111b6f065bb2c721ac6fc9830e5b))
* **w3up-client:** add default gateway authorization ([#1604](https://github.com/tx-ravenxbsw3/w3up/issues/1604)) ([42d6624](https://github.com/tx-ravenxbsw3/w3up/commit/42d6624d9194afef505f2d8044e7df73ac3ede7e))
* **w3up-client:** export additional modules ([#1110](https://github.com/tx-ravenxbsw3/w3up/issues/1110)) ([c8b3d54](https://github.com/tx-ravenxbsw3/w3up/commit/c8b3d54abe5f7c48d478dd1e80b67356293c7860))
* wait for plan selection ([#1547](https://github.com/tx-ravenxbsw3/w3up/issues/1547)) ([ca8a070](https://github.com/tx-ravenxbsw3/w3up/commit/ca8a070c5eb7a46cae939811b23f3e485c1a55c4))


### Fixes

* additional space setup steps ([#1284](https://github.com/tx-ravenxbsw3/w3up/issues/1284)) ([30b3be0](https://github.com/tx-ravenxbsw3/w3up/commit/30b3be0625de5ccac444df5bfa7baca6df13ff46))
* allow import memory store in the browser ([#1276](https://github.com/tx-ravenxbsw3/w3up/issues/1276)) ([8cb7ca6](https://github.com/tx-ravenxbsw3/w3up/commit/8cb7ca60603857b1da0332a9746bafbf812c15cd))
* authorize renamed to login in docs ([#1125](https://github.com/tx-ravenxbsw3/w3up/issues/1125)) ([4dca2be](https://github.com/tx-ravenxbsw3/w3up/commit/4dca2beb6bab8f0a5735c468e9fdbd14e9907058))
* badgers on README ([b3f5bf9](https://github.com/tx-ravenxbsw3/w3up/commit/b3f5bf97a4ea930824ba00511b9ce94e335f07ee))
* c8 issue ([7d4629c](https://github.com/tx-ravenxbsw3/w3up/commit/7d4629c6b67db25efba4eead2b1bd2af5a914b36))
* check for blob/accept receipts before blob/add is concluded ([#1459](https://github.com/tx-ravenxbsw3/w3up/issues/1459)) ([e7c3e50](https://github.com/tx-ravenxbsw3/w3up/commit/e7c3e50d3c39984d3b64aa633037faf530420ef5))
* copy src into dist in w3up-client ([#1239](https://github.com/tx-ravenxbsw3/w3up/issues/1239)) ([bfc917c](https://github.com/tx-ravenxbsw3/w3up/commit/bfc917c12244d484f887647b50639f549fc154f1))
* **egress/record:** rename capability ([#1572](https://github.com/tx-ravenxbsw3/w3up/issues/1572)) ([9cb5261](https://github.com/tx-ravenxbsw3/w3up/commit/9cb5261de19cb22109f03e9695adbf08b651cd63))
* export blob client ([#1485](https://github.com/tx-ravenxbsw3/w3up/issues/1485)) ([0c4cab8](https://github.com/tx-ravenxbsw3/w3up/commit/0c4cab813234fd3fb226457652462ae3e218b5a3))
* export filecoin types ([#1185](https://github.com/tx-ravenxbsw3/w3up/issues/1185)) ([e67516f](https://github.com/tx-ravenxbsw3/w3up/commit/e67516f46f04129eaa51d5e646f4a72eb76aee61))
* export new subscription, usage and filecoin clients ([#1111](https://github.com/tx-ravenxbsw3/w3up/issues/1111)) ([0ae6265](https://github.com/tx-ravenxbsw3/w3up/commit/0ae626538efb475ba2826e835e25a1eaa4064388))
* export ProgressStatus ([571c555](https://github.com/tx-ravenxbsw3/w3up/commit/571c555b1da4ac99408c77c712b1402f73baffda))
* floating promises and add no-floating-promises to eslint-config-w3up ([#1198](https://github.com/tx-ravenxbsw3/w3up/issues/1198)) ([3ad073f](https://github.com/tx-ravenxbsw3/w3up/commit/3ad073f1617fb929409ce44b012eb629378ae10b))
* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/tx-ravenxbsw3/w3up/issues/1141)) ([93980ef](https://github.com/tx-ravenxbsw3/w3up/commit/93980ef8759b01b689a017aa7ae5a06d83284948))
* look for the correct capability in `client.capability.upload.get` ([#1357](https://github.com/tx-ravenxbsw3/w3up/issues/1357)) ([a2e57be](https://github.com/tx-ravenxbsw3/w3up/commit/a2e57bee40a3378dd295231a2192b4d0fa95f1f0))
* make login idempotent ([#1149](https://github.com/tx-ravenxbsw3/w3up/issues/1149)) ([aa22141](https://github.com/tx-ravenxbsw3/w3up/commit/aa221417ce9c25eb3b7a6cf682f4dbc5b268c2ca))
* migrate repo ([#1389](https://github.com/tx-ravenxbsw3/w3up/issues/1389)) ([9e18c76](https://github.com/tx-ravenxbsw3/w3up/commit/9e18c761e63c88e395b66b4f7cbadc79fc837dec))
* missing export ([6595223](https://github.com/tx-ravenxbsw3/w3up/commit/6595223217afc2c85dc2f5059b0165eb6bc6472b))
* package metadata ([#1161](https://github.com/tx-ravenxbsw3/w3up/issues/1161)) ([68b41e4](https://github.com/tx-ravenxbsw3/w3up/commit/68b41e49f4e77aabe07594b22691b2febdb3ea91))
* publish location claim to content claims service ([#1571](https://github.com/tx-ravenxbsw3/w3up/issues/1571)) ([d1b0824](https://github.com/tx-ravenxbsw3/w3up/commit/d1b0824bc5a033982925a7896791c405e333c3d8))
* README with uploadDirectory, not store ([#1106](https://github.com/tx-ravenxbsw3/w3up/issues/1106)) ([167e732](https://github.com/tx-ravenxbsw3/w3up/commit/167e73200c17ee21e67b621e55542421cd169758))
* remove mention of registerSpace from w3up-client README ([#1214](https://github.com/tx-ravenxbsw3/w3up/issues/1214)) ([fc17887](https://github.com/tx-ravenxbsw3/w3up/commit/fc17887bcea41987236943baaf1836fd9ee5efef))
* rename blob and index client capabilities ([#1478](https://github.com/tx-ravenxbsw3/w3up/issues/1478)) ([ee5a89c](https://github.com/tx-ravenxbsw3/w3up/commit/ee5a89cac2248e634bd4e835270d052cdbb31aef))
* repo URLs ([#1550](https://github.com/tx-ravenxbsw3/w3up/issues/1550)) ([6fd5aa3](https://github.com/tx-ravenxbsw3/w3up/commit/6fd5aa32e9cfb5633ec662363e6a48493b1f8cf0))
* revert blob add by default ([#1456](https://github.com/tx-ravenxbsw3/w3up/issues/1456)) ([1dad15c](https://github.com/tx-ravenxbsw3/w3up/commit/1dad15c47487026fb92ba060d9117d53a4a9b7fd))
* test against actual api ([#1438](https://github.com/tx-ravenxbsw3/w3up/issues/1438)) ([851d5be](https://github.com/tx-ravenxbsw3/w3up/commit/851d5beb7fc2ed9d434d6a6105b262a9047023ff))
* thread abort signal through login functions ([#1189](https://github.com/tx-ravenxbsw3/w3up/issues/1189)) ([3022892](https://github.com/tx-ravenxbsw3/w3up/commit/30228928a2175122971a40631bd3b208253ef07f))
* trigger commit for release of w3up client ([#1070](https://github.com/tx-ravenxbsw3/w3up/issues/1070)) ([0b2d5a3](https://github.com/tx-ravenxbsw3/w3up/commit/0b2d5a3bb04d9f7aa9ec9a9d488b81ad92079845))
* trigger release ([d566ecc](https://github.com/tx-ravenxbsw3/w3up/commit/d566ecc6f61828efbd6a9ac08762da669a183387))
* trigger w3up client release with new client ([#1497](https://github.com/tx-ravenxbsw3/w3up/issues/1497)) ([45cbef0](https://github.com/tx-ravenxbsw3/w3up/commit/45cbef032bc82ed27d38168d50b677cb4ac71701))
* update "byo agent" example to match website snippet ([#1268](https://github.com/tx-ravenxbsw3/w3up/issues/1268)) ([c256938](https://github.com/tx-ravenxbsw3/w3up/commit/c256938def78c985456842b642cd93acfa7656fc))
* upgrade ucanto core ([#1127](https://github.com/tx-ravenxbsw3/w3up/issues/1127)) ([40b3257](https://github.com/tx-ravenxbsw3/w3up/commit/40b32571b42ff63f37d5020299ebb013e1886286))
* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/tx-ravenxbsw3/w3up/issues/1359)) ([6ca062f](https://github.com/tx-ravenxbsw3/w3up/commit/6ca062fad73a442b81553fc79fd75923ff9e1bcf))
* upload client does not need cors mode on presigned url put ([#1295](https://github.com/tx-ravenxbsw3/w3up/issues/1295)) ([031f5ec](https://github.com/tx-ravenxbsw3/w3up/commit/031f5ec83de134675e6096e552058903a69e4bbe))
* upload client should perform filecoin offer ([#1333](https://github.com/tx-ravenxbsw3/w3up/issues/1333)) ([52c5a1b](https://github.com/tx-ravenxbsw3/w3up/commit/52c5a1b2459739d7bd0ecd914c7c53bbe6cc4427))
* use configured receipts endpoint ([a1f586e](https://github.com/tx-ravenxbsw3/w3up/commit/a1f586ed213f081b4143fdf806815f83eb9ae221))
* use MultihashDigest type in stores ([#1474](https://github.com/tx-ravenxbsw3/w3up/issues/1474)) ([a364a17](https://github.com/tx-ravenxbsw3/w3up/commit/a364a1766d05ac9f69bc22bac6e9c946fd799c7e))
* **w3up-client:** authorize agent to use space ([#1610](https://github.com/tx-ravenxbsw3/w3up/issues/1610)) ([6c85851](https://github.com/tx-ravenxbsw3/w3up/commit/6c85851f494d22a8bd3e16295daee5af40caaf4b))
* **w3up-client:** options in createSpace should be optional ([#1613](https://github.com/tx-ravenxbsw3/w3up/issues/1613)) ([079907f](https://github.com/tx-ravenxbsw3/w3up/commit/079907f62fb8c49346e1b9bb2b624a97dfc3ce7c))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/tx-ravenxbsw3/w3up/issues/1533)) ([47cc600](https://github.com/tx-ravenxbsw3/w3up/commit/47cc6006b1b7316c6815dfdca0a55122f632fec3))
* appease linter ([0f49e0c](https://github.com/tx-ravenxbsw3/w3up/commit/0f49e0ce451946d909be4a788e934a126fec5812))
* c8 fix ([a380870](https://github.com/tx-ravenxbsw3/w3up/commit/a3808707e80b8f0572d54adcb6a67529897e453d))
* **capabilities:** top level filecoin cap ([#1606](https://github.com/tx-ravenxbsw3/w3up/issues/1606)) ([bf89593](https://github.com/tx-ravenxbsw3/w3up/commit/bf89593f48fcd041e1c12d144985406f139a4a7f))
* **main:** release w3up-client 10.0.0 ([#1099](https://github.com/tx-ravenxbsw3/w3up/issues/1099)) ([54cb5dd](https://github.com/tx-ravenxbsw3/w3up/commit/54cb5ddbdbdef05318596060cab13dfe13982ff9))
* **main:** release w3up-client 10.1.0 ([#1112](https://github.com/tx-ravenxbsw3/w3up/issues/1112)) ([00a78a5](https://github.com/tx-ravenxbsw3/w3up/commit/00a78a5732b1f4a2c6480b26b93fa59131c1dca3))
* **main:** release w3up-client 10.2.0 ([#1118](https://github.com/tx-ravenxbsw3/w3up/issues/1118)) ([ceeba90](https://github.com/tx-ravenxbsw3/w3up/commit/ceeba90184edf0a1966009bb55079bea30e15603))
* **main:** release w3up-client 10.3.0 ([#1121](https://github.com/tx-ravenxbsw3/w3up/issues/1121)) ([d227133](https://github.com/tx-ravenxbsw3/w3up/commit/d227133cd95662917c5f4a1bb807bd7640ccf982))
* **main:** release w3up-client 11.0.0 ([#1129](https://github.com/tx-ravenxbsw3/w3up/issues/1129)) ([39c4ff6](https://github.com/tx-ravenxbsw3/w3up/commit/39c4ff6ad86b74c6b4465fd8f4da547f901990c2))
* **main:** release w3up-client 11.0.1 ([#1144](https://github.com/tx-ravenxbsw3/w3up/issues/1144)) ([5192779](https://github.com/tx-ravenxbsw3/w3up/commit/51927791ce3fd6e714587aa3bffda97b76203574))
* **main:** release w3up-client 11.0.2 ([#1167](https://github.com/tx-ravenxbsw3/w3up/issues/1167)) ([1885a32](https://github.com/tx-ravenxbsw3/w3up/commit/1885a32b49f74b45a486a6fe1b5e9baad2739c5a))
* **main:** release w3up-client 11.1.0 ([#1179](https://github.com/tx-ravenxbsw3/w3up/issues/1179)) ([c4c9a71](https://github.com/tx-ravenxbsw3/w3up/commit/c4c9a71399785ba0d74b4cc9511ef7ab5fa90f57))
* **main:** release w3up-client 11.1.1 ([#1186](https://github.com/tx-ravenxbsw3/w3up/issues/1186)) ([30c7c86](https://github.com/tx-ravenxbsw3/w3up/commit/30c7c86628e8e0af8888fe86929b643b7fbd3f74))
* **main:** release w3up-client 11.1.2 ([#1187](https://github.com/tx-ravenxbsw3/w3up/issues/1187)) ([cdaa37b](https://github.com/tx-ravenxbsw3/w3up/commit/cdaa37ba981e2823a4f3ef6c71e4af33c19fe578))
* **main:** release w3up-client 11.1.3 ([#1190](https://github.com/tx-ravenxbsw3/w3up/issues/1190)) ([0f98e19](https://github.com/tx-ravenxbsw3/w3up/commit/0f98e195f1dcca9c28e1bea65f3c08461a0c09f1))
* **main:** release w3up-client 11.2.0 ([#1196](https://github.com/tx-ravenxbsw3/w3up/issues/1196)) ([4d29dc1](https://github.com/tx-ravenxbsw3/w3up/commit/4d29dc17c76d71ee859eca56f5ce3e1e38923c4c))
* **main:** release w3up-client 11.2.1 ([#1216](https://github.com/tx-ravenxbsw3/w3up/issues/1216)) ([00afc30](https://github.com/tx-ravenxbsw3/w3up/commit/00afc30bf156b72a8ecac8bcb641521eee83b024))
* **main:** release w3up-client 12.0.0 ([#1231](https://github.com/tx-ravenxbsw3/w3up/issues/1231)) ([3d49314](https://github.com/tx-ravenxbsw3/w3up/commit/3d49314bc9e3b826094720b305316ce46b07f86a))
* **main:** release w3up-client 12.1.0 ([#1256](https://github.com/tx-ravenxbsw3/w3up/issues/1256)) ([10a843d](https://github.com/tx-ravenxbsw3/w3up/commit/10a843d4f68b40aa63822b3edfc94140fa39e75b))
* **main:** release w3up-client 12.2.0 ([#1270](https://github.com/tx-ravenxbsw3/w3up/issues/1270)) ([810013e](https://github.com/tx-ravenxbsw3/w3up/commit/810013e6ee8962e164365ddc47fb049d2f5bffd9))
* **main:** release w3up-client 12.2.1 ([#1277](https://github.com/tx-ravenxbsw3/w3up/issues/1277)) ([4c5e7b6](https://github.com/tx-ravenxbsw3/w3up/commit/4c5e7b632b27ce112736db709df2f481c408e1cf))
* **main:** release w3up-client 12.3.0 ([#1285](https://github.com/tx-ravenxbsw3/w3up/issues/1285)) ([68baeb7](https://github.com/tx-ravenxbsw3/w3up/commit/68baeb7f6a966a44de95b8fd8303a6ad8b84148a))
* **main:** release w3up-client 12.4.0 ([#1286](https://github.com/tx-ravenxbsw3/w3up/issues/1286)) ([efbb469](https://github.com/tx-ravenxbsw3/w3up/commit/efbb469144b0a1072291c7822a6c3a5379100eaa))
* **main:** release w3up-client 12.4.1 ([#1297](https://github.com/tx-ravenxbsw3/w3up/issues/1297)) ([61fe30a](https://github.com/tx-ravenxbsw3/w3up/commit/61fe30a4cd32355b196445b299d8b3f4f3e54778))
* **main:** release w3up-client 12.5.0 ([#1313](https://github.com/tx-ravenxbsw3/w3up/issues/1313)) ([7609aac](https://github.com/tx-ravenxbsw3/w3up/commit/7609aacf72c523097b15991039428b89477f699b))
* **main:** release w3up-client 12.5.1 ([#1358](https://github.com/tx-ravenxbsw3/w3up/issues/1358)) ([033b75f](https://github.com/tx-ravenxbsw3/w3up/commit/033b75f1d4b60621408759c767e3509ca0576534))
* **main:** release w3up-client 12.5.2 ([#1364](https://github.com/tx-ravenxbsw3/w3up/issues/1364)) ([8246e84](https://github.com/tx-ravenxbsw3/w3up/commit/8246e84657d1364d55939bd5f62d54c5d8593640))
* **main:** release w3up-client 12.5.3 ([#1394](https://github.com/tx-ravenxbsw3/w3up/issues/1394)) ([81fe04a](https://github.com/tx-ravenxbsw3/w3up/commit/81fe04a59ebea78048065bdcfed19cfa102681ef))
* **main:** release w3up-client 13.0.0 ([#1416](https://github.com/tx-ravenxbsw3/w3up/issues/1416)) ([7dc3304](https://github.com/tx-ravenxbsw3/w3up/commit/7dc33048c21654bd8b28879a6883de19613ec849))
* **main:** release w3up-client 13.0.1 ([#1431](https://github.com/tx-ravenxbsw3/w3up/issues/1431)) ([e8e898b](https://github.com/tx-ravenxbsw3/w3up/commit/e8e898b51951ebdca8fef3834c948f98902bd577))
* **main:** release w3up-client 13.1.0 ([#1440](https://github.com/tx-ravenxbsw3/w3up/issues/1440)) ([74e7e89](https://github.com/tx-ravenxbsw3/w3up/commit/74e7e89377e61b2219be0d478804587ad8f187df))
* **main:** release w3up-client 13.1.1 ([#1457](https://github.com/tx-ravenxbsw3/w3up/issues/1457)) ([32367f4](https://github.com/tx-ravenxbsw3/w3up/commit/32367f4232336eb978ed903db545d79108def146))
* **main:** release w3up-client 14.0.0 ([#1464](https://github.com/tx-ravenxbsw3/w3up/issues/1464)) ([c20c807](https://github.com/tx-ravenxbsw3/w3up/commit/c20c8070219b9d548f9b2b4919ccb99732e2eeb0))
* **main:** release w3up-client 14.1.0 ([#1492](https://github.com/tx-ravenxbsw3/w3up/issues/1492)) ([4893f26](https://github.com/tx-ravenxbsw3/w3up/commit/4893f2684572514577693c25e1bdb46d8d309d01))
* **main:** release w3up-client 14.1.1 ([#1498](https://github.com/tx-ravenxbsw3/w3up/issues/1498)) ([471c1fe](https://github.com/tx-ravenxbsw3/w3up/commit/471c1fe4b7e3088b88fe4969f40f1a65c7002c60))
* **main:** release w3up-client 15.0.0 ([#1504](https://github.com/tx-ravenxbsw3/w3up/issues/1504)) ([0421299](https://github.com/tx-ravenxbsw3/w3up/commit/042129946a76af704f8ee4513c92c3d7203d9d67))
* **main:** release w3up-client 16.0.0 ([#1508](https://github.com/tx-ravenxbsw3/w3up/issues/1508)) ([8b4e341](https://github.com/tx-ravenxbsw3/w3up/commit/8b4e341204c46e118d63546e50ca53eea21c3406))
* **main:** release w3up-client 16.1.0 ([#1538](https://github.com/tx-ravenxbsw3/w3up/issues/1538)) ([0c6f48c](https://github.com/tx-ravenxbsw3/w3up/commit/0c6f48c46e7fb4b63f3fce623124f6e6dae3f47a))
* **main:** release w3up-client 16.1.1 ([#1549](https://github.com/tx-ravenxbsw3/w3up/issues/1549)) ([45e5b43](https://github.com/tx-ravenxbsw3/w3up/commit/45e5b4364300ed43c999f8cfd211f3b56d1d300d))
* **main:** release w3up-client 16.2.0 ([#1552](https://github.com/tx-ravenxbsw3/w3up/issues/1552)) ([48f074b](https://github.com/tx-ravenxbsw3/w3up/commit/48f074badd7fd89fec56c7e9d8379a809241d844))
* **main:** release w3up-client 16.3.0 ([#1568](https://github.com/tx-ravenxbsw3/w3up/issues/1568)) ([403bbbc](https://github.com/tx-ravenxbsw3/w3up/commit/403bbbc1f0471ffe3ba1e1b4fce1417b37962d24))
* **main:** release w3up-client 16.4.0 ([#1570](https://github.com/tx-ravenxbsw3/w3up/issues/1570)) ([7cbe176](https://github.com/tx-ravenxbsw3/w3up/commit/7cbe176fb2624cb3b9f1af651061efe16910396a))
* **main:** release w3up-client 16.4.1 ([#1575](https://github.com/tx-ravenxbsw3/w3up/issues/1575)) ([951c105](https://github.com/tx-ravenxbsw3/w3up/commit/951c105d7214b765fe6c258925435c6cf39c337c))
* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/tx-ravenxbsw3/w3up/issues/1577)) ([bdaa5e2](https://github.com/tx-ravenxbsw3/w3up/commit/bdaa5e297fef7e7ddca6a63c12ab071000cc7d2b))
* **main:** release w3up-client 16.5.0 ([#1582](https://github.com/tx-ravenxbsw3/w3up/issues/1582)) ([bd6d1b7](https://github.com/tx-ravenxbsw3/w3up/commit/bd6d1b71312bae1804f283f2d2c2e2f387e0cd77))
* **main:** release w3up-client 16.5.1 ([#1587](https://github.com/tx-ravenxbsw3/w3up/issues/1587)) ([7c7d76f](https://github.com/tx-ravenxbsw3/w3up/commit/7c7d76f32e5467f401a3e4fed1463de6dfe4b086))
* **main:** release w3up-client 16.5.2 ([#1594](https://github.com/tx-ravenxbsw3/w3up/issues/1594)) ([ed6484d](https://github.com/tx-ravenxbsw3/w3up/commit/ed6484d3be004f757bffcf8b19c24be657eb9101))
* **main:** release w3up-client 17.0.0 ([#1598](https://github.com/tx-ravenxbsw3/w3up/issues/1598)) ([b839d8a](https://github.com/tx-ravenxbsw3/w3up/commit/b839d8a7a53b59fb7c8ec83d352afed28d85b687))
* **main:** release w3up-client 17.1.0 ([#1608](https://github.com/tx-ravenxbsw3/w3up/issues/1608)) ([8da8039](https://github.com/tx-ravenxbsw3/w3up/commit/8da80394adc353cdb633c7e5e2b62cd96307c76e))
* **main:** release w3up-client 17.1.1 ([#1611](https://github.com/tx-ravenxbsw3/w3up/issues/1611)) ([4a6417c](https://github.com/tx-ravenxbsw3/w3up/commit/4a6417cb142b95b8815d46c1b9ed717f48af8911))
* **main:** release w3up-client 17.1.2 ([#1614](https://github.com/tx-ravenxbsw3/w3up/issues/1614)) ([c826535](https://github.com/tx-ravenxbsw3/w3up/commit/c82653574d1eb36e6c347ee3a6ba6aecf840cc7b))
* **main:** release w3up-client 17.2.0 ([#1632](https://github.com/tx-ravenxbsw3/w3up/issues/1632)) ([c13dc12](https://github.com/tx-ravenxbsw3/w3up/commit/c13dc12f2e375eca2b3514d0ec112178c4013240))
* **main:** release w3up-client 17.3.0 ([#1643](https://github.com/tx-ravenxbsw3/w3up/issues/1643)) ([63e9be2](https://github.com/tx-ravenxbsw3/w3up/commit/63e9be20dc8daa001963baf958c833a994f5c1f5))
* **main:** release w3up-client 9.2.2 ([#1071](https://github.com/tx-ravenxbsw3/w3up/issues/1071)) ([1db2427](https://github.com/tx-ravenxbsw3/w3up/commit/1db2427925da9f4942ebcfa55422442eff29137e))
* **main:** release w3up-client 9.3.0 ([#1083](https://github.com/tx-ravenxbsw3/w3up/issues/1083)) ([d831305](https://github.com/tx-ravenxbsw3/w3up/commit/d831305fda873a3d08f4e5be55c195548a0d182f))
* no longer depends on hd-scripts, packages use/configure eslint directly, fixes warnings from npm lint script ([#1058](https://github.com/tx-ravenxbsw3/w3up/issues/1058)) ([3a99cc0](https://github.com/tx-ravenxbsw3/w3up/commit/3a99cc02941f9d563cac1838e1e67a3faa42c3de))

## [17.3.0](https://github.com/storacha/w3up/compare/w3up-client-v17.2.0...w3up-client-v17.3.0) (2025-05-21)


### Features

* port of https://github.com/storacha/upload-service/commit/2c12c23d13d14e9f1b79c34b8169f20975d431f7 ([#1641](https://github.com/storacha/w3up/issues/1641)) ([8eb4306](https://github.com/storacha/w3up/commit/8eb43061b184e222f6aaf10d69a0129225858a6f))

## [17.2.0](https://github.com/storacha/w3up/compare/w3up-client-v17.1.2...w3up-client-v17.2.0) (2025-02-25)


### Features

* external login ([#1629](https://github.com/storacha/w3up/issues/1629)) ([150b5d7](https://github.com/storacha/w3up/commit/150b5d7c55ca92becbabab969285497fbba86268))

## [17.1.2](https://github.com/storacha/w3up/compare/w3up-client-v17.1.1...w3up-client-v17.1.2) (2025-01-08)


### Fixes

* **w3up-client:** options in createSpace should be optional ([#1613](https://github.com/storacha/w3up/issues/1613)) ([52ccfc2](https://github.com/storacha/w3up/commit/52ccfc2b8208b9e58e37868d0e40e35ef647032c))

## [17.1.1](https://github.com/storacha/w3up/compare/w3up-client-v17.1.0...w3up-client-v17.1.1) (2024-12-20)


### Fixes

* **w3up-client:** authorize agent to use space ([#1610](https://github.com/storacha/w3up/issues/1610)) ([52ceb12](https://github.com/storacha/w3up/commit/52ceb12e29e04ab76f9863c17542088291685890))

## [17.1.0](https://github.com/storacha/w3up/compare/w3up-client-v17.0.0...w3up-client-v17.1.0) (2024-12-19)


### Features

* **w3up-client:** add default gateway authorization ([#1604](https://github.com/storacha/w3up/issues/1604)) ([e669b55](https://github.com/storacha/w3up/commit/e669b5596aa65ec0c93b1cfd199217d64771aba4))


### Other Changes

* **capabilities:** top level filecoin cap ([#1606](https://github.com/storacha/w3up/issues/1606)) ([22d0bf9](https://github.com/storacha/w3up/commit/22d0bf9e540ffb8b76eb79453c4d881195abf2ef))

## [17.0.0](https://github.com/storacha/w3up/compare/w3up-client-v16.5.2...w3up-client-v17.0.0) (2024-12-09)


### ⚠ BREAKING CHANGES

* content serve authorization ([#1590](https://github.com/storacha/w3up/issues/1590))

### Features

* content serve authorization ([#1590](https://github.com/storacha/w3up/issues/1590)) ([8b553a5](https://github.com/storacha/w3up/commit/8b553a53253f55a3f0a2980557fa5c3b92427f3f))

## [16.5.2](https://github.com/storacha/w3up/compare/w3up-client-v16.5.1...w3up-client-v16.5.2) (2024-11-29)


### Fixes

* publish location claim to content claims service ([#1571](https://github.com/storacha/w3up/issues/1571)) ([fb08e0e](https://github.com/storacha/w3up/commit/fb08e0e11ed482fe8996d4dc7535c45fbcc373b7))

## [16.5.1](https://github.com/storacha/w3up/compare/w3up-client-v16.5.0...w3up-client-v16.5.1) (2024-11-20)


### Fixes

* use configured receipts endpoint ([882d1c5](https://github.com/storacha/w3up/commit/882d1c5bda412103fa7d635f4ef1b99c1782e17a))

## [16.5.0](https://github.com/storacha/w3up/compare/w3up-client-v16.4.1...w3up-client-v16.5.0) (2024-11-17)


### Features

* add pre-built browser bundle ([#1586](https://github.com/storacha/w3up/issues/1586)) ([2fd07e7](https://github.com/storacha/w3up/commit/2fd07e7c2337ca5ea4eff265338976b34ad0bf27))


### Other Changes

* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/storacha/w3up/issues/1577)) ([1482d69](https://github.com/storacha/w3up/commit/1482d69c28baff1c27b1baf5f3e5c76f844e5576))

## [16.4.1](https://github.com/storacha/w3up/compare/w3up-client-v16.4.0...w3up-client-v16.4.1) (2024-11-05)


### Fixes

* **egress/record:** rename capability ([#1572](https://github.com/storacha/w3up/issues/1572)) ([d28691c](https://github.com/storacha/w3up/commit/d28691c4709f4e7c5ba81e042cac9e961c273bc9))

## [16.4.0](https://github.com/storacha/w3up/compare/w3up-client-v16.3.0...w3up-client-v16.4.0) (2024-10-24)


### Features

* w3up-client new release ([#1569](https://github.com/storacha/w3up/issues/1569)) ([6989e6e](https://github.com/storacha/w3up/commit/6989e6ecb334dcbf79c5a5cf7f4854ac452c6ef4))

## [16.3.0](https://github.com/storacha/w3up/compare/w3up-client-v16.2.0...w3up-client-v16.3.0) (2024-10-24)


### Features

* usage/record capability definition ([#1562](https://github.com/storacha/w3up/issues/1562)) ([98c8a87](https://github.com/storacha/w3up/commit/98c8a87c52ef88da728225259e77f65733d2d7e6))

## [16.2.0](https://github.com/storacha/w3up/compare/w3up-client-v16.1.1...w3up-client-v16.2.0) (2024-09-20)


### Features

* sharing spaces ([#1551](https://github.com/storacha/w3up/issues/1551)) ([7deb9a4](https://github.com/storacha/w3up/commit/7deb9a47fa0e37da0cf12a8d89214e45cf09bcbb))


### Fixes

* repo URLs ([#1550](https://github.com/storacha/w3up/issues/1550)) ([e02ddf3](https://github.com/storacha/w3up/commit/e02ddf3696553b03f8d2f7316de0a99a9303a60f))

## [16.1.1](https://github.com/storacha/w3up/compare/w3up-client-v16.1.0...w3up-client-v16.1.1) (2024-09-16)


### Fixes

* trigger release ([9eadccc](https://github.com/storacha/w3up/commit/9eadcccb7aac944ea571acf5f39e9880b2914168))

## [16.1.0](https://github.com/storacha/w3up/compare/w3up-client-v16.0.0...w3up-client-v16.1.0) (2024-09-16)


### Features

* **client:** optional account recovery ([#1546](https://github.com/storacha/w3up/issues/1546)) ([ea02adb](https://github.com/storacha/w3up/commit/ea02adb77cfe207a5823e24d886d28b6650ecc03))
* wait for plan selection ([#1547](https://github.com/storacha/w3up/issues/1547)) ([7fdee77](https://github.com/storacha/w3up/commit/7fdee77cb35326807a59f368c2276f945c256874))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/storacha/w3up/issues/1533)) ([07970ef](https://github.com/storacha/w3up/commit/07970efd443149158ebbfb2c4e745b5007eb9407))

## [16.0.0](https://github.com/storacha-network/w3up/compare/w3up-client-v15.0.0...w3up-client-v16.0.0) (2024-07-29)


### ⚠ BREAKING CHANGES

* allow invocation configuration to be generated on demand ([#1507](https://github.com/storacha-network/w3up/issues/1507))

### Features

* allow invocation configuration to be generated on demand ([#1507](https://github.com/storacha-network/w3up/issues/1507)) ([fd74cbb](https://github.com/storacha-network/w3up/commit/fd74cbb9a59c10f1688a5994dd2cdc6722be00be))
* configure UnixFS encoder ([#1509](https://github.com/storacha-network/w3up/issues/1509)) ([1a5e648](https://github.com/storacha-network/w3up/commit/1a5e64817d20525c456b78eea22da8189b5748b1))


### Fixes

* badgers on README ([ffe49f2](https://github.com/storacha-network/w3up/commit/ffe49f2be3f0a550d7561bc5ebb124de1b913735))

## [15.0.0](https://github.com/storacha-network/w3up/compare/w3up-client-v14.1.1...w3up-client-v15.0.0) (2024-06-13)


### ⚠ BREAKING CHANGES

* `AllocationsStorage` and `BlobsStorage` methods not take `MultihashDigest` types instead of `Uint8Array`s.

### Features

* utility exports for better UX ([#1505](https://github.com/storacha-network/w3up/issues/1505)) ([54b0d93](https://github.com/storacha-network/w3up/commit/54b0d93eb1994022c935b30a0b238d825e9e93a0))


### Fixes

* use MultihashDigest type in stores ([#1474](https://github.com/storacha-network/w3up/issues/1474)) ([6c6a3bd](https://github.com/storacha-network/w3up/commit/6c6a3bdcb924cf6f9a4723f710a27f1ae34ca560))

## [14.1.1](https://github.com/w3s-project/w3up/compare/w3up-client-v14.1.0...w3up-client-v14.1.1) (2024-06-05)


### Fixes

* trigger w3up client release with new client ([#1497](https://github.com/w3s-project/w3up/issues/1497)) ([9616f0d](https://github.com/w3s-project/w3up/commit/9616f0d64d342e2e1c9524e900549ff94471a10e))

## [14.1.0](https://github.com/w3s-project/w3up/compare/w3up-client-v14.0.0...w3up-client-v14.1.0) (2024-06-04)


### Features

* add blob/get ([#1484](https://github.com/w3s-project/w3up/issues/1484)) ([328039d](https://github.com/w3s-project/w3up/commit/328039d8a29fec3c1bbab28d1bb9de1643f54f71))

## [14.0.0](https://github.com/w3s-project/w3up/compare/w3up-client-v13.1.1...w3up-client-v14.0.0) (2024-06-04)


### ⚠ BREAKING CHANGES

* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/w3s-project/w3up/issues/1444))
* delegated capabilities required to use `uploadFile`, `uploadDirectory` and `uploadCAR` have changed. In order to use these methods your agent will now need to be delegated `blob/add`, `index/add`, `filecoin/offer` and `upload/add` capabilities. Note: no code changes are required.

### Features

* generate sharded DAG index on client and invoke w `index/add` ([#1451](https://github.com/w3s-project/w3up/issues/1451)) ([a6d9026](https://github.com/w3s-project/w3up/commit/a6d9026536e60c0ce93b613acc6e337f2a21aeb2))
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/w3s-project/w3up/issues/1444)) ([c9bf33e](https://github.com/w3s-project/w3up/commit/c9bf33e5512397a654db933a5e6b5db0c7c22da5))


### Fixes

* check for blob/accept receipts before blob/add is concluded ([#1459](https://github.com/w3s-project/w3up/issues/1459)) ([462518c](https://github.com/w3s-project/w3up/commit/462518ca832515c65cc674e8aef3c28f2228797d))
* export blob client ([#1485](https://github.com/w3s-project/w3up/issues/1485)) ([7944077](https://github.com/w3s-project/w3up/commit/7944077d91d5dd154bac2760dff831a41d4f814b))
* rename blob and index client capabilities ([#1478](https://github.com/w3s-project/w3up/issues/1478)) ([17e3a31](https://github.com/w3s-project/w3up/commit/17e3a3161c6585b1844abcf7ed27252fa8580870))

## [13.1.1](https://github.com/w3s-project/w3up/compare/w3up-client-v13.1.0...w3up-client-v13.1.1) (2024-05-15)


### Fixes

* revert blob add by default ([#1456](https://github.com/w3s-project/w3up/issues/1456)) ([b77ec75](https://github.com/w3s-project/w3up/commit/b77ec750c3911f6f47fa32a5e1560858b347985c))

## [13.1.0](https://github.com/w3s-project/w3up/compare/w3up-client-v13.0.1...w3up-client-v13.1.0) (2024-05-14)


### Features

* add "plan/create-admin-session" capability ([#1411](https://github.com/w3s-project/w3up/issues/1411)) ([50eeeb5](https://github.com/w3s-project/w3up/commit/50eeeb502335ba0413318b5047869a275901824b))
* add blob protocol to upload-client ([#1425](https://github.com/w3s-project/w3up/issues/1425)) ([49aef56](https://github.com/w3s-project/w3up/commit/49aef564a726d34dbbedbd83f5366d9320180f99))


### Fixes

* test against actual api ([#1438](https://github.com/w3s-project/w3up/issues/1438)) ([f8132ca](https://github.com/w3s-project/w3up/commit/f8132ca1fced72a4addc7e9f0a2162e823c1ea5f))

## [13.0.1](https://github.com/w3s-project/w3up/compare/w3up-client-v13.0.0...w3up-client-v13.0.1) (2024-05-07)


### Fixes

* c8 issue ([f5055b7](https://github.com/w3s-project/w3up/commit/f5055b7ff4ee9974611805a58dd274974e69c56e))
* missing export ([d72d083](https://github.com/w3s-project/w3up/commit/d72d083f8815245be2562a7d7e6aabe0c4cc4b45))


### Other Changes

* appease linter ([782c6d0](https://github.com/w3s-project/w3up/commit/782c6d0b3ca93ee801b38126339a262bcd713ede))
* c8 fix ([049170d](https://github.com/w3s-project/w3up/commit/049170d45678257161ac22b55068b2adf96a7ebb))

## [13.0.0](https://github.com/w3s-project/w3up/compare/w3up-client-v12.5.3...w3up-client-v13.0.0) (2024-04-29)


### ⚠ BREAKING CHANGES

* restrict store API to CARs ([#1415](https://github.com/w3s-project/w3up/issues/1415))

### Features

* restrict store API to CARs ([#1415](https://github.com/w3s-project/w3up/issues/1415)) ([e53aa87](https://github.com/w3s-project/w3up/commit/e53aa87780446458ef9a19c88877073c1470d50e))

## [12.5.3](https://github.com/w3s-project/w3up/compare/w3up-client-v12.5.2...w3up-client-v12.5.3) (2024-04-25)


### Fixes

* migrate repo ([#1389](https://github.com/w3s-project/w3up/issues/1389)) ([475a287](https://github.com/w3s-project/w3up/commit/475a28743ff9f7138b46dfe4227d3c80ed75a6a2))

## [12.5.2](https://github.com/web3-storage/w3up/compare/w3up-client-v12.5.1...w3up-client-v12.5.2) (2024-04-12)


### Fixes

* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/web3-storage/w3up/issues/1359)) ([87ca098](https://github.com/web3-storage/w3up/commit/87ca098186fe204ff3409a2684719f1c54148c97))

## [12.5.1](https://github.com/web3-storage/w3up/compare/w3up-client-v12.5.0...w3up-client-v12.5.1) (2024-04-11)


### Fixes

* look for the correct capability in `client.capability.upload.get` ([#1357](https://github.com/web3-storage/w3up/issues/1357)) ([77199fe](https://github.com/web3-storage/w3up/commit/77199fe2261355f9c24fa06ab6aa5aad419e649a))

## [12.5.0](https://github.com/web3-storage/w3up/compare/w3up-client-v12.4.1...w3up-client-v12.5.0) (2024-03-21)


### Features

* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/web3-storage/w3up/issues/1312)) ([d6978d7](https://github.com/web3-storage/w3up/commit/d6978d7ab299be76987c6533d18e6857f6998fe6))


### Fixes

* upload client should perform filecoin offer ([#1333](https://github.com/web3-storage/w3up/issues/1333)) ([466e3f7](https://github.com/web3-storage/w3up/commit/466e3f79733c30f864cb21e7ed0f0684945417ed))

## [12.4.1](https://github.com/web3-storage/w3up/compare/w3up-client-v12.4.0...w3up-client-v12.4.1) (2024-02-01)


### Fixes

* upload client does not need cors mode on presigned url put ([#1295](https://github.com/web3-storage/w3up/issues/1295)) ([ef70a2b](https://github.com/web3-storage/w3up/commit/ef70a2b45d98583842c95980e5c6de5d20870e0d))

## [12.4.0](https://github.com/web3-storage/w3up/compare/w3up-client-v12.3.0...w3up-client-v12.4.0) (2024-01-30)


### Features

* export PlanSet{Success|Failure} from w3up-client ([#1291](https://github.com/web3-storage/w3up/issues/1291)) ([47a2954](https://github.com/web3-storage/w3up/commit/47a2954630097df220d1998f29a9026764b7e76c))


### Fixes

* additional space setup steps ([#1284](https://github.com/web3-storage/w3up/issues/1284)) ([42804ff](https://github.com/web3-storage/w3up/commit/42804ff8b123874389f63f3b5387e6a578c3bbc9))

## [12.3.0](https://github.com/web3-storage/w3up/compare/w3up-client-v12.2.1...w3up-client-v12.3.0) (2024-01-29)


### Features

* add `set` method to `AccountPlan` ([#1281](https://github.com/web3-storage/w3up/issues/1281)) ([b94f0d4](https://github.com/web3-storage/w3up/commit/b94f0d48ea71454cef867feb9291c500f676faa3))

## [12.2.1](https://github.com/web3-storage/w3up/compare/w3up-client-v12.2.0...w3up-client-v12.2.1) (2024-01-24)


### Fixes

* allow import memory store in the browser ([#1276](https://github.com/web3-storage/w3up/issues/1276)) ([301e0fc](https://github.com/web3-storage/w3up/commit/301e0fcb8941c0a517d270c9b731b24cbdf00eb9))

## [12.2.0](https://github.com/web3-storage/w3up/compare/w3up-client-v12.1.0...w3up-client-v12.2.0) (2024-01-24)


### Features

* add remove high level function to client ([#1248](https://github.com/web3-storage/w3up/issues/1248)) ([104b8de](https://github.com/web3-storage/w3up/commit/104b8deaf487320f682540aff7fbeede26eca861))


### Fixes

* update "byo agent" example to match website snippet ([#1268](https://github.com/web3-storage/w3up/issues/1268)) ([e34eed1](https://github.com/web3-storage/w3up/commit/e34eed1fa3d6ef24ce2c01982764f2012dbf30d8))

## [12.1.0](https://github.com/web3-storage/w3up/compare/w3up-client-v12.0.0...w3up-client-v12.1.0) (2024-01-17)


### Features

* add a function to verify and return Abilities. ([#1252](https://github.com/web3-storage/w3up/issues/1252)) ([2f026a2](https://github.com/web3-storage/w3up/commit/2f026a2483a4f323c4e2c6a8a8cb10afd92e21c4))
* re-export Store implementations from w3up-client ([#1266](https://github.com/web3-storage/w3up/issues/1266)) ([b3c6b46](https://github.com/web3-storage/w3up/commit/b3c6b4608b5aa66290128613e029c70a870b05f1))
* strictly require nodejs version ([#1264](https://github.com/web3-storage/w3up/issues/1264)) ([bc9f427](https://github.com/web3-storage/w3up/commit/bc9f4279aa509ebf2a90b54fa6e68a962621b37a))

## [12.0.0](https://github.com/web3-storage/w3up/compare/w3up-client-v11.2.1...w3up-client-v12.0.0) (2024-01-03)


### ⚠ BREAKING CHANGES

* return allocated bytes in `store/add` receipt ([#1213](https://github.com/web3-storage/w3up/issues/1213))

### Features

* expose OwnedSpace and SharedSpace from access-client ([#1244](https://github.com/web3-storage/w3up/issues/1244)) ([8ec1b44](https://github.com/web3-storage/w3up/commit/8ec1b446590399aa236904c1b6937b7be5d83054))
* return allocated bytes in `store/add` receipt ([#1213](https://github.com/web3-storage/w3up/issues/1213)) ([5d52e44](https://github.com/web3-storage/w3up/commit/5d52e447c14e7f7fd334e7ff575e032b7b0d89d7))


### Fixes

* copy src into dist in w3up-client ([#1239](https://github.com/web3-storage/w3up/issues/1239)) ([468bb79](https://github.com/web3-storage/w3up/commit/468bb79cfd6cbc7d513d0174da5b3b43a3f82cba))

## [11.2.1](https://github.com/web3-storage/w3up/compare/w3up-client-v11.2.0...w3up-client-v11.2.1) (2023-12-07)


### Fixes

* remove mention of registerSpace from w3up-client README ([#1214](https://github.com/web3-storage/w3up/issues/1214)) ([38c5b37](https://github.com/web3-storage/w3up/commit/38c5b3762b71e5cf70fe5d916c27b85cbfbb8c73))

## [11.2.0](https://github.com/web3-storage/w3up/compare/w3up-client-v11.1.3...w3up-client-v11.2.0) (2023-11-29)


### Features

* move aggregate information out of deals in filecoin/info ([#1192](https://github.com/web3-storage/w3up/issues/1192)) ([18dc590](https://github.com/web3-storage/w3up/commit/18dc590ad50a023ef3094bfc1a2d729459e5d68e))


### Fixes

* floating promises and add no-floating-promises to eslint-config-w3up ([#1198](https://github.com/web3-storage/w3up/issues/1198)) ([1b8c5aa](https://github.com/web3-storage/w3up/commit/1b8c5aa86ec3d177bf77df4e2916699c1f522598))

## [11.1.3](https://github.com/web3-storage/w3up/compare/w3up-client-v11.1.2...w3up-client-v11.1.3) (2023-11-28)


### Fixes

* thread abort signal through login functions ([#1189](https://github.com/web3-storage/w3up/issues/1189)) ([8e908a9](https://github.com/web3-storage/w3up/commit/8e908a9fbacaedb40fdaf214f862720fb8454fca))

## [11.1.2](https://github.com/web3-storage/w3up/compare/w3up-client-v11.1.1...w3up-client-v11.1.2) (2023-11-27)


### Fixes

* export ProgressStatus ([ab29c05](https://github.com/web3-storage/w3up/commit/ab29c05a05390e63538ef71ed2dd1f65dbb326d5))

## [11.1.1](https://github.com/web3-storage/w3up/compare/w3up-client-v11.1.0...w3up-client-v11.1.1) (2023-11-27)


### Fixes

* export filecoin types ([#1185](https://github.com/web3-storage/w3up/issues/1185)) ([9b1f526](https://github.com/web3-storage/w3up/commit/9b1f52609903b40d965d51a87f8ba7a530ca74cd))

## [11.1.0](https://github.com/web3-storage/w3up/compare/w3up-client-v11.0.2...w3up-client-v11.1.0) (2023-11-25)


### Features

* add store.get and upload.get to clients ([#1178](https://github.com/web3-storage/w3up/issues/1178)) ([d1be42a](https://github.com/web3-storage/w3up/commit/d1be42a642e04d290710e824dc4c9b924de8d8ac))

## [11.0.2](https://github.com/web3-storage/w3up/compare/w3up-client-v11.0.1...w3up-client-v11.0.2) (2023-11-20)


### Bug Fixes

* package metadata ([#1161](https://github.com/web3-storage/w3up/issues/1161)) ([b8a1cc2](https://github.com/web3-storage/w3up/commit/b8a1cc2e125a91be582998bda295e1ae1caab087))

## [11.0.1](https://github.com/web3-storage/w3up/compare/w3up-client-v11.0.0...w3up-client-v11.0.1) (2023-11-16)


### Bug Fixes

* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/web3-storage/w3up/issues/1141)) ([0b8d3f3](https://github.com/web3-storage/w3up/commit/0b8d3f3b52918b1b4d3b76ea6fea3fb0c837cd73))
* make login idempotent ([#1149](https://github.com/web3-storage/w3up/issues/1149)) ([c1df8d8](https://github.com/web3-storage/w3up/commit/c1df8d8a2cfcf3a8706028a367b1d6b75f5ebb4f))

## [11.0.0](https://github.com/web3-storage/w3up/compare/w3up-client-v10.3.0...w3up-client-v11.0.0) (2023-11-15)


### ⚠ BREAKING CHANGES

* coupon ([#1136](https://github.com/web3-storage/w3up/issues/1136))

### Features

* coupon ([#1136](https://github.com/web3-storage/w3up/issues/1136)) ([1b94f2d](https://github.com/web3-storage/w3up/commit/1b94f2d3f6538d717d38b21dcb76657fd1f3e268))
* get receipt support in client ([#1135](https://github.com/web3-storage/w3up/issues/1135)) ([660d088](https://github.com/web3-storage/w3up/commit/660d0886e468d373b142470b50282b231e645d19))


### Bug Fixes

* upgrade ucanto core ([#1127](https://github.com/web3-storage/w3up/issues/1127)) ([5ce4d22](https://github.com/web3-storage/w3up/commit/5ce4d2292d7e980da4a2ea0f1583f608a81157d2))

## [10.3.0](https://github.com/web3-storage/w3up/compare/w3up-client-v10.2.0...w3up-client-v10.3.0) (2023-11-15)


### Features

* w3up client login ([#1120](https://github.com/web3-storage/w3up/issues/1120)) ([8279bf6](https://github.com/web3-storage/w3up/commit/8279bf6371182709b46e83e5ac86d89ed1f292e8))


### Bug Fixes

* authorize renamed to login in docs ([#1125](https://github.com/web3-storage/w3up/issues/1125)) ([1c3e773](https://github.com/web3-storage/w3up/commit/1c3e773b7e2572d68a8c64bdefc08f8839f17670))

## [10.2.0](https://github.com/web3-storage/w3up/compare/w3up-client-v10.1.0...w3up-client-v10.2.0) (2023-11-14)


### Features

* account.plan.get method ([#1117](https://github.com/web3-storage/w3up/issues/1117)) ([1385a9c](https://github.com/web3-storage/w3up/commit/1385a9c4f722e678090fc4371a0c4959cef3c6cd))

## [10.1.0](https://github.com/web3-storage/w3up/compare/w3up-client-v10.0.0...w3up-client-v10.1.0) (2023-11-13)


### Features

* export Account so we can use it in w3ui ([#1116](https://github.com/web3-storage/w3up/issues/1116)) ([9c7266e](https://github.com/web3-storage/w3up/commit/9c7266ea296e567784feba62e2737d5d700bf2ac))


### Bug Fixes

* export new subscription, usage and filecoin clients ([#1111](https://github.com/web3-storage/w3up/issues/1111)) ([7fe797d](https://github.com/web3-storage/w3up/commit/7fe797d4e4920ff01e668e228cc237da9f81ed9f))

## [10.0.0](https://github.com/web3-storage/w3up/compare/w3up-client-v9.3.0...w3up-client-v10.0.0) (2023-11-09)


### ⚠ BREAKING CHANGES

* tweak readmes to get release-please to bump major version ([#1102](https://github.com/web3-storage/w3up/issues/1102))

### Features

* add `subscription/list` capability ([#1088](https://github.com/web3-storage/w3up/issues/1088)) ([471d7e5](https://github.com/web3-storage/w3up/commit/471d7e5db24e12a06c1c52ae76bf95ff9471bac8))
* expose accounts list on client instance ([#1109](https://github.com/web3-storage/w3up/issues/1109)) ([1810684](https://github.com/web3-storage/w3up/commit/1810684e1a21109a8f03685eb9a15ae5b2bc1782))
* filecoin info ([#1091](https://github.com/web3-storage/w3up/issues/1091)) ([adb2442](https://github.com/web3-storage/w3up/commit/adb24424d1faf50daf2339b77c22fdd44faa236a))
* tweak readmes to get release-please to bump major version ([#1102](https://github.com/web3-storage/w3up/issues/1102)) ([a411255](https://github.com/web3-storage/w3up/commit/a4112551f5dbac00f4b5a0da8c81ea35783f3ef9))
* **w3up-client:** export additional modules ([#1110](https://github.com/web3-storage/w3up/issues/1110)) ([5ce43bc](https://github.com/web3-storage/w3up/commit/5ce43bc309f4029232f70d827f1fcc71a13c3758))


### Bug Fixes

* README with uploadDirectory, not store ([#1106](https://github.com/web3-storage/w3up/issues/1106)) ([22773bf](https://github.com/web3-storage/w3up/commit/22773bf7e06742658d175d0959fd3f1edcd4a0bd))

## [9.3.0](https://github.com/web3-storage/w3up/compare/w3up-client-v9.2.2...w3up-client-v9.3.0) (2023-11-08)


### Features

* add usage/report capability ([#1079](https://github.com/web3-storage/w3up/issues/1079)) ([6418b4b](https://github.com/web3-storage/w3up/commit/6418b4b22329a118fb258928bd9a6a45ced5ce45))

## [9.2.2](https://github.com/web3-storage/w3up/compare/w3up-client-v9.2.1...w3up-client-v9.2.2) (2023-11-03)


### Bug Fixes

* trigger commit for release of w3up client ([#1070](https://github.com/web3-storage/w3up/issues/1070)) ([8edcbf8](https://github.com/web3-storage/w3up/commit/8edcbf827269495a112272b1e59ee6a286b5bd3b))

## [9.2.1](https://github.com/web3-storage/w3up/compare/w3up-client-v9.2.0...w3up-client-v9.2.1) (2023-10-25)


### Bug Fixes

* fix arethetypesworking errors in all packages ([#1004](https://github.com/web3-storage/w3up/issues/1004)) ([2e2936a](https://github.com/web3-storage/w3up/commit/2e2936a3831389dd13be5be5146a04e2b15553c5))

## [9.2.0](https://github.com/web3-storage/w3up/compare/w3up-client-v9.1.0...w3up-client-v9.2.0) (2023-10-20)


### Features

* add `store/get` and `upload/get` capabilities ([#942](https://github.com/web3-storage/w3up/issues/942)) ([40c79eb](https://github.com/web3-storage/w3up/commit/40c79eb8f246775b9e1828240f271fa75ef696be))

## [9.1.0](https://github.com/web3-storage/w3up/compare/w3up-client-v9.0.0...w3up-client-v9.1.0) (2023-10-19)


### Features

* add revocation to access-client and w3up-client ([#975](https://github.com/web3-storage/w3up/issues/975)) ([6c877aa](https://github.com/web3-storage/w3up/commit/6c877aac78eddb924e999dc3270cba010e48e30a))


### Bug Fixes

* update README to reflect authorize-first flow ([#961](https://github.com/web3-storage/w3up/issues/961)) ([9f59720](https://github.com/web3-storage/w3up/commit/9f59720890e38cf225794a4893b803532c916c50))

## [9.0.0](https://github.com/web3-storage/w3up/compare/w3up-client-v8.1.0...w3up-client-v9.0.0) (2023-10-18)


### ⚠ BREAKING CHANGES

* Returning the `size` means that we need to fetch the stored item beforehand, and if it does not exist throw a `StoreItemNotFound` error. This is a change from the current behaviour which returns successfully even if the item is not present in the space.

### Features

* add size to `store/remove` receipt ([#969](https://github.com/web3-storage/w3up/issues/969)) ([d2100eb](https://github.com/web3-storage/w3up/commit/d2100eb0ffa5968c326d58d583a258187f9119eb))

## [8.1.0](https://github.com/web3-storage/w3up/compare/w3up-client-v8.0.3...w3up-client-v8.1.0) (2023-10-10)


### Features

* diagrams in readme, delegated example ([#909](https://github.com/web3-storage/w3up/issues/909)) ([329354d](https://github.com/web3-storage/w3up/commit/329354d75a03c2e6281696b6b12628e0b65e27b2))
* upgrade to ucanto@9 ([#951](https://github.com/web3-storage/w3up/issues/951)) ([d72faf1](https://github.com/web3-storage/w3up/commit/d72faf1bb07dd11462ae6dff8ee0469f8ae7e9e7))


### Bug Fixes

* clarity for bring your own agent example ([#939](https://github.com/web3-storage/w3up/issues/939)) ([acaafd1](https://github.com/web3-storage/w3up/commit/acaafd160b6168d470d2cf73517b23887dee62f8))
* upgrade to latest ts ([#962](https://github.com/web3-storage/w3up/issues/962)) ([711e3f7](https://github.com/web3-storage/w3up/commit/711e3f73f6905fde0d929952fff70be845a55fa1))

## [8.0.3](https://github.com/web3-storage/w3up/compare/w3up-client-v8.0.2...w3up-client-v8.0.3) (2023-09-15)


### Bug Fixes

* add providers to space/info result type ([#911](https://github.com/web3-storage/w3up/issues/911)) ([877f1a8](https://github.com/web3-storage/w3up/commit/877f1a8cf03884dcd40f979c0974b9123be8d915))
* export missing UploadRemoveOk type ([#912](https://github.com/web3-storage/w3up/issues/912)) ([8b8353c](https://github.com/web3-storage/w3up/commit/8b8353cce7ce324bf966da75654ff8d92b3e68b0))

## [8.0.2](https://github.com/web3-storage/w3up/compare/w3up-client-v8.0.1...w3up-client-v8.0.2) (2023-09-07)


### Bug Fixes

* node version ([#907](https://github.com/web3-storage/w3up/issues/907)) ([366a940](https://github.com/web3-storage/w3up/commit/366a94049d9256e9a6b6bfcee16dcffc6a6b9c31))
* README for clarity ([#892](https://github.com/web3-storage/w3up/issues/892)) ([2e75726](https://github.com/web3-storage/w3up/commit/2e7572604664c4746303169d7173257c8a123cb3))
* types for capability specific clients ([#904](https://github.com/web3-storage/w3up/issues/904)) ([b69d4aa](https://github.com/web3-storage/w3up/commit/b69d4aa11385cd23bdcda2240f7e1ba507da44b8))

## [8.0.1](https://github.com/web3-storage/w3up/compare/w3up-client-v8.0.0...w3up-client-v8.0.1) (2023-07-21)


### Bug Fixes

* bump package number to ensure w3up-client depends on &gt;= access@15 ([#836](https://github.com/web3-storage/w3up/issues/836)) ([b095b7c](https://github.com/web3-storage/w3up/commit/b095b7cfaea30f1230b8da884fb580fdf56ec732))

## [8.0.0](https://github.com/web3-storage/w3up/compare/w3up-client-v7.0.0...w3up-client-v8.0.0) (2023-07-21)


### ⚠ BREAKING CHANGES

* stop using access.web3.storage ([#833](https://github.com/web3-storage/w3up/issues/833))

### Features

* stop using access.web3.storage ([#833](https://github.com/web3-storage/w3up/issues/833)) ([0df3f2c](https://github.com/web3-storage/w3up/commit/0df3f2c0341244b2404702e8a8878cf0f6e31bc0))

## [7.0.0](https://github.com/web3-storage/w3up/compare/w3up-client-v6.0.1...w3up-client-v7.0.0) (2023-06-08)


### ⚠ BREAKING CHANGES

* merge `@web3-storage/access-api` into `@web3-storage/upload-api` ([#790](https://github.com/web3-storage/w3up/issues/790))

### Features

* merge `@web3-storage/access-api` into `@web3-storage/upload-api` ([#790](https://github.com/web3-storage/w3up/issues/790)) ([4f6ddb6](https://github.com/web3-storage/w3up/commit/4f6ddb690c365a42a3dc4c5c6898e4999bd0f868))
* w3 aggregate protocol client and api implementation ([#787](https://github.com/web3-storage/w3up/issues/787)) ([b58069d](https://github.com/web3-storage/w3up/commit/b58069d7960efe09283f3b23fed77515b62d4639))

## [6.0.1](https://github.com/web3-storage/w3up/compare/w3up-client-v6.0.0...w3up-client-v6.0.1) (2023-05-23)


### Bug Fixes

* docs for `uploadCAR` return value ([#791](https://github.com/web3-storage/w3up/issues/791)) ([a5ceee4](https://github.com/web3-storage/w3up/commit/a5ceee4ed115bf4d784b99d814c522364fdb97e6))
* upgrade remaining ucanto deps ([#798](https://github.com/web3-storage/w3up/issues/798)) ([7211501](https://github.com/web3-storage/w3up/commit/72115010663a62140127cdeed21f2dc37f59da08))
* upgrade ucanto to 8 ([#794](https://github.com/web3-storage/w3up/issues/794)) ([00b011d](https://github.com/web3-storage/w3up/commit/00b011d87f628d4b3040398ca6cba567a69713ff))

## [6.0.0](https://github.com/web3-storage/w3up/compare/w3up-client-v5.5.1...w3up-client-v6.0.0) (2023-05-03)


### ⚠ BREAKING CHANGES

* upgrade to ucanto7.x.x ([#774](https://github.com/web3-storage/w3up/issues/774))

### Features

* upgrade to ucanto7.x.x ([#774](https://github.com/web3-storage/w3up/issues/774)) ([0cc6e66](https://github.com/web3-storage/w3up/commit/0cc6e66a80476e05c75bea94c1bee9bd12cbacf5))

## [5.5.1](https://github.com/web3-storage/w3up/compare/w3up-client-v5.5.0...w3up-client-v5.5.1) (2023-04-06)


### Bug Fixes

* add newline to space.js to test release-please 694 fix ([#696](https://github.com/web3-storage/w3up/issues/696)) ([ea18619](https://github.com/web3-storage/w3up/commit/ea186193575dc1e19d01fcecddf91c0df37376cc))

## [5.5.0](https://github.com/web3-storage/w3protocol/compare/w3up-client-v5.4.0...w3up-client-v5.5.0) (2023-03-29)


### Features

* add capabilities option type for authorize ([#687](https://github.com/web3-storage/w3protocol/issues/687)) ([bf262dd](https://github.com/web3-storage/w3protocol/commit/bf262dd4380ce2564b4d0afc6aa41b47da2fb36d))
* get `access/claim` authorization wait function working ([#666](https://github.com/web3-storage/w3protocol/issues/666)) ([83971de](https://github.com/web3-storage/w3protocol/commit/83971de683b5fccbbc7ae36b7cb34d62a9930349))


### Bug Fixes

* missing file from byo principal ([6b2384e](https://github.com/web3-storage/w3protocol/commit/6b2384e45eba08a5d7a35a052d451e1cac33ff0b))

## [5.4.0](https://github.com/web3-storage/w3protocol/compare/w3up-client-v5.3.0...w3up-client-v5.4.0) (2023-03-29)


### Features

* bring your own principal ([#672](https://github.com/web3-storage/w3protocol/issues/672)) ([4586df2](https://github.com/web3-storage/w3protocol/commit/4586df25fc8b43dab0191c77ef70620fbf276e1c))

## [5.3.0](https://github.com/web3-storage/w3protocol/compare/w3up-client-v5.2.0...w3up-client-v5.3.0) (2023-03-28)


### Features

* expose `onDirectoryEntryLink` option ([#663](https://github.com/web3-storage/w3protocol/issues/663)) ([e96c8ef](https://github.com/web3-storage/w3protocol/commit/e96c8efecc09bba5756c608a1edd4e52340cd37c))

## [5.2.0](https://github.com/web3-storage/w3protocol/compare/w3up-client-v5.1.0...w3up-client-v5.2.0) (2023-03-28)


### Features

* add w3up-client at /packages/w3up-client ([#653](https://github.com/web3-storage/w3protocol/issues/653)) ([ca921ec](https://github.com/web3-storage/w3protocol/commit/ca921ec2d6fb99d5d3db44f1d5ce77e1fe3dd7dd))


### Miscellaneous Chores

* **access-client:** release 11.0.0-rc.0 ([#573](https://github.com/web3-storage/w3protocol/issues/573)) ([be4386d](https://github.com/web3-storage/w3protocol/commit/be4386d66ceea393f289adb3c79273c250542807))

## [5.1.0](https://github.com/web3-storage/w3up-client/compare/v5.0.0...v5.1.0) (2023-03-24)


### Features

* updated README instructions for MVP ([#85](https://github.com/web3-storage/w3up-client/issues/85)) ([0d0a038](https://github.com/web3-storage/w3up-client/commit/0d0a0389f0b6b29c843d5b28c3ea2d840d38120f))

## [5.0.0](https://github.com/web3-storage/w3up-client/compare/v4.3.0...v5.0.0) (2023-03-23)


### ⚠ BREAKING CHANGES

* updated access client dep ([#89](https://github.com/web3-storage/w3up-client/issues/89))

### Features

* add HAMT sharded directories support ([#87](https://github.com/web3-storage/w3up-client/issues/87)) ([a6673e9](https://github.com/web3-storage/w3up-client/commit/a6673e98f51dc1dc93e5e40ea752a5c10e46c159))
* updated access client dep ([#89](https://github.com/web3-storage/w3up-client/issues/89)) ([35f3964](https://github.com/web3-storage/w3up-client/commit/35f39640a62eaf9a2e6a81632e32cf1851d640b4))

## [4.3.0](https://github.com/web3-storage/w3up-client/compare/v4.2.0...v4.3.0) (2023-03-21)


### Features

* add authorize to client, register no longer needs email ([c9555d9](https://github.com/web3-storage/w3up-client/commit/c9555d92edb1ded9c7db81efcdd2c83331b52106))
* expose connection id did and add email back to registerSpace ([ee1cf3a](https://github.com/web3-storage/w3up-client/commit/ee1cf3a30a79a98c21f2e897d6a26e443b41390f))
* use new claimDelegations "use case" ([1659786](https://github.com/web3-storage/w3up-client/commit/1659786fd79da6292d3605c1ca09b80d94ac83ca))


### Bug Fixes

* back to 100% test coverage ([5ae7f1e](https://github.com/web3-storage/w3up-client/commit/5ae7f1e1d19f7eb95b13ed3bc491fc99e51296d0))
* keep casting defaultProvider() ([7b8c859](https://github.com/web3-storage/w3up-client/commit/7b8c8594abd1665b0c0061ab2eef233d6a0b6cdf))
* pass registerSpace default provider inferred from connection ([224f818](https://github.com/web3-storage/w3up-client/commit/224f818f45b3fa4778a659c4f95124c92534c354))
* typos ([52c648a](https://github.com/web3-storage/w3up-client/commit/52c648a525466e1d6e0619ed4ab663164a9b6a9d))
* typos ([52c648a](https://github.com/web3-storage/w3up-client/commit/52c648a525466e1d6e0619ed4ab663164a9b6a9d))
* update package-lock ([6aa7c47](https://github.com/web3-storage/w3up-client/commit/6aa7c4785ae2bc49039c326e02d1fd042460b83d))
* use released packages to green the build ([05881fc](https://github.com/web3-storage/w3up-client/commit/05881fce652a1bc964937bec9c0cdd20aa2204b2))
* warnings about uploads being public/permanent ([187228a](https://github.com/web3-storage/w3up-client/commit/187228a828ff357f3d1083738673c6a502f2aff9))

## [4.2.0](https://github.com/web3-storage/w3up-client/compare/v4.1.0...v4.2.0) (2023-02-15)


### Features

* update to latest dependencies ([f4da59e](https://github.com/web3-storage/w3up-client/commit/f4da59ec10d8f7e96857998d34672d8848652445))

## [4.1.0](https://github.com/web3-storage/w3up-client/compare/v4.0.1...v4.1.0) (2023-01-11)


### Features

* add CAR upload method ([#72](https://github.com/web3-storage/w3up-client/issues/72)) ([8b31255](https://github.com/web3-storage/w3up-client/commit/8b31255521e6fd875fe043b9c09b347759ebf315))

## [4.0.1](https://github.com/web3-storage/w3up-client/compare/v4.0.0...v4.0.1) (2022-12-14)


### Bug Fixes

* prod access service DID ([67a5d4c](https://github.com/web3-storage/w3up-client/commit/67a5d4c77eb054f5e0075137e77daed3337f35d2))

## [4.0.0](https://github.com/web3-storage/w3up-client/compare/v3.2.0...v4.0.0) (2022-12-14)


### ⚠ BREAKING CHANGES

* The client has been re-written as a wrapper around [access-client](https://www.npmjs.com/package/@web3-storage/access) and [upload-client](https://www.npmjs.com/package/@web3-storage/upload-client) and the API has changed. 
 
Migration notes:

* `client.account()` has been removed, use `client.currentSpace()`
* `client.exportDelegation()` has been removed, use `client.createDelegation()` and then call `export()` on the returned value and encode the returned blocks as a CAR file using the [`@ipld/car`](https://www.npmjs.com/package/@ipld/car) library.
* `client.identity()` has been removed, use `client.agent()` + `client.currentSpace()` + `client.delegations()`
* `client.importDelegation()` has been removed, use `client.addProof()` (for general delegations to your agent) or `client.addSpace()` (to add a proof and _also_ add the space to your list of spaces).
* `client.insights()` has been removed - this was never working
* `client.invoke()` has been removed
* `client.list()` has been removed, use `client.capability.upload.list()`
* `client.makeDelegation()` has been renamed and signature has changed, use `client.createDelegation()`
* `client.register()` has been removed, use `client.registerSpace()`
* `client.remove()` has been removed, use `client.capability.store.remove()`
* `client.removeUpload()` has been removed, use `client.capability.upload.remove()`
* `client.stat()` has been removed, use `client.capability.store.list()`
* `client.upload()` has been removed, use `client.capability.store.add()`
* `client.uploadAdd()` has been removed, use `client.capability.upload.add()`
* `client.whoami()` has been removed, use `client.capability.space.info()`

### Features

* consume upload and access client ([#58](https://github.com/web3-storage/w3up-client/issues/58)) ([7bd91d5](https://github.com/web3-storage/w3up-client/commit/7bd91d59da2b961a4227d9c062e74169e645a0bc))


### Bug Fixes

* release please package name ([3d00586](https://github.com/web3-storage/w3up-client/commit/3d0058658d4a0e819b2da49c7cea3d084b8bba1b))
* remove pnpm reference from deploy-docs workflow ([6807f5d](https://github.com/web3-storage/w3up-client/commit/6807f5d91366e24ffe28d3177540549efbf808ca))
