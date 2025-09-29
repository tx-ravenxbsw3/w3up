# Changelog

## [20.0.0](https://github.com/tx-ravenxbsw3/w3up/compare/upload-api-v19.2.0...upload-api-v20.0.0) (2025-09-29)


### ⚠ BREAKING CHANGES

* content serve authorization ([#1590](https://github.com/tx-ravenxbsw3/w3up/issues/1590))
* `AllocationsStorage` and `BlobsStorage` methods not take `MultihashDigest` types instead of `Uint8Array`s.
* updates agent-store api to unblock integration with w3infra ([#1479](https://github.com/tx-ravenxbsw3/w3up/issues/1479))
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/tx-ravenxbsw3/w3up/issues/1444))
* add download URL method to `BlobsStorage` ([#1469](https://github.com/tx-ravenxbsw3/w3up/issues/1469))
* delegated capabilities required to use `uploadFile`, `uploadDirectory` and `uploadCAR` have changed. In order to use these methods your agent will now need to be delegated `blob/add`, `index/add`, `filecoin/offer` and `upload/add` capabilities. Note: no code changes are required.
* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344))
* add `index/add` handler ([#1421](https://github.com/tx-ravenxbsw3/w3up/issues/1421))
* restrict store API to CARs ([#1415](https://github.com/tx-ravenxbsw3/w3up/issues/1415))
* **capabilities:** `BlobMultihash` type in `@web3-storage/capabilities` renamed to `Multihash`.
* allocations storage interface now requires remove to be implemented
* release upload api with new filecoin api service for storefront ([#1347](https://github.com/tx-ravenxbsw3/w3up/issues/1347))
* return allocated bytes in `store/add` receipt ([#1213](https://github.com/tx-ravenxbsw3/w3up/issues/1213))
* add storefront filecoin api to upload api ([#1052](https://github.com/tx-ravenxbsw3/w3up/issues/1052))

### Features

* access agent proofs method would fail to return some session proofs ([#1047](https://github.com/tx-ravenxbsw3/w3up/issues/1047)) ([fd6c574](https://github.com/tx-ravenxbsw3/w3up/commit/fd6c574471e443b15ae3eba9d2c7304262ba5e49))
* add "plan/create-admin-session" capability ([#1411](https://github.com/tx-ravenxbsw3/w3up/issues/1411)) ([d9662c7](https://github.com/tx-ravenxbsw3/w3up/commit/d9662c75dd138be02213931be3c8b59f08f26ad1))
* add `index/add` handler ([#1421](https://github.com/tx-ravenxbsw3/w3up/issues/1421)) ([e2eb8a7](https://github.com/tx-ravenxbsw3/w3up/commit/e2eb8a7232116c0f4169adc1e4aaf82b60daf086))
* add `initialize` method to `PlansStorage` ([#1278](https://github.com/tx-ravenxbsw3/w3up/issues/1278)) ([4ee293a](https://github.com/tx-ravenxbsw3/w3up/commit/4ee293a5d34ce9cec2a71a71e825c8e7cd00936e))
* add `set` method to `AccountPlan` ([#1281](https://github.com/tx-ravenxbsw3/w3up/issues/1281)) ([d578c7c](https://github.com/tx-ravenxbsw3/w3up/commit/d578c7c11a1fa397b5354f31df80459fb2da63b4))
* add `subscription/list` capability ([#1088](https://github.com/tx-ravenxbsw3/w3up/issues/1088)) ([dd2c715](https://github.com/tx-ravenxbsw3/w3up/commit/dd2c715b6b3004425273d15e3a9eaa3d2f25673a))
* add blob list and remove ([#1385](https://github.com/tx-ravenxbsw3/w3up/issues/1385)) ([b4e8b40](https://github.com/tx-ravenxbsw3/w3up/commit/b4e8b401cb614e86ba636a12118c5fbf32cb5f7c))
* add blob protocol to upload-client ([#1425](https://github.com/tx-ravenxbsw3/w3up/issues/1425)) ([44bde76](https://github.com/tx-ravenxbsw3/w3up/commit/44bde7616adc94f82cfef751bcaa94cf59bf24c5))
* add blob/get ([#1484](https://github.com/tx-ravenxbsw3/w3up/issues/1484)) ([9f774cc](https://github.com/tx-ravenxbsw3/w3up/commit/9f774ccb847b0e1182b6d9a0a1ff13db03253800))
* add download URL method to `BlobsStorage` ([#1469](https://github.com/tx-ravenxbsw3/w3up/issues/1469)) ([5a15d63](https://github.com/tx-ravenxbsw3/w3up/commit/5a15d631284b5938ef5911b36e3f61bd4ba4df48))
* add storefront filecoin api to upload api ([#1052](https://github.com/tx-ravenxbsw3/w3up/issues/1052)) ([e71373f](https://github.com/tx-ravenxbsw3/w3up/commit/e71373f3536edf92d94e23eaf8d2a1bc3b95ada6))
* add usage/report capability ([#1079](https://github.com/tx-ravenxbsw3/w3up/issues/1079)) ([95db863](https://github.com/tx-ravenxbsw3/w3up/commit/95db8632ce796ff698d7b016cca6e676e846eeac))
* blob, web3.storage and ucan conclude capabilities together with api handlers  ([#1342](https://github.com/tx-ravenxbsw3/w3up/issues/1342)) ([d702ecb](https://github.com/tx-ravenxbsw3/w3up/commit/d702ecb10f87159fb50bcf0b7693ec2b3d9447d4))
* **capabilities:** add `index/add` capability ([#1410](https://github.com/tx-ravenxbsw3/w3up/issues/1410)) ([4d92f6d](https://github.com/tx-ravenxbsw3/w3up/commit/4d92f6d4209338b189e883016badef2c20784944))
* change `plan/update` to `plan/set` and use existing `PlansStorage#set` to implement an invocation handler ([#1258](https://github.com/tx-ravenxbsw3/w3up/issues/1258)) ([e2b840a](https://github.com/tx-ravenxbsw3/w3up/commit/e2b840a67092dbc1b1f1dd88808a23804086ba8c))
* content serve authorization ([#1590](https://github.com/tx-ravenxbsw3/w3up/issues/1590)) ([c752277](https://github.com/tx-ravenxbsw3/w3up/commit/c752277cc07008437fc4482ea5689a1cabc92abf))
* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344)) ([db98e3a](https://github.com/tx-ravenxbsw3/w3up/commit/db98e3ad7fd5ce589ab5f002a9e614341f9121ca))
* expose test context of upload-api ([#1069](https://github.com/tx-ravenxbsw3/w3up/issues/1069)) ([0601f41](https://github.com/tx-ravenxbsw3/w3up/commit/0601f41aa0815ecac9529c10e31cf8122906f1f8))
* external login ([#1629](https://github.com/tx-ravenxbsw3/w3up/issues/1629)) ([638c31c](https://github.com/tx-ravenxbsw3/w3up/commit/638c31c5ae06fa73264b2fa45cd223fc2f7cc704))
* filecoin info ([#1091](https://github.com/tx-ravenxbsw3/w3up/issues/1091)) ([ad4e328](https://github.com/tx-ravenxbsw3/w3up/commit/ad4e32852f9f804163ef813bae47d2d430b6cac1))
* generate sharded DAG index on client and invoke w `index/add` ([#1451](https://github.com/tx-ravenxbsw3/w3up/issues/1451)) ([a1b3ee0](https://github.com/tx-ravenxbsw3/w3up/commit/a1b3ee0f3e82a92008d0ebb4bb386a5680ca70c1))
* Generate Space proofs on the fly, on `access/claim` ([#1555](https://github.com/tx-ravenxbsw3/w3up/issues/1555)) ([45ea3e9](https://github.com/tx-ravenxbsw3/w3up/commit/45ea3e9d9ecb4285fa22fc45055c12196e1e476b))
* implement `plan/get` capability ([#1005](https://github.com/tx-ravenxbsw3/w3up/issues/1005)) ([d572f37](https://github.com/tx-ravenxbsw3/w3up/commit/d572f374c0e8a3ef1968ac14dff6632512cd2f12))
* move blob index logic from upload-api to blob-index lib ([#1434](https://github.com/tx-ravenxbsw3/w3up/issues/1434)) ([525cac8](https://github.com/tx-ravenxbsw3/w3up/commit/525cac8bdcadc3b42e313a1a4bf588a631b031cd))
* optionally require plans for provisioning ([#1087](https://github.com/tx-ravenxbsw3/w3up/issues/1087)) ([7452480](https://github.com/tx-ravenxbsw3/w3up/commit/74524801240a5b15824c22ddd3fbe17f5370f45d))
* port of https://github.com/storacha/upload-service/commit/2c12c23d13d14e9f1b79c34b8169f20975d431f7 ([#1641](https://github.com/tx-ravenxbsw3/w3up/issues/1641)) ([a7f964b](https://github.com/tx-ravenxbsw3/w3up/commit/a7f964b76442a66b9c94acd219fe3c099c999d82))
* publish index claim ([#1487](https://github.com/tx-ravenxbsw3/w3up/issues/1487)) ([6de2ba8](https://github.com/tx-ravenxbsw3/w3up/commit/6de2ba837e04f371a319be90a588b00608846b57))
* remove issuer row ([#1345](https://github.com/tx-ravenxbsw3/w3up/issues/1345)) ([dc4adce](https://github.com/tx-ravenxbsw3/w3up/commit/dc4adcebee2a515988524a25dec97d2ffc2fea98))
* restrict store API to CARs ([#1415](https://github.com/tx-ravenxbsw3/w3up/issues/1415)) ([4a8bdb6](https://github.com/tx-ravenxbsw3/w3up/commit/4a8bdb69c4c7edec121ee4b53374cc30c5ee81b3))
* return allocated bytes in `store/add` receipt ([#1213](https://github.com/tx-ravenxbsw3/w3up/issues/1213)) ([a243e22](https://github.com/tx-ravenxbsw3/w3up/commit/a243e221153a8107ad92218f545d20ab1b3bd120))
* two more interface tweaks ([#1287](https://github.com/tx-ravenxbsw3/w3up/issues/1287)) ([3abd0e2](https://github.com/tx-ravenxbsw3/w3up/commit/3abd0e23f5c48312e98338e2af6e813c0c3b1b35))
* updates agent-store api to unblock integration with w3infra ([#1479](https://github.com/tx-ravenxbsw3/w3up/issues/1479)) ([bfc8b35](https://github.com/tx-ravenxbsw3/w3up/commit/bfc8b35b4077b5a6b4433aef517e847d9191c754))
* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/tx-ravenxbsw3/w3up/issues/1312)) ([5ed0f70](https://github.com/tx-ravenxbsw3/w3up/commit/5ed0f708d74745ae86c6c69c436a7dffb9c9d7c8))
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/tx-ravenxbsw3/w3up/issues/1444)) ([bd4885b](https://github.com/tx-ravenxbsw3/w3up/commit/bd4885b3a88216cd3402749bd03fa4682e5a7495))
* usage/record capability definition ([#1562](https://github.com/tx-ravenxbsw3/w3up/issues/1562)) ([0cb6af9](https://github.com/tx-ravenxbsw3/w3up/commit/0cb6af9ac0954e3d9ee24f63ed86a5cfa1312ef0))
* use digest in `blob/accept` location commitment ([#1480](https://github.com/tx-ravenxbsw3/w3up/issues/1480)) ([b1784af](https://github.com/tx-ravenxbsw3/w3up/commit/b1784aff914d2d6be2d9b2d914b80699b9e660cc))


### Fixes

* `encodeURIComponent` on bucket origin ([#1448](https://github.com/tx-ravenxbsw3/w3up/issues/1448)) ([faf9b30](https://github.com/tx-ravenxbsw3/w3up/commit/faf9b301296940e1a2dc78734d3cf03eb4363bd3))
* add debugging for allocate receipt ([6142796](https://github.com/tx-ravenxbsw3/w3up/commit/6142796d3b60c7f27817df07f6341c9401b7f9f3))
* add errors to exports ([#1368](https://github.com/tx-ravenxbsw3/w3up/issues/1368)) ([ae1ba90](https://github.com/tx-ravenxbsw3/w3up/commit/ae1ba908d6c0710254247878094b49ee12f23e64))
* add format specifier to blob location claim URL ([#1445](https://github.com/tx-ravenxbsw3/w3up/issues/1445)) ([495f47a](https://github.com/tx-ravenxbsw3/w3up/commit/495f47a44d3111b9b668405a65bd49c85f15867c))
* add whitespace to trigger a release ([#1390](https://github.com/tx-ravenxbsw3/w3up/issues/1390)) ([3f6a185](https://github.com/tx-ravenxbsw3/w3up/commit/3f6a1854ac4bacd6040cd20d88a452bcf9dace76))
* allocation interface rename invocation to cause ([#1382](https://github.com/tx-ravenxbsw3/w3up/issues/1382)) ([e430ba9](https://github.com/tx-ravenxbsw3/w3up/commit/e430ba9954209610c774f83c5cd68ad2c44e9ca2))
* **egress/record:** rename capability ([#1572](https://github.com/tx-ravenxbsw3/w3up/issues/1572)) ([9cb5261](https://github.com/tx-ravenxbsw3/w3up/commit/9cb5261de19cb22109f03e9695adbf08b651cd63))
* **egressRecord:** Remove unnecessary multiplication for ts conversion ([#1588](https://github.com/tx-ravenxbsw3/w3up/issues/1588)) ([5609fa9](https://github.com/tx-ravenxbsw3/w3up/commit/5609fa905513806de38b9cc9db4cfce789de2070))
* enable storefront signer to be different from main service signer ([#1072](https://github.com/tx-ravenxbsw3/w3up/issues/1072)) ([aaf9daf](https://github.com/tx-ravenxbsw3/w3up/commit/aaf9daf4d13b552a2f1e70b762483e7b52c8c389))
* ensure idempotent ([b979f53](https://github.com/tx-ravenxbsw3/w3up/commit/b979f531361789396f681cebf6e6ebf662d6463b))
* Error should refer to Resource, not Issuer ([#1558](https://github.com/tx-ravenxbsw3/w3up/issues/1558)) ([47e7d10](https://github.com/tx-ravenxbsw3/w3up/commit/47e7d101ca98b89dac9e99b7ad896f3e6bd321f4))
* export ShardedDAGIndex type ([f2ee33a](https://github.com/tx-ravenxbsw3/w3up/commit/f2ee33a1bf6edc2245dceb4edcdf0df46e29d57d))
* export test handlers and storages ([#1370](https://github.com/tx-ravenxbsw3/w3up/issues/1370)) ([928badf](https://github.com/tx-ravenxbsw3/w3up/commit/928badf8350728e0db7321f62ebab6816829552d))
* export UsageStorage ([#1334](https://github.com/tx-ravenxbsw3/w3up/issues/1334)) ([e3c304c](https://github.com/tx-ravenxbsw3/w3up/commit/e3c304c3feeeabc23e9d104f3230e49891a6e545))
* floating promises and add no-floating-promises to eslint-config-w3up ([#1198](https://github.com/tx-ravenxbsw3/w3up/issues/1198)) ([3ad073f](https://github.com/tx-ravenxbsw3/w3up/commit/3ad073f1617fb929409ce44b012eb629378ae10b))
* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/tx-ravenxbsw3/w3up/issues/1141)) ([93980ef](https://github.com/tx-ravenxbsw3/w3up/commit/93980ef8759b01b689a017aa7ae5a06d83284948))
* lint ([#1095](https://github.com/tx-ravenxbsw3/w3up/issues/1095)) ([6b37256](https://github.com/tx-ravenxbsw3/w3up/commit/6b37256cbaac1246812e6200b7a23cd7dd61165d))
* migrate repo ([#1388](https://github.com/tx-ravenxbsw3/w3up/issues/1388)) ([5cdd6eb](https://github.com/tx-ravenxbsw3/w3up/commit/5cdd6eb504db7b6c61985ecadc005581f3a2412a))
* migrate repo ([#1389](https://github.com/tx-ravenxbsw3/w3up/issues/1389)) ([9e18c76](https://github.com/tx-ravenxbsw3/w3up/commit/9e18c761e63c88e395b66b4f7cbadc79fc837dec))
* missing exports ([35f072f](https://github.com/tx-ravenxbsw3/w3up/commit/35f072fa29830513483a2f53bb6d08aeff35bbdf))
* missing exports ([#1335](https://github.com/tx-ravenxbsw3/w3up/issues/1335)) ([5348856](https://github.com/tx-ravenxbsw3/w3up/commit/53488564650132743cbf369b5227bfa89df742e7))
* missing test export ([87f680c](https://github.com/tx-ravenxbsw3/w3up/commit/87f680cc2d8e1c681d31829a3570c19c0282d82b))
* one more tweak to the `PlanStorage` interface ([#1280](https://github.com/tx-ravenxbsw3/w3up/issues/1280)) ([9dabd5b](https://github.com/tx-ravenxbsw3/w3up/commit/9dabd5b4118cb58ffe9897630ab9251ac9dc21d2))
* package metadata ([#1161](https://github.com/tx-ravenxbsw3/w3up/issues/1161)) ([68b41e4](https://github.com/tx-ravenxbsw3/w3up/commit/68b41e49f4e77aabe07594b22691b2febdb3ea91))
* publish location claim to content claims service ([#1571](https://github.com/tx-ravenxbsw3/w3up/issues/1571)) ([d1b0824](https://github.com/tx-ravenxbsw3/w3up/commit/d1b0824bc5a033982925a7896791c405e333c3d8))
* release upload api with new filecoin api service for storefront ([#1347](https://github.com/tx-ravenxbsw3/w3up/issues/1347)) ([dd659b9](https://github.com/tx-ravenxbsw3/w3up/commit/dd659b9b8db49b9d9ee1c554b5df83df89e00236))
* rename blob and index client capabilities ([#1478](https://github.com/tx-ravenxbsw3/w3up/issues/1478)) ([ee5a89c](https://github.com/tx-ravenxbsw3/w3up/commit/ee5a89cac2248e634bd4e835270d052cdbb31aef))
* repo URLs ([#1550](https://github.com/tx-ravenxbsw3/w3up/issues/1550)) ([6fd5aa3](https://github.com/tx-ravenxbsw3/w3up/commit/6fd5aa32e9cfb5633ec662363e6a48493b1f8cf0))
* return correct response for index extract error ([6cdab0c](https://github.com/tx-ravenxbsw3/w3up/commit/6cdab0cd057aba2fde5fd4239ade96a08e006423))
* revert enable storefront signer to be different from main service signer ([#1075](https://github.com/tx-ravenxbsw3/w3up/issues/1075)) ([ccf78a1](https://github.com/tx-ravenxbsw3/w3up/commit/ccf78a1192020c5189d76a41bfa642ccb12083af))
* stop writing to DUDEWHERE ([#1500](https://github.com/tx-ravenxbsw3/w3up/issues/1500)) ([f748f87](https://github.com/tx-ravenxbsw3/w3up/commit/f748f8799daf5414023dd6a2e5c6a1bc5943724e))
* storage operation failed type name instead of store ([#1374](https://github.com/tx-ravenxbsw3/w3up/issues/1374)) ([bf8172c](https://github.com/tx-ravenxbsw3/w3up/commit/bf8172cb2eb6eaab0fbc4f22f88940989e221768))
* test against actual api ([#1438](https://github.com/tx-ravenxbsw3/w3up/issues/1438)) ([851d5be](https://github.com/tx-ravenxbsw3/w3up/commit/851d5beb7fc2ed9d434d6a6105b262a9047023ff))
* **test:** await promise and check error ([#1563](https://github.com/tx-ravenxbsw3/w3up/issues/1563)) ([d9b34d1](https://github.com/tx-ravenxbsw3/w3up/commit/d9b34d10ff9ba73b290160236b566b8d2bb93ebf))
* trigger release for upload api ([#1107](https://github.com/tx-ravenxbsw3/w3up/issues/1107)) ([82d8112](https://github.com/tx-ravenxbsw3/w3up/commit/82d8112db095ed73558baf4185c368bcc7d55115))
* ucan conclude scheduler invocation type and improve test ([#1379](https://github.com/tx-ravenxbsw3/w3up/issues/1379)) ([a5d76e6](https://github.com/tx-ravenxbsw3/w3up/commit/a5d76e6bf74d834f5a1e735bd7e33ec2a390804d))
* upgrade @ucanto/validator with bugfix ([#1151](https://github.com/tx-ravenxbsw3/w3up/issues/1151)) ([34e6f87](https://github.com/tx-ravenxbsw3/w3up/commit/34e6f87747809083388354926c606d8fbbd3db95))
* upgrade ucanto core ([#1127](https://github.com/tx-ravenxbsw3/w3up/issues/1127)) ([40b3257](https://github.com/tx-ravenxbsw3/w3up/commit/40b32571b42ff63f37d5020299ebb013e1886286))
* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/tx-ravenxbsw3/w3up/issues/1359)) ([6ca062f](https://github.com/tx-ravenxbsw3/w3up/commit/6ca062fad73a442b81553fc79fd75923ff9e1bcf))
* use MultihashDigest type in stores ([#1474](https://github.com/tx-ravenxbsw3/w3up/issues/1474)) ([a364a17](https://github.com/tx-ravenxbsw3/w3up/commit/a364a1766d05ac9f69bc22bac6e9c946fd799c7e))
* use one-webcrypto from npm ([#1525](https://github.com/tx-ravenxbsw3/w3up/issues/1525)) ([f72908a](https://github.com/tx-ravenxbsw3/w3up/commit/f72908a60b758c78f5b9d33ba790d3c4ff8c566f))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/tx-ravenxbsw3/w3up/issues/1533)) ([47cc600](https://github.com/tx-ravenxbsw3/w3up/commit/47cc6006b1b7316c6815dfdca0a55122f632fec3))
* appease linter ([0f49e0c](https://github.com/tx-ravenxbsw3/w3up/commit/0f49e0ce451946d909be4a788e934a126fec5812))
* **main:** release upload-api 10.0.0 ([#1387](https://github.com/tx-ravenxbsw3/w3up/issues/1387)) ([cd675a9](https://github.com/tx-ravenxbsw3/w3up/commit/cd675a9f11ee838b57b554e1bb5fb7dc4bb5a85c))
* **main:** release upload-api 10.0.1 ([#1393](https://github.com/tx-ravenxbsw3/w3up/issues/1393)) ([1cdc289](https://github.com/tx-ravenxbsw3/w3up/commit/1cdc2895fb96bc8020c1191b0ee3d603f244acd2))
* **main:** release upload-api 11.0.0 ([#1413](https://github.com/tx-ravenxbsw3/w3up/issues/1413)) ([c9496d4](https://github.com/tx-ravenxbsw3/w3up/commit/c9496d4961a2759a260d184f517b901a174f161d))
* **main:** release upload-api 12.0.0 ([#1417](https://github.com/tx-ravenxbsw3/w3up/issues/1417)) ([d20917b](https://github.com/tx-ravenxbsw3/w3up/commit/d20917b13be36458255d149ea94ddfaa942c28b4))
* **main:** release upload-api 13.0.0 ([#1427](https://github.com/tx-ravenxbsw3/w3up/issues/1427)) ([5edc101](https://github.com/tx-ravenxbsw3/w3up/commit/5edc101dd0c3e56e3ca0ac871f847d5a059869ad))
* **main:** release upload-api 13.0.1 ([#1432](https://github.com/tx-ravenxbsw3/w3up/issues/1432)) ([8db97bf](https://github.com/tx-ravenxbsw3/w3up/commit/8db97bf77857fd4e85b874cb990120f4e55a127e))
* **main:** release upload-api 13.0.2 ([#1433](https://github.com/tx-ravenxbsw3/w3up/issues/1433)) ([1a56edc](https://github.com/tx-ravenxbsw3/w3up/commit/1a56edc9cd916727240de0a9702c41cec066a6b7))
* **main:** release upload-api 14.0.0 ([#1441](https://github.com/tx-ravenxbsw3/w3up/issues/1441)) ([0e4f1b5](https://github.com/tx-ravenxbsw3/w3up/commit/0e4f1b5cf964a9a66889edfa05f6d057299fc86c))
* **main:** release upload-api 15.0.0 ([#1463](https://github.com/tx-ravenxbsw3/w3up/issues/1463)) ([b22bfe5](https://github.com/tx-ravenxbsw3/w3up/commit/b22bfe55ebf49e71b7b5762355dca3eaa4cf217b))
* **main:** release upload-api 15.0.1 ([#1466](https://github.com/tx-ravenxbsw3/w3up/issues/1466)) ([c8bb8c6](https://github.com/tx-ravenxbsw3/w3up/commit/c8bb8c6d1b521e20513ce4b9ea5ad2e59c0f9bc5))
* **main:** release upload-api 16.0.0 ([#1470](https://github.com/tx-ravenxbsw3/w3up/issues/1470)) ([041fe4a](https://github.com/tx-ravenxbsw3/w3up/commit/041fe4af5418aa6269fe178d47278bccf95e8bbf))
* **main:** release upload-api 17.0.0 ([#1471](https://github.com/tx-ravenxbsw3/w3up/issues/1471)) ([8996494](https://github.com/tx-ravenxbsw3/w3up/commit/8996494e2bc4b4da4ff163896195375bc74e21b6))
* **main:** release upload-api 17.1.0 ([#1491](https://github.com/tx-ravenxbsw3/w3up/issues/1491)) ([3aa28d0](https://github.com/tx-ravenxbsw3/w3up/commit/3aa28d0ac82305eea6371a2f4c596cec776b28e6))
* **main:** release upload-api 18.0.0 ([#1501](https://github.com/tx-ravenxbsw3/w3up/issues/1501)) ([3f10a09](https://github.com/tx-ravenxbsw3/w3up/commit/3f10a0929fed3ac59fc019602ee623a3b74983ea))
* **main:** release upload-api 18.0.1 ([#1511](https://github.com/tx-ravenxbsw3/w3up/issues/1511)) ([15d9bbb](https://github.com/tx-ravenxbsw3/w3up/commit/15d9bbbe828dd375deacb96979e3a1af6ff0ad04))
* **main:** release upload-api 18.0.2 ([#1519](https://github.com/tx-ravenxbsw3/w3up/issues/1519)) ([5a806d1](https://github.com/tx-ravenxbsw3/w3up/commit/5a806d1d65b0aa10138a12187c423401247cf9fc))
* **main:** release upload-api 18.0.3 ([#1527](https://github.com/tx-ravenxbsw3/w3up/issues/1527)) ([8585433](https://github.com/tx-ravenxbsw3/w3up/commit/858543310801d5a97c5bec13cba8889990926d78))
* **main:** release upload-api 18.1.0 ([#1543](https://github.com/tx-ravenxbsw3/w3up/issues/1543)) ([e134494](https://github.com/tx-ravenxbsw3/w3up/commit/e1344940a9aa010e13c84b78d2276728d65cbe51))
* **main:** release upload-api 18.1.1 ([#1576](https://github.com/tx-ravenxbsw3/w3up/issues/1576)) ([b8fba42](https://github.com/tx-ravenxbsw3/w3up/commit/b8fba424abdd09709af385efd7d56d8a10c2a233))
* **main:** release upload-api 18.1.2 ([#1584](https://github.com/tx-ravenxbsw3/w3up/issues/1584)) ([51f6b72](https://github.com/tx-ravenxbsw3/w3up/commit/51f6b7219fca066bdd69d47c6eea4e9591bfedd8))
* **main:** release upload-api 18.1.3 ([#1589](https://github.com/tx-ravenxbsw3/w3up/issues/1589)) ([65e32e2](https://github.com/tx-ravenxbsw3/w3up/commit/65e32e2bdc76773e25ac646e2bc53164420299f7))
* **main:** release upload-api 18.1.4 ([#1593](https://github.com/tx-ravenxbsw3/w3up/issues/1593)) ([49e8880](https://github.com/tx-ravenxbsw3/w3up/commit/49e8880ad0f92a6e5a220191f9579e69e24ec58c))
* **main:** release upload-api 19.0.0 ([#1599](https://github.com/tx-ravenxbsw3/w3up/issues/1599)) ([7dbd83c](https://github.com/tx-ravenxbsw3/w3up/commit/7dbd83c171dc03b664e223045bc31cc4c3077156))
* **main:** release upload-api 19.1.0 ([#1625](https://github.com/tx-ravenxbsw3/w3up/issues/1625)) ([c09bfc1](https://github.com/tx-ravenxbsw3/w3up/commit/c09bfc1d08266fe4e209ab639eb596643b82825d))
* **main:** release upload-api 19.2.0 ([#1642](https://github.com/tx-ravenxbsw3/w3up/issues/1642)) ([9b7f735](https://github.com/tx-ravenxbsw3/w3up/commit/9b7f7354ec6ac3432482458a42da9772432f28c5))
* **main:** release upload-api 6.3.0 ([#1003](https://github.com/tx-ravenxbsw3/w3up/issues/1003)) ([ffb915c](https://github.com/tx-ravenxbsw3/w3up/commit/ffb915c3ca3b828d1e9f9032cdc8fe68863d7543))
* **main:** release upload-api 7.0.0 ([#1027](https://github.com/tx-ravenxbsw3/w3up/issues/1027)) ([ce96414](https://github.com/tx-ravenxbsw3/w3up/commit/ce9641496db387e90f337bd2b8392bf5f8288eca))
* **main:** release upload-api 7.1.0 ([#1057](https://github.com/tx-ravenxbsw3/w3up/issues/1057)) ([9471d16](https://github.com/tx-ravenxbsw3/w3up/commit/9471d164324317b7e4c9fc8122c4d8216ddf6582))
* **main:** release upload-api 7.1.1 ([#1074](https://github.com/tx-ravenxbsw3/w3up/issues/1074)) ([14d0817](https://github.com/tx-ravenxbsw3/w3up/commit/14d08175ceb5b5640973aa0bc827dbe009b0d096))
* **main:** release upload-api 7.1.2 ([#1076](https://github.com/tx-ravenxbsw3/w3up/issues/1076)) ([51921ff](https://github.com/tx-ravenxbsw3/w3up/commit/51921ff8e5f9e156dd9b406970eefac4fda91cea))
* **main:** release upload-api 7.2.0 ([#1082](https://github.com/tx-ravenxbsw3/w3up/issues/1082)) ([76aa419](https://github.com/tx-ravenxbsw3/w3up/commit/76aa419e6b8e703dd7e418fe5c69e8fb400e1d28))
* **main:** release upload-api 7.3.0 ([#1096](https://github.com/tx-ravenxbsw3/w3up/issues/1096)) ([338f2bd](https://github.com/tx-ravenxbsw3/w3up/commit/338f2bdf3a6d05ea014d29d286426846f038953e))
* **main:** release upload-api 7.3.1 ([#1108](https://github.com/tx-ravenxbsw3/w3up/issues/1108)) ([a20e7c5](https://github.com/tx-ravenxbsw3/w3up/commit/a20e7c51e7ad30bb0bae40a536637b36720e85ca))
* **main:** release upload-api 7.3.2 ([#1128](https://github.com/tx-ravenxbsw3/w3up/issues/1128)) ([1194592](https://github.com/tx-ravenxbsw3/w3up/commit/1194592728f129dc345491371ed58cda2839c2eb))
* **main:** release upload-api 7.3.3 ([#1143](https://github.com/tx-ravenxbsw3/w3up/issues/1143)) ([d7a891c](https://github.com/tx-ravenxbsw3/w3up/commit/d7a891c9d5103cd5eaef9b67d1f3c1bdd679f52c))
* **main:** release upload-api 7.3.4 ([#1165](https://github.com/tx-ravenxbsw3/w3up/issues/1165)) ([8a434db](https://github.com/tx-ravenxbsw3/w3up/commit/8a434db64405dfafc8226fb51f198dff77c219de))
* **main:** release upload-api 7.3.5 ([#1201](https://github.com/tx-ravenxbsw3/w3up/issues/1201)) ([b9df421](https://github.com/tx-ravenxbsw3/w3up/commit/b9df4218f3e423663fd7a47f994d6f59ebc35406))
* **main:** release upload-api 8.0.0 ([#1232](https://github.com/tx-ravenxbsw3/w3up/issues/1232)) ([5f8de32](https://github.com/tx-ravenxbsw3/w3up/commit/5f8de32692ec4e6bb9d849e6b63723c6ffe9d619))
* **main:** release upload-api 8.1.0 ([#1262](https://github.com/tx-ravenxbsw3/w3up/issues/1262)) ([a9b4a57](https://github.com/tx-ravenxbsw3/w3up/commit/a9b4a572c6e7b074181e1ed5b37e875138257f64))
* **main:** release upload-api 8.2.0 ([#1282](https://github.com/tx-ravenxbsw3/w3up/issues/1282)) ([a832ea1](https://github.com/tx-ravenxbsw3/w3up/commit/a832ea1ba5d6e18ea25ced0e0c75ae591b3f306f))
* **main:** release upload-api 8.3.0 ([#1289](https://github.com/tx-ravenxbsw3/w3up/issues/1289)) ([be92fbc](https://github.com/tx-ravenxbsw3/w3up/commit/be92fbc330add2b7a59d06d266f3a54d292f85bf))
* **main:** release upload-api 8.4.0 ([#1316](https://github.com/tx-ravenxbsw3/w3up/issues/1316)) ([51b8e75](https://github.com/tx-ravenxbsw3/w3up/commit/51b8e7506410891f8354506abc050388067208d4))
* **main:** release upload-api 8.4.1 ([#1336](https://github.com/tx-ravenxbsw3/w3up/issues/1336)) ([70df101](https://github.com/tx-ravenxbsw3/w3up/commit/70df101e24e92785af9683ed08972a2980d310e2))
* **main:** release upload-api 9.0.0 ([#1348](https://github.com/tx-ravenxbsw3/w3up/issues/1348)) ([a184f61](https://github.com/tx-ravenxbsw3/w3up/commit/a184f610bd9ac1000cecc34e3819b26d3f1f2ca7))
* **main:** release upload-api 9.0.1 ([#1360](https://github.com/tx-ravenxbsw3/w3up/issues/1360)) ([326f60a](https://github.com/tx-ravenxbsw3/w3up/commit/326f60a424f8e0d06eb6522f12975f63cefeaf41))
* **main:** release upload-api 9.1.0 ([#1367](https://github.com/tx-ravenxbsw3/w3up/issues/1367)) ([ee6b639](https://github.com/tx-ravenxbsw3/w3up/commit/ee6b6395fbf744f8fa195f5978a9283eca4fd664))
* **main:** release upload-api 9.1.1 ([#1369](https://github.com/tx-ravenxbsw3/w3up/issues/1369)) ([f49369a](https://github.com/tx-ravenxbsw3/w3up/commit/f49369a9c0bf675e58d2ca651e048f7602428dd9))
* **main:** release upload-api 9.1.2 ([#1372](https://github.com/tx-ravenxbsw3/w3up/issues/1372)) ([8a2dc99](https://github.com/tx-ravenxbsw3/w3up/commit/8a2dc998edb1ab4faad2f32e4c8fceb9d3b998b0))
* **main:** release upload-api 9.1.3 ([#1375](https://github.com/tx-ravenxbsw3/w3up/issues/1375)) ([dbec402](https://github.com/tx-ravenxbsw3/w3up/commit/dbec402a62dd1e247375dc3ed6fc278887e1d0d0))
* **main:** release upload-api 9.1.4 ([#1380](https://github.com/tx-ravenxbsw3/w3up/issues/1380)) ([e3dd863](https://github.com/tx-ravenxbsw3/w3up/commit/e3dd86397e46f4557a006df2bf3884cabc680933))
* **main:** release upload-api 9.1.5 ([#1383](https://github.com/tx-ravenxbsw3/w3up/issues/1383)) ([2727d98](https://github.com/tx-ravenxbsw3/w3up/commit/2727d98cecd1eb1bbc9140c644bc6503818ca89d))
* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/tx-ravenxbsw3/w3up/issues/1577)) ([bdaa5e2](https://github.com/tx-ravenxbsw3/w3up/commit/bdaa5e297fef7e7ddca6a63c12ab071000cc7d2b))
* no longer depends on hd-scripts, packages use/configure eslint directly, fixes warnings from npm lint script ([#1058](https://github.com/tx-ravenxbsw3/w3up/issues/1058)) ([3a99cc0](https://github.com/tx-ravenxbsw3/w3up/commit/3a99cc02941f9d563cac1838e1e67a3faa42c3de))
* upgrade dependencies for better de-duplication ([#1620](https://github.com/tx-ravenxbsw3/w3up/issues/1620)) ([081120e](https://github.com/tx-ravenxbsw3/w3up/commit/081120e5ad823be84922ad863acf5e48618cb69b))

## [19.2.0](https://github.com/storacha/w3up/compare/upload-api-v19.1.0...upload-api-v19.2.0) (2025-05-21)


### Features

* port of https://github.com/storacha/upload-service/commit/2c12c23d13d14e9f1b79c34b8169f20975d431f7 ([#1641](https://github.com/storacha/w3up/issues/1641)) ([8eb4306](https://github.com/storacha/w3up/commit/8eb43061b184e222f6aaf10d69a0129225858a6f))

## [19.1.0](https://github.com/storacha/w3up/compare/upload-api-v19.0.0...upload-api-v19.1.0) (2025-02-25)


### Features

* external login ([#1629](https://github.com/storacha/w3up/issues/1629)) ([150b5d7](https://github.com/storacha/w3up/commit/150b5d7c55ca92becbabab969285497fbba86268))


### Other Changes

* upgrade dependencies for better de-duplication ([#1620](https://github.com/storacha/w3up/issues/1620)) ([fa90a01](https://github.com/storacha/w3up/commit/fa90a01ceb0877cfe606d6a5a86b7a11f6b0a018))

## [19.0.0](https://github.com/storacha/w3up/compare/upload-api-v18.1.4...upload-api-v19.0.0) (2024-12-09)


### ⚠ BREAKING CHANGES

* content serve authorization ([#1590](https://github.com/storacha/w3up/issues/1590))

### Features

* content serve authorization ([#1590](https://github.com/storacha/w3up/issues/1590)) ([8b553a5](https://github.com/storacha/w3up/commit/8b553a53253f55a3f0a2980557fa5c3b92427f3f))

## [18.1.4](https://github.com/storacha/w3up/compare/upload-api-v18.1.3...upload-api-v18.1.4) (2024-11-28)


### Fixes

* publish location claim to content claims service ([#1571](https://github.com/storacha/w3up/issues/1571)) ([fb08e0e](https://github.com/storacha/w3up/commit/fb08e0e11ed482fe8996d4dc7535c45fbcc373b7))

## [18.1.3](https://github.com/storacha/w3up/compare/upload-api-v18.1.2...upload-api-v18.1.3) (2024-11-22)


### Fixes

* **egressRecord:** Remove unnecessary multiplication for ts conversion ([#1588](https://github.com/storacha/w3up/issues/1588)) ([b7bc90e](https://github.com/storacha/w3up/commit/b7bc90e6a33b8f33dd7356794c55a77b364799ee))

## [18.1.2](https://github.com/storacha/w3up/compare/upload-api-v18.1.1...upload-api-v18.1.2) (2024-11-20)


### Fixes

* ensure idempotent ([8b0584d](https://github.com/storacha/w3up/commit/8b0584dd0bea5b6cfe8ccafae8d19e708864e5d1))


### Other Changes

* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/storacha/w3up/issues/1577)) ([1482d69](https://github.com/storacha/w3up/commit/1482d69c28baff1c27b1baf5f3e5c76f844e5576))

## [18.1.1](https://github.com/storacha/w3up/compare/upload-api-v18.1.0...upload-api-v18.1.1) (2024-11-05)


### Fixes

* **egress/record:** rename capability ([#1572](https://github.com/storacha/w3up/issues/1572)) ([d28691c](https://github.com/storacha/w3up/commit/d28691c4709f4e7c5ba81e042cac9e961c273bc9))

## [18.1.0](https://github.com/storacha/w3up/compare/upload-api-v18.0.3...upload-api-v18.1.0) (2024-10-24)


### Features

* Generate Space proofs on the fly, on `access/claim` ([#1555](https://github.com/storacha/w3up/issues/1555)) ([9e2b1d4](https://github.com/storacha/w3up/commit/9e2b1d4dc721d3e61cea008719d172909c984344))
* usage/record capability definition ([#1562](https://github.com/storacha/w3up/issues/1562)) ([98c8a87](https://github.com/storacha/w3up/commit/98c8a87c52ef88da728225259e77f65733d2d7e6))


### Fixes

* Error should refer to Resource, not Issuer ([#1558](https://github.com/storacha/w3up/issues/1558)) ([25e35e3](https://github.com/storacha/w3up/commit/25e35e3c3ae86be549f11861f10894c86c46cbdd))
* repo URLs ([#1550](https://github.com/storacha/w3up/issues/1550)) ([e02ddf3](https://github.com/storacha/w3up/commit/e02ddf3696553b03f8d2f7316de0a99a9303a60f))
* **test:** await promise and check error ([#1563](https://github.com/storacha/w3up/issues/1563)) ([86e7a46](https://github.com/storacha/w3up/commit/86e7a46e289ee176fcfa6827827302510434ffb5))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/storacha/w3up/issues/1533)) ([07970ef](https://github.com/storacha/w3up/commit/07970efd443149158ebbfb2c4e745b5007eb9407))

## [18.0.3](https://github.com/storacha-network/w3up/compare/upload-api-v18.0.2...upload-api-v18.0.3) (2024-07-29)


### Fixes

* use one-webcrypto from npm ([#1525](https://github.com/storacha-network/w3up/issues/1525)) ([9345c54](https://github.com/storacha-network/w3up/commit/9345c5415bc0b0d6ce8ccdbe92eb155b11835fd8))

## [18.0.2](https://github.com/storacha-network/w3up/compare/upload-api-v18.0.1...upload-api-v18.0.2) (2024-07-16)


### Fixes

* add debugging for allocate receipt ([315f761](https://github.com/storacha-network/w3up/commit/315f76194d029fd72b1f5776a0194494af82b2e4))

## [18.0.1](https://github.com/storacha-network/w3up/compare/upload-api-v18.0.0...upload-api-v18.0.1) (2024-06-20)


### Fixes

* return correct response for index extract error ([67ef2b0](https://github.com/storacha-network/w3up/commit/67ef2b02ab2d745e4a2f023cf03f58c2a6ee1e2f))

## [18.0.0](https://github.com/w3s-project/w3up/compare/upload-api-v17.1.0...upload-api-v18.0.0) (2024-06-07)


### ⚠ BREAKING CHANGES

* `AllocationsStorage` and `BlobsStorage` methods not take `MultihashDigest` types instead of `Uint8Array`s.

### Features

* publish index claim ([#1487](https://github.com/w3s-project/w3up/issues/1487)) ([237b0c6](https://github.com/w3s-project/w3up/commit/237b0c6cda70ae3e156bac8a011a2739b346ae4b))


### Fixes

* stop writing to DUDEWHERE ([#1500](https://github.com/w3s-project/w3up/issues/1500)) ([cf0a1d6](https://github.com/w3s-project/w3up/commit/cf0a1d6e08d515854080899e57d16dca420f81e6))
* use MultihashDigest type in stores ([#1474](https://github.com/w3s-project/w3up/issues/1474)) ([6c6a3bd](https://github.com/w3s-project/w3up/commit/6c6a3bdcb924cf6f9a4723f710a27f1ae34ca560))

## [17.1.0](https://github.com/w3s-project/w3up/compare/upload-api-v17.0.0...upload-api-v17.1.0) (2024-06-04)


### Features

* add blob/get ([#1484](https://github.com/w3s-project/w3up/issues/1484)) ([328039d](https://github.com/w3s-project/w3up/commit/328039d8a29fec3c1bbab28d1bb9de1643f54f71))

## [17.0.0](https://github.com/w3s-project/w3up/compare/upload-api-v16.0.0...upload-api-v17.0.0) (2024-05-30)


### ⚠ BREAKING CHANGES

* updates agent-store api to unblock integration with w3infra ([#1479](https://github.com/w3s-project/w3up/issues/1479))
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/w3s-project/w3up/issues/1444))

### Features

* updates agent-store api to unblock integration with w3infra ([#1479](https://github.com/w3s-project/w3up/issues/1479)) ([2998a93](https://github.com/w3s-project/w3up/commit/2998a938628a924361450d24c5fc7be572acef3e))
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/w3s-project/w3up/issues/1444)) ([c9bf33e](https://github.com/w3s-project/w3up/commit/c9bf33e5512397a654db933a5e6b5db0c7c22da5))
* use digest in `blob/accept` location commitment ([#1480](https://github.com/w3s-project/w3up/issues/1480)) ([ade45eb](https://github.com/w3s-project/w3up/commit/ade45eb6f9b71f4bb4fcc771345ad21e966db730))


### Fixes

* rename blob and index client capabilities ([#1478](https://github.com/w3s-project/w3up/issues/1478)) ([17e3a31](https://github.com/w3s-project/w3up/commit/17e3a3161c6585b1844abcf7ed27252fa8580870))

## [16.0.0](https://github.com/w3s-project/w3up/compare/upload-api-v15.0.1...upload-api-v16.0.0) (2024-05-16)


### ⚠ BREAKING CHANGES

* add download URL method to `BlobsStorage` ([#1469](https://github.com/w3s-project/w3up/issues/1469))

### Features

* add download URL method to `BlobsStorage` ([#1469](https://github.com/w3s-project/w3up/issues/1469)) ([4a2c994](https://github.com/w3s-project/w3up/commit/4a2c99478fdcb129da260c1fc14da0ba1842e5ff))

## [15.0.1](https://github.com/w3s-project/w3up/compare/upload-api-v15.0.0...upload-api-v15.0.1) (2024-05-15)


### Fixes

* export ShardedDAGIndex type ([979e2c3](https://github.com/w3s-project/w3up/commit/979e2c3b070025e952e7bb490701aabb5e660e39))

## [15.0.0](https://github.com/w3s-project/w3up/compare/upload-api-v14.0.0...upload-api-v15.0.0) (2024-05-15)


### ⚠ BREAKING CHANGES

* delegated capabilities required to use `uploadFile`, `uploadDirectory` and `uploadCAR` have changed. In order to use these methods your agent will now need to be delegated `blob/add`, `index/add`, `filecoin/offer` and `upload/add` capabilities. Note: no code changes are required.

### Features

* generate sharded DAG index on client and invoke w `index/add` ([#1451](https://github.com/w3s-project/w3up/issues/1451)) ([a6d9026](https://github.com/w3s-project/w3up/commit/a6d9026536e60c0ce93b613acc6e337f2a21aeb2))

## [14.0.0](https://github.com/w3s-project/w3up/compare/upload-api-v13.0.2...upload-api-v14.0.0) (2024-05-14)


### ⚠ BREAKING CHANGES

* deprecate issuer ([#1344](https://github.com/w3s-project/w3up/issues/1344))

### Features

* add "plan/create-admin-session" capability ([#1411](https://github.com/w3s-project/w3up/issues/1411)) ([50eeeb5](https://github.com/w3s-project/w3up/commit/50eeeb502335ba0413318b5047869a275901824b))
* add blob protocol to upload-client ([#1425](https://github.com/w3s-project/w3up/issues/1425)) ([49aef56](https://github.com/w3s-project/w3up/commit/49aef564a726d34dbbedbd83f5366d9320180f99))
* deprecate issuer ([#1344](https://github.com/w3s-project/w3up/issues/1344)) ([afbbde3](https://github.com/w3s-project/w3up/commit/afbbde340d974792699dc56946cc1c72f74c09e3))
* move blob index logic from upload-api to blob-index lib ([#1434](https://github.com/w3s-project/w3up/issues/1434)) ([797f628](https://github.com/w3s-project/w3up/commit/797f6285c1b000af9eaf0240f85deca6a0b83e06))
* remove issuer row ([#1345](https://github.com/w3s-project/w3up/issues/1345)) ([cf5b0db](https://github.com/w3s-project/w3up/commit/cf5b0db276ffe3b9926dbf1d8e2cd04ef7b607c9))


### Fixes

* `encodeURIComponent` on bucket origin ([#1448](https://github.com/w3s-project/w3up/issues/1448)) ([5618644](https://github.com/w3s-project/w3up/commit/561864422db2ec3eaddc2d790cc4ea0406eebf32))
* add format specifier to blob location claim URL ([#1445](https://github.com/w3s-project/w3up/issues/1445)) ([9982d12](https://github.com/w3s-project/w3up/commit/9982d12b0a1f9a6da3f0d4264b9a35348e189dfb))
* test against actual api ([#1438](https://github.com/w3s-project/w3up/issues/1438)) ([f8132ca](https://github.com/w3s-project/w3up/commit/f8132ca1fced72a4addc7e9f0a2162e823c1ea5f))

## [13.0.2](https://github.com/w3s-project/w3up/compare/upload-api-v13.0.1...upload-api-v13.0.2) (2024-05-02)


### Fixes

* missing test export ([1fc6808](https://github.com/w3s-project/w3up/commit/1fc68087ccca5798cd9c633580025bef034bcadf))

## [13.0.1](https://github.com/w3s-project/w3up/compare/upload-api-v13.0.0...upload-api-v13.0.1) (2024-05-01)


### Fixes

* missing exports ([dec43e5](https://github.com/w3s-project/w3up/commit/dec43e51ee3b22a960a3769537c04f3de55d7097))


### Other Changes

* appease linter ([782c6d0](https://github.com/w3s-project/w3up/commit/782c6d0b3ca93ee801b38126339a262bcd713ede))

## [13.0.0](https://github.com/w3s-project/w3up/compare/upload-api-v12.0.0...upload-api-v13.0.0) (2024-05-01)


### ⚠ BREAKING CHANGES

* add `index/add` handler ([#1421](https://github.com/w3s-project/w3up/issues/1421))

### Features

* add `index/add` handler ([#1421](https://github.com/w3s-project/w3up/issues/1421)) ([cbe9524](https://github.com/w3s-project/w3up/commit/cbe952451b719fe7ae2f7480d26865eca80aba55))

## [12.0.0](https://github.com/w3s-project/w3up/compare/upload-api-v11.0.0...upload-api-v12.0.0) (2024-04-29)


### ⚠ BREAKING CHANGES

* restrict store API to CARs ([#1415](https://github.com/w3s-project/w3up/issues/1415))

### Features

* restrict store API to CARs ([#1415](https://github.com/w3s-project/w3up/issues/1415)) ([e53aa87](https://github.com/w3s-project/w3up/commit/e53aa87780446458ef9a19c88877073c1470d50e))

## [11.0.0](https://github.com/w3s-project/w3up/compare/upload-api-v10.0.1...upload-api-v11.0.0) (2024-04-26)


### ⚠ BREAKING CHANGES

* **capabilities:** `BlobMultihash` type in `@web3-storage/capabilities` renamed to `Multihash`.

### Features

* **capabilities:** add `index/add` capability ([#1410](https://github.com/w3s-project/w3up/issues/1410)) ([1b71b89](https://github.com/w3s-project/w3up/commit/1b71b89ed989cde8ef4bf35c1ebc333872cbc54c))

## [10.0.1](https://github.com/w3s-project/w3up/compare/upload-api-v10.0.0...upload-api-v10.0.1) (2024-04-25)


### Fixes

* add whitespace to trigger a release ([#1390](https://github.com/w3s-project/w3up/issues/1390)) ([ec95a0e](https://github.com/w3s-project/w3up/commit/ec95a0e5cf1bc08c6eabba1214b9803fda723393))
* migrate repo ([#1388](https://github.com/w3s-project/w3up/issues/1388)) ([10b7742](https://github.com/w3s-project/w3up/commit/10b7742d3f568f4b2dc1e2f435916a9e23480952))
* migrate repo ([#1389](https://github.com/w3s-project/w3up/issues/1389)) ([475a287](https://github.com/w3s-project/w3up/commit/475a28743ff9f7138b46dfe4227d3c80ed75a6a2))

## [10.0.0](https://github.com/web3-storage/w3up/compare/upload-api-v9.1.5...upload-api-v10.0.0) (2024-04-23)


### ⚠ BREAKING CHANGES

* allocations storage interface now requires remove to be implemented

### Features

* add blob list and remove ([#1385](https://github.com/web3-storage/w3up/issues/1385)) ([2f69946](https://github.com/web3-storage/w3up/commit/2f6994600e8cc0f70cedc5afe06003a2a0b70af3))

## [9.1.5](https://github.com/web3-storage/w3up/compare/upload-api-v9.1.4...upload-api-v9.1.5) (2024-04-18)


### Fixes

* allocation interface rename invocation to cause ([#1382](https://github.com/web3-storage/w3up/issues/1382)) ([2d13042](https://github.com/web3-storage/w3up/commit/2d1304243c2f21de449090261001a625008c5607))

## [9.1.4](https://github.com/web3-storage/w3up/compare/upload-api-v9.1.3...upload-api-v9.1.4) (2024-04-17)


### Fixes

* ucan conclude scheduler invocation type and improve test ([#1379](https://github.com/web3-storage/w3up/issues/1379)) ([11e0864](https://github.com/web3-storage/w3up/commit/11e0864bfdc49852127d2d55ef08954d775d7901))

## [9.1.3](https://github.com/web3-storage/w3up/compare/upload-api-v9.1.2...upload-api-v9.1.3) (2024-04-16)


### Fixes

* storage operation failed type name instead of store ([#1374](https://github.com/web3-storage/w3up/issues/1374)) ([a99251e](https://github.com/web3-storage/w3up/commit/a99251efc712888bf76270a4fe372163f938eddf))

## [9.1.2](https://github.com/web3-storage/w3up/compare/upload-api-v9.1.1...upload-api-v9.1.2) (2024-04-15)


### Fixes

* export test handlers and storages ([#1370](https://github.com/web3-storage/w3up/issues/1370)) ([61de1e1](https://github.com/web3-storage/w3up/commit/61de1e1eb4d2cee8eaea87913e8fd17ec17f1cd9))

## [9.1.1](https://github.com/web3-storage/w3up/compare/upload-api-v9.1.0...upload-api-v9.1.1) (2024-04-12)


### Fixes

* add errors to exports ([#1368](https://github.com/web3-storage/w3up/issues/1368)) ([27619c5](https://github.com/web3-storage/w3up/commit/27619c517e66321012f1c9ba0d8edb9c0037d6ff))

## [9.1.0](https://github.com/web3-storage/w3up/compare/upload-api-v9.0.1...upload-api-v9.1.0) (2024-04-12)


### Features

* blob, web3.storage and ucan conclude capabilities together with api handlers  ([#1342](https://github.com/web3-storage/w3up/issues/1342)) ([00735a8](https://github.com/web3-storage/w3up/commit/00735a80dfddbe86359af78ed9bd182f4804691f))

## [9.0.1](https://github.com/web3-storage/w3up/compare/upload-api-v9.0.0...upload-api-v9.0.1) (2024-04-12)


### Fixes

* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/web3-storage/w3up/issues/1359)) ([87ca098](https://github.com/web3-storage/w3up/commit/87ca098186fe204ff3409a2684719f1c54148c97))

## [9.0.0](https://github.com/web3-storage/w3up/compare/upload-api-v8.4.1...upload-api-v9.0.0) (2024-03-26)


### ⚠ BREAKING CHANGES

* release upload api with new filecoin api service for storefront ([#1347](https://github.com/web3-storage/w3up/issues/1347))

### Fixes

* release upload api with new filecoin api service for storefront ([#1347](https://github.com/web3-storage/w3up/issues/1347)) ([692751a](https://github.com/web3-storage/w3up/commit/692751aa6a178ede2820990ca9a44118bd6e8e55))

## [8.4.1](https://github.com/web3-storage/w3up/compare/upload-api-v8.4.0...upload-api-v8.4.1) (2024-03-20)


### Fixes

* missing exports ([#1335](https://github.com/web3-storage/w3up/issues/1335)) ([4e41ff4](https://github.com/web3-storage/w3up/commit/4e41ff4498cd75853204d9ae209fe36008cd8018))

## [8.4.0](https://github.com/web3-storage/w3up/compare/upload-api-v8.3.0...upload-api-v8.4.0) (2024-03-20)


### Features

* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/web3-storage/w3up/issues/1312)) ([d6978d7](https://github.com/web3-storage/w3up/commit/d6978d7ab299be76987c6533d18e6857f6998fe6))


### Fixes

* export UsageStorage ([#1334](https://github.com/web3-storage/w3up/issues/1334)) ([d466211](https://github.com/web3-storage/w3up/commit/d466211979e26698755f99daeaed8697c0ee2bdd))

## [8.3.0](https://github.com/web3-storage/w3up/compare/upload-api-v8.2.0...upload-api-v8.3.0) (2024-01-29)


### Features

* two more interface tweaks ([#1287](https://github.com/web3-storage/w3up/issues/1287)) ([bc3c364](https://github.com/web3-storage/w3up/commit/bc3c36452454398ea8e0f574aed44b318561ad94))

## [8.2.0](https://github.com/web3-storage/w3up/compare/upload-api-v8.1.0...upload-api-v8.2.0) (2024-01-29)


### Features

* add `set` method to `AccountPlan` ([#1281](https://github.com/web3-storage/w3up/issues/1281)) ([b94f0d4](https://github.com/web3-storage/w3up/commit/b94f0d48ea71454cef867feb9291c500f676faa3))


### Fixes

* one more tweak to the `PlanStorage` interface ([#1280](https://github.com/web3-storage/w3up/issues/1280)) ([5a44565](https://github.com/web3-storage/w3up/commit/5a44565feb33fc08102cd2559a2f22fb0476e86b))

## [8.1.0](https://github.com/web3-storage/w3up/compare/upload-api-v8.0.0...upload-api-v8.1.0) (2024-01-25)


### Features

* add `initialize` method to `PlansStorage` ([#1278](https://github.com/web3-storage/w3up/issues/1278)) ([6792126](https://github.com/web3-storage/w3up/commit/6792126d63a1e983713c3886eeba64038cb7cf34))
* change `plan/update` to `plan/set` and use existing `PlansStorage#set` to implement an invocation handler ([#1258](https://github.com/web3-storage/w3up/issues/1258)) ([1ccbfe9](https://github.com/web3-storage/w3up/commit/1ccbfe9f84ae5b2e99e315c92d15d2b54e9723ba))

## [8.0.0](https://github.com/web3-storage/w3up/compare/upload-api-v7.3.5...upload-api-v8.0.0) (2023-12-07)


### ⚠ BREAKING CHANGES

* return allocated bytes in `store/add` receipt ([#1213](https://github.com/web3-storage/w3up/issues/1213))

### Features

* return allocated bytes in `store/add` receipt ([#1213](https://github.com/web3-storage/w3up/issues/1213)) ([5d52e44](https://github.com/web3-storage/w3up/commit/5d52e447c14e7f7fd334e7ff575e032b7b0d89d7))

## [7.3.5](https://github.com/web3-storage/w3up/compare/upload-api-v7.3.4...upload-api-v7.3.5) (2023-11-29)


### Fixes

* floating promises and add no-floating-promises to eslint-config-w3up ([#1198](https://github.com/web3-storage/w3up/issues/1198)) ([1b8c5aa](https://github.com/web3-storage/w3up/commit/1b8c5aa86ec3d177bf77df4e2916699c1f522598))

## [7.3.4](https://github.com/web3-storage/w3up/compare/upload-api-v7.3.3...upload-api-v7.3.4) (2023-11-28)


### Fixes

* package metadata ([#1161](https://github.com/web3-storage/w3up/issues/1161)) ([b8a1cc2](https://github.com/web3-storage/w3up/commit/b8a1cc2e125a91be582998bda295e1ae1caab087))

## [7.3.3](https://github.com/web3-storage/w3up/compare/upload-api-v7.3.2...upload-api-v7.3.3) (2023-11-16)


### Bug Fixes

* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/web3-storage/w3up/issues/1141)) ([0b8d3f3](https://github.com/web3-storage/w3up/commit/0b8d3f3b52918b1b4d3b76ea6fea3fb0c837cd73))
* upgrade @ucanto/validator with bugfix ([#1151](https://github.com/web3-storage/w3up/issues/1151)) ([d4e961b](https://github.com/web3-storage/w3up/commit/d4e961bab09e88245e7d9323146849271e78eb57))

## [7.3.2](https://github.com/web3-storage/w3up/compare/upload-api-v7.3.1...upload-api-v7.3.2) (2023-11-15)


### Bug Fixes

* upgrade ucanto core ([#1127](https://github.com/web3-storage/w3up/issues/1127)) ([5ce4d22](https://github.com/web3-storage/w3up/commit/5ce4d2292d7e980da4a2ea0f1583f608a81157d2))

## [7.3.1](https://github.com/web3-storage/w3up/compare/upload-api-v7.3.0...upload-api-v7.3.1) (2023-11-09)


### Bug Fixes

* trigger release for upload api ([#1107](https://github.com/web3-storage/w3up/issues/1107)) ([9930b10](https://github.com/web3-storage/w3up/commit/9930b10962d365303ae45467a44f414aeac3dccb))

## [7.3.0](https://github.com/web3-storage/w3up/compare/upload-api-v7.2.0...upload-api-v7.3.0) (2023-11-09)


### Features

* add `subscription/list` capability ([#1088](https://github.com/web3-storage/w3up/issues/1088)) ([471d7e5](https://github.com/web3-storage/w3up/commit/471d7e5db24e12a06c1c52ae76bf95ff9471bac8))
* filecoin info ([#1091](https://github.com/web3-storage/w3up/issues/1091)) ([adb2442](https://github.com/web3-storage/w3up/commit/adb24424d1faf50daf2339b77c22fdd44faa236a))


### Bug Fixes

* lint ([#1095](https://github.com/web3-storage/w3up/issues/1095)) ([f9cc770](https://github.com/web3-storage/w3up/commit/f9cc77029d7c0651cb2961d08eca6f94dc1aef6c))

## [7.2.0](https://github.com/web3-storage/w3up/compare/upload-api-v7.1.2...upload-api-v7.2.0) (2023-11-07)


### Features

* add usage/report capability ([#1079](https://github.com/web3-storage/w3up/issues/1079)) ([6418b4b](https://github.com/web3-storage/w3up/commit/6418b4b22329a118fb258928bd9a6a45ced5ce45))
* optionally require plans for provisioning ([#1087](https://github.com/web3-storage/w3up/issues/1087)) ([b24731b](https://github.com/web3-storage/w3up/commit/b24731b0bdde785eef7785468cc1f49b92af2563))

## [7.1.2](https://github.com/web3-storage/w3up/compare/upload-api-v7.1.1...upload-api-v7.1.2) (2023-11-05)


### Bug Fixes

* revert enable storefront signer to be different from main service signer ([#1075](https://github.com/web3-storage/w3up/issues/1075)) ([80cdde0](https://github.com/web3-storage/w3up/commit/80cdde0f5b610cf6328dc17cb505759eddda821a))

## [7.1.1](https://github.com/web3-storage/w3up/compare/upload-api-v7.1.0...upload-api-v7.1.1) (2023-11-04)


### Bug Fixes

* enable storefront signer to be different from main service signer ([#1072](https://github.com/web3-storage/w3up/issues/1072)) ([21ded3c](https://github.com/web3-storage/w3up/commit/21ded3c171ca66480e4f74329943527dcc2bac3e))

## [7.1.0](https://github.com/web3-storage/w3up/compare/upload-api-v7.0.0...upload-api-v7.1.0) (2023-11-03)


### Features

* access agent proofs method would fail to return some session proofs ([#1047](https://github.com/web3-storage/w3up/issues/1047)) ([d23a1c9](https://github.com/web3-storage/w3up/commit/d23a1c972f91b855ee91f862da15bab0e68cca0a))
* expose test context of upload-api ([#1069](https://github.com/web3-storage/w3up/issues/1069)) ([f0757d1](https://github.com/web3-storage/w3up/commit/f0757d15fbe653ae4914960ac401385afd752e57))

## [7.0.0](https://github.com/web3-storage/w3up/compare/upload-api-v6.3.0...upload-api-v7.0.0) (2023-11-01)


### ⚠ BREAKING CHANGES

* add storefront filecoin api to upload api ([#1052](https://github.com/web3-storage/w3up/issues/1052))

### Features

* add storefront filecoin api to upload api ([#1052](https://github.com/web3-storage/w3up/issues/1052)) ([39916c2](https://github.com/web3-storage/w3up/commit/39916c25cbbfce6392fbb7cc71112987185c798c))
* implement `plan/get` capability ([#1005](https://github.com/web3-storage/w3up/issues/1005)) ([f0456d2](https://github.com/web3-storage/w3up/commit/f0456d2e2aab462666810e22abd7dfb7e1ce21be))

## [6.3.0](https://github.com/web3-storage/w3up/compare/upload-api-v6.2.0...upload-api-v6.3.0) (2023-10-25)


### Features

* allow customers to create more than one space ([#989](https://github.com/web3-storage/w3up/issues/989)) ([06e0ca9](https://github.com/web3-storage/w3up/commit/06e0ca9fd3e34104002023f81fc605b666ef9a5b))


### Bug Fixes

* fix arethetypesworking errors in all packages ([#1004](https://github.com/web3-storage/w3up/issues/1004)) ([2e2936a](https://github.com/web3-storage/w3up/commit/2e2936a3831389dd13be5be5146a04e2b15553c5))

## [6.2.0](https://github.com/web3-storage/w3up/compare/upload-api-v6.1.0...upload-api-v6.2.0) (2023-10-20)


### Features

* add `store/get` and `upload/get` capabilities ([#942](https://github.com/web3-storage/w3up/issues/942)) ([40c79eb](https://github.com/web3-storage/w3up/commit/40c79eb8f246775b9e1828240f271fa75ef696be))

## [6.1.0](https://github.com/web3-storage/w3up/compare/upload-api-v6.0.0...upload-api-v6.1.0) (2023-10-19)


### Features

* add revocation to access-client and w3up-client ([#975](https://github.com/web3-storage/w3up/issues/975)) ([6c877aa](https://github.com/web3-storage/w3up/commit/6c877aac78eddb924e999dc3270cba010e48e30a))

## [6.0.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.9.0...upload-api-v6.0.0) (2023-10-13)


### ⚠ BREAKING CHANGES

* Returning the `size` means that we need to fetch the stored item beforehand, and if it does not exist throw a `StoreItemNotFound` error. This is a change from the current behaviour which returns successfully even if the item is not present in the space.

### Features

* add size to `store/remove` receipt ([#969](https://github.com/web3-storage/w3up/issues/969)) ([d2100eb](https://github.com/web3-storage/w3up/commit/d2100eb0ffa5968c326d58d583a258187f9119eb))

## [5.9.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.8.0...upload-api-v5.9.0) (2023-10-10)


### Features

* revocation handler ([#960](https://github.com/web3-storage/w3up/issues/960)) ([91f52c6](https://github.com/web3-storage/w3up/commit/91f52c6d35e4aea2a98c75d8b95ff61cdffac452))
* upgrade to ucanto@9 ([#951](https://github.com/web3-storage/w3up/issues/951)) ([d72faf1](https://github.com/web3-storage/w3up/commit/d72faf1bb07dd11462ae6dff8ee0469f8ae7e9e7))

## [5.8.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.7.0...upload-api-v5.8.0) (2023-10-06)


### Features

* Add basic README to upload-api ([#949](https://github.com/web3-storage/w3up/issues/949)) ([d09db73](https://github.com/web3-storage/w3up/commit/d09db734da5eec55d5a21106fecc07bddd5f14dc))

## [5.7.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.6.0...upload-api-v5.7.0) (2023-10-05)


### Features

* add `RevocationsStorage` ([#941](https://github.com/web3-storage/w3up/issues/941)) ([0069701](https://github.com/web3-storage/w3up/commit/0069701c76eff9ce0ac229658d217dac42d9adc8))

## [5.6.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.5.0...upload-api-v5.6.0) (2023-09-18)


### Features

* rename getCID to inspect ([#931](https://github.com/web3-storage/w3up/issues/931)) ([2f8dbe6](https://github.com/web3-storage/w3up/commit/2f8dbe6bfbfbac2e2f4b8819e5fa91f8141df1bf))

## [5.5.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.4.0...upload-api-v5.5.0) (2023-09-14)


### Features

* reorg tests ([#926](https://github.com/web3-storage/w3up/issues/926)) ([946db3c](https://github.com/web3-storage/w3up/commit/946db3c329c893139ee3e5eac640899796aa307c))

## [5.4.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.3.1...upload-api-v5.4.0) (2023-09-13)


### Features

* implement `admin/upload/inspect` and `admin/store/inspect` capabilities ([#918](https://github.com/web3-storage/w3up/issues/918)) ([5616a12](https://github.com/web3-storage/w3up/commit/5616a12125500a1d5ee41f0504812d82c0451852))

## [5.3.1](https://github.com/web3-storage/w3up/compare/upload-api-v5.3.0...upload-api-v5.3.1) (2023-09-12)


### Bug Fixes

* store add should validate size right away ([#917](https://github.com/web3-storage/w3up/issues/917)) ([2770e6c](https://github.com/web3-storage/w3up/commit/2770e6cfde60236b12d043caa72fd944f6b80918))

## [5.3.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.2.0...upload-api-v5.3.0) (2023-09-05)


### Features

* make agent Service generic ([#875](https://github.com/web3-storage/w3up/issues/875)) ([cdfe36d](https://github.com/web3-storage/w3up/commit/cdfe36dc7298e92066d0454144f598b0e0535b19))


### Bug Fixes

* add a test that exercises ProvisionsStorage#getConsumer ([#893](https://github.com/web3-storage/w3up/issues/893)) ([ed60572](https://github.com/web3-storage/w3up/commit/ed605725a71102b6584bb1c7039ee1a1f50dd7c6))

## [5.2.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.1.0...upload-api-v5.2.0) (2023-08-28)


### Features

* return ID from ProvisionsStorage `put` ([#869](https://github.com/web3-storage/w3up/issues/869)) ([d165c23](https://github.com/web3-storage/w3up/commit/d165c234d8ee6bf0fa31e954b3743d39c6d91699))

## [5.1.0](https://github.com/web3-storage/w3up/compare/upload-api-v5.0.0...upload-api-v5.1.0) (2023-08-22)


### Features

* add providers to space/info ([#862](https://github.com/web3-storage/w3up/issues/862)) ([ac72921](https://github.com/web3-storage/w3up/commit/ac7292177767e6456492200653f0a8b33a4cd98e))
* add subscriptions to CustomerGetSuccess ([#863](https://github.com/web3-storage/w3up/issues/863)) ([dd2e77c](https://github.com/web3-storage/w3up/commit/dd2e77c51d84a517cb50ff05199b8eebf9223bf2))
* change "total" to "limit" ([#867](https://github.com/web3-storage/w3up/issues/867)) ([8295070](https://github.com/web3-storage/w3up/commit/8295070c8fbbc508da2cfe6f32846090a530f282))


### Bug Fixes

* re-enable upload-api tests ([#864](https://github.com/web3-storage/w3up/issues/864)) ([d76a6af](https://github.com/web3-storage/w3up/commit/d76a6af5b48aae60e66f164f61f3c9e010395f29))

## [5.0.0](https://github.com/web3-storage/w3up/compare/upload-api-v4.1.0...upload-api-v5.0.0) (2023-08-09)


### ⚠ BREAKING CHANGES

* introduce new administrative capabilities ([#832](https://github.com/web3-storage/w3up/issues/832))

### Features

* introduce new administrative capabilities ([#832](https://github.com/web3-storage/w3up/issues/832)) ([7b8037a](https://github.com/web3-storage/w3up/commit/7b8037a6ab92f830af4aa7ba07a91bc2a20c0d8c))


### Bug Fixes

* run format for upload-api ([#825](https://github.com/web3-storage/w3up/issues/825)) ([59dc765](https://github.com/web3-storage/w3up/commit/59dc7659a6a19942fad5f73efbed84cc33381314))

## [4.1.0](https://github.com/web3-storage/w3up/compare/upload-api-v4.0.0...upload-api-v4.1.0) (2023-06-20)


### Features

* add failure type to DelegationsStorage#putMany return ([#819](https://github.com/web3-storage/w3up/issues/819)) ([ae7b7c6](https://github.com/web3-storage/w3up/commit/ae7b7c651b57cd514b9429677a420fd14237b8a8))

## [4.0.0](https://github.com/web3-storage/w3up/compare/upload-api-v3.0.0...upload-api-v4.0.0) (2023-06-08)


### ⚠ BREAKING CHANGES

* merge `@web3-storage/access-api` into `@web3-storage/upload-api` ([#790](https://github.com/web3-storage/w3up/issues/790))

### Features

* merge `@web3-storage/access-api` into `@web3-storage/upload-api` ([#790](https://github.com/web3-storage/w3up/issues/790)) ([4f6ddb6](https://github.com/web3-storage/w3up/commit/4f6ddb690c365a42a3dc4c5c6898e4999bd0f868))


### Bug Fixes

* upgrade remaining ucanto deps ([#798](https://github.com/web3-storage/w3up/issues/798)) ([7211501](https://github.com/web3-storage/w3up/commit/72115010663a62140127cdeed21f2dc37f59da08))
* upgrade ucanto to 8 ([#794](https://github.com/web3-storage/w3up/issues/794)) ([00b011d](https://github.com/web3-storage/w3up/commit/00b011d87f628d4b3040398ca6cba567a69713ff))
* use legacy codec on upload api ([#788](https://github.com/web3-storage/w3up/issues/788)) ([1514474](https://github.com/web3-storage/w3up/commit/151447414f79e9df5aba1873b962c9c2efed1935))
* use legacy codec on upload api ([#788](https://github.com/web3-storage/w3up/issues/788)) ([84a4d44](https://github.com/web3-storage/w3up/commit/84a4d440ffa0be1ea4962b32070c12b83cc95562))

## [3.0.0](https://github.com/web3-storage/w3up/compare/upload-api-v2.0.0...upload-api-v3.0.0) (2023-05-03)


### ⚠ BREAKING CHANGES

* upgrade to ucanto7.x.x ([#774](https://github.com/web3-storage/w3up/issues/774))

### Features

* upgrade to ucanto7.x.x ([#774](https://github.com/web3-storage/w3up/issues/774)) ([0cc6e66](https://github.com/web3-storage/w3up/commit/0cc6e66a80476e05c75bea94c1bee9bd12cbacf5))

## [2.0.0](https://github.com/web3-storage/w3protocol/compare/upload-api-v1.0.4...upload-api-v2.0.0) (2023-03-23)


### ⚠ BREAKING CHANGES

* ucan bucket is not part of upload-api but rather ucan-api
* implement new account-based multi-device flow ([#433](https://github.com/web3-storage/w3protocol/issues/433))

### Features

* implement new account-based multi-device flow ([#433](https://github.com/web3-storage/w3protocol/issues/433)) ([1ddc6a0](https://github.com/web3-storage/w3protocol/commit/1ddc6a0c53f8cdb6837a315d8aaf567100dfb8d7))


### Bug Fixes

* remove ucan bucket interface ([#594](https://github.com/web3-storage/w3protocol/issues/594)) ([52cf7c1](https://github.com/web3-storage/w3protocol/commit/52cf7c1f35f01aac66d475d884b87f29348a145c))


### Miscellaneous Chores

* **access-client:** release 11.0.0-rc.0 ([#573](https://github.com/web3-storage/w3protocol/issues/573)) ([be4386d](https://github.com/web3-storage/w3protocol/commit/be4386d66ceea393f289adb3c79273c250542807))

## [1.0.4](https://github.com/web3-storage/w3protocol/compare/upload-api-v1.0.3...upload-api-v1.0.4) (2023-03-08)


### Bug Fixes

* **upload-api:** include test types in the package ([#513](https://github.com/web3-storage/w3protocol/issues/513)) ([0c7a452](https://github.com/web3-storage/w3protocol/commit/0c7a452af99757aa34871c4d5c9d77938934892e))

## [1.0.3](https://github.com/web3-storage/w3protocol/compare/upload-api-v1.0.2...upload-api-v1.0.3) (2023-03-08)


### Bug Fixes

* switch upload-api to node16 ([#509](https://github.com/web3-storage/w3protocol/issues/509)) ([698a033](https://github.com/web3-storage/w3protocol/commit/698a03391221aceb1ce602c407587497d97a77ed))
* types so that w3infra would have been evident ([#507](https://github.com/web3-storage/w3protocol/issues/507)) ([544a838](https://github.com/web3-storage/w3protocol/commit/544a838fa16b316825f69fd95fcb5e35002ac958))

## [1.0.2](https://github.com/web3-storage/w3protocol/compare/upload-api-v1.0.1...upload-api-v1.0.2) (2023-03-08)


### Bug Fixes

* **upload-api:** fix incompatibilities with w3infra ([#504](https://github.com/web3-storage/w3protocol/issues/504)) ([d3dcf34](https://github.com/web3-storage/w3protocol/commit/d3dcf3493030abba62da2e16ffa52107e18d6fa8))

## [1.0.1](https://github.com/web3-storage/w3protocol/compare/upload-api-v1.0.0...upload-api-v1.0.1) (2023-03-08)


### Bug Fixes

* release upload api ([#501](https://github.com/web3-storage/w3protocol/issues/501)) ([23d536a](https://github.com/web3-storage/w3protocol/commit/23d536af6f323311721aecf75ca77b7a19f88643))

## 1.0.0 (2023-03-08)


### Features

* Migrate store/* & upload/* APIs ([#485](https://github.com/web3-storage/w3protocol/issues/485)) ([f0b1e73](https://github.com/web3-storage/w3protocol/commit/f0b1e737f4d2f1689c5da04ad5408b114928d2fe))
* upgrade to new ucanto ([#498](https://github.com/web3-storage/w3protocol/issues/498)) ([dcb41a9](https://github.com/web3-storage/w3protocol/commit/dcb41a9981c2b6bebbdbd29debcad9f510383680))
