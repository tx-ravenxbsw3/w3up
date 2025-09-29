# Changelog

## [9.0.0](https://github.com/tx-ravenxbsw3/w3up/compare/filecoin-api-v8.0.0...filecoin-api-v9.0.0) (2025-09-29)


### ⚠ BREAKING CHANGES

* content serve authorization ([#1590](https://github.com/tx-ravenxbsw3/w3up/issues/1590))
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/tx-ravenxbsw3/w3up/issues/1444))
* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344))
* dataStore in storefront renamed to contentStore
* not possible to skip submit queue on storefront service anymore
* return allocated bytes in `store/add` receipt ([#1213](https://github.com/tx-ravenxbsw3/w3up/issues/1213))
* add storefront filecoin api to upload api ([#1052](https://github.com/tx-ravenxbsw3/w3up/issues/1052))
* upgrade data segment v4 ([#996](https://github.com/tx-ravenxbsw3/w3up/issues/996))

### Features

* add blob protocol to upload-client ([#1425](https://github.com/tx-ravenxbsw3/w3up/issues/1425)) ([44bde76](https://github.com/tx-ravenxbsw3/w3up/commit/44bde7616adc94f82cfef751bcaa94cf59bf24c5))
* add storefront filecoin api to upload api ([#1052](https://github.com/tx-ravenxbsw3/w3up/issues/1052)) ([e71373f](https://github.com/tx-ravenxbsw3/w3up/commit/e71373f3536edf92d94e23eaf8d2a1bc3b95ada6))
* add support to prepend pieces while buffering to aggregate ([#1301](https://github.com/tx-ravenxbsw3/w3up/issues/1301)) ([0c9a448](https://github.com/tx-ravenxbsw3/w3up/commit/0c9a448a0e15236c9286063eb7c42003983f15cf))
* add usage/report capability ([#1079](https://github.com/tx-ravenxbsw3/w3up/issues/1079)) ([95db863](https://github.com/tx-ravenxbsw3/w3up/commit/95db8632ce796ff698d7b016cca6e676e846eeac))
* aggregator keeping oldest piece ts ([#1188](https://github.com/tx-ravenxbsw3/w3up/issues/1188)) ([db3285c](https://github.com/tx-ravenxbsw3/w3up/commit/db3285c0e3ad84c17550a9e53d33670de3610957))
* api waits for trigger filecoin pipeline from the client ([#1332](https://github.com/tx-ravenxbsw3/w3up/issues/1332)) ([7d005e2](https://github.com/tx-ravenxbsw3/w3up/commit/7d005e2de0f51abecd27139af1cb7996624512db))
* content serve authorization ([#1590](https://github.com/tx-ravenxbsw3/w3up/issues/1590)) ([c752277](https://github.com/tx-ravenxbsw3/w3up/commit/c752277cc07008437fc4482ea5689a1cabc92abf))
* deprecate issuer ([#1344](https://github.com/tx-ravenxbsw3/w3up/issues/1344)) ([db98e3a](https://github.com/tx-ravenxbsw3/w3up/commit/db98e3ad7fd5ce589ab5f002a9e614341f9121ca))
* external login ([#1629](https://github.com/tx-ravenxbsw3/w3up/issues/1629)) ([638c31c](https://github.com/tx-ravenxbsw3/w3up/commit/638c31c5ae06fa73264b2fa45cd223fc2f7cc704))
* filecoin info ([#1091](https://github.com/tx-ravenxbsw3/w3up/issues/1091)) ([ad4e328](https://github.com/tx-ravenxbsw3/w3up/commit/ad4e32852f9f804163ef813bae47d2d430b6cac1))
* **filecoin-api:** allow custom hashing function to be passed to aggregate builder ([#1553](https://github.com/tx-ravenxbsw3/w3up/issues/1553)) ([0786181](https://github.com/tx-ravenxbsw3/w3up/commit/078618192f2be7f1fc5bc38de42bc7b6980847cd))
* **filecoin-api:** paginated queries ([#1521](https://github.com/tx-ravenxbsw3/w3up/issues/1521)) ([fc2adb2](https://github.com/tx-ravenxbsw3/w3up/commit/fc2adb210bb76de87955fbb5039304d35e295bf6))
* move aggregate information out of deals in filecoin/info ([#1192](https://github.com/tx-ravenxbsw3/w3up/issues/1192)) ([49e1363](https://github.com/tx-ravenxbsw3/w3up/commit/49e1363925acb1224e62f9ae4e9df4464cf6281d))
* return allocated bytes in `store/add` receipt ([#1213](https://github.com/tx-ravenxbsw3/w3up/issues/1213)) ([a243e22](https://github.com/tx-ravenxbsw3/w3up/commit/a243e221153a8107ad92218f545d20ab1b3bd120))
* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/tx-ravenxbsw3/w3up/issues/1312)) ([5ed0f70](https://github.com/tx-ravenxbsw3/w3up/commit/5ed0f708d74745ae86c6c69c436a7dffb9c9d7c8))
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/tx-ravenxbsw3/w3up/issues/1444)) ([bd4885b](https://github.com/tx-ravenxbsw3/w3up/commit/bd4885b3a88216cd3402749bd03fa4682e5a7495))
* upload-client uploadDirectory, by default, sorts the provided files by file name to help the user call us in a way that is deterministic and minimizes cost ([#1173](https://github.com/tx-ravenxbsw3/w3up/issues/1173)) ([6cf5f4c](https://github.com/tx-ravenxbsw3/w3up/commit/6cf5f4ce4c77d02579ae2263e7cf028066f278ab))
* use digest in `blob/accept` location commitment ([#1480](https://github.com/tx-ravenxbsw3/w3up/issues/1480)) ([b1784af](https://github.com/tx-ravenxbsw3/w3up/commit/b1784aff914d2d6be2d9b2d914b80699b9e660cc))


### Fixes

* aggregate accept must query with aggregate only ([#1024](https://github.com/tx-ravenxbsw3/w3up/issues/1024)) ([a3dba5b](https://github.com/tx-ravenxbsw3/w3up/commit/a3dba5b88672ca34edd098b3c928d994b1b6c0e1))
* aggregate accept should rely on deal tracker response to issue receipt ([#1038](https://github.com/tx-ravenxbsw3/w3up/issues/1038)) ([efc849f](https://github.com/tx-ravenxbsw3/w3up/commit/efc849f4bb67d6514081f9642cee814d1be6ee0a))
* aggregate offer invocation cid wrong ([#1063](https://github.com/tx-ravenxbsw3/w3up/issues/1063)) ([ed6cca3](https://github.com/tx-ravenxbsw3/w3up/commit/ed6cca3495d0299008210508767be26dbac61dd9))
* aggregator event tests ([#1048](https://github.com/tx-ravenxbsw3/w3up/issues/1048)) ([b6daf6e](https://github.com/tx-ravenxbsw3/w3up/commit/b6daf6ea5012ac39d5de844841b58ac19624a738))
* aggregator events inclusion record type simplified ([#1050](https://github.com/tx-ravenxbsw3/w3up/issues/1050)) ([11c6670](https://github.com/tx-ravenxbsw3/w3up/commit/11c667015697bef3aa48594db15ea122b58bdc55))
* aggregator service types have unused types ([#1039](https://github.com/tx-ravenxbsw3/w3up/issues/1039)) ([d60ae67](https://github.com/tx-ravenxbsw3/w3up/commit/d60ae672efd1dbccc3bd02f77e83fe236b042b48))
* avoid duplicates on aggregator buffer concat ([#1259](https://github.com/tx-ravenxbsw3/w3up/issues/1259)) ([47f7aa0](https://github.com/tx-ravenxbsw3/w3up/commit/47f7aa0adcca83f529d5cb703752deaf76515ed0))
* check service did in w3filecoin ([#1476](https://github.com/tx-ravenxbsw3/w3up/issues/1476)) ([4afa351](https://github.com/tx-ravenxbsw3/w3up/commit/4afa3516eac214ea9090f8b15dd5689555cb7a5e))
* configure max pieces ([#1566](https://github.com/tx-ravenxbsw3/w3up/issues/1566)) ([def8b1f](https://github.com/tx-ravenxbsw3/w3up/commit/def8b1f934fd3bb3bb7e9db507980bc7c33bec8d))
* dealer aggregate store query type does not need aggregate anymore ([#1042](https://github.com/tx-ravenxbsw3/w3up/issues/1042)) ([2f77d9a](https://github.com/tx-ravenxbsw3/w3up/commit/2f77d9a2287ddc3ccbb8606ee4599803e14478b7))
* dealer offer store keys without space ([#1066](https://github.com/tx-ravenxbsw3/w3up/issues/1066)) ([04bd896](https://github.com/tx-ravenxbsw3/w3up/commit/04bd896fadda97182790dc990b5b069e946faa10))
* drop filecoin storefront skip submit queue option ([#1371](https://github.com/tx-ravenxbsw3/w3up/issues/1371)) ([7b582b2](https://github.com/tx-ravenxbsw3/w3up/commit/7b582b2c5f3c243b12027fd8e3bc3bb5c24c23ac))
* enable storefront signer to be different from main service signer ([#1072](https://github.com/tx-ravenxbsw3/w3up/issues/1072)) ([aaf9daf](https://github.com/tx-ravenxbsw3/w3up/commit/aaf9daf4d13b552a2f1e70b762483e7b52c8c389))
* filecoin api store has returns false ([#1022](https://github.com/tx-ravenxbsw3/w3up/issues/1022)) ([1da121f](https://github.com/tx-ravenxbsw3/w3up/commit/1da121f5e74eb27f22d4800534bd9eeb08e07165))
* filecoin api test service context explicit exported ([#1034](https://github.com/tx-ravenxbsw3/w3up/issues/1034)) ([dad99ce](https://github.com/tx-ravenxbsw3/w3up/commit/dad99ce8d3898e1a52dce6d1ebb123294124a10b))
* filecoin test use blob ([#1422](https://github.com/tx-ravenxbsw3/w3up/issues/1422)) ([bb37641](https://github.com/tx-ravenxbsw3/w3up/commit/bb37641d5641d3bff879187597b02ae3d1e18674))
* **filecoin-api:** parallel put to piece accept queue ([#1560](https://github.com/tx-ravenxbsw3/w3up/issues/1560)) ([3b7a8f4](https://github.com/tx-ravenxbsw3/w3up/commit/3b7a8f4bb2fefeb7ea7d6b852b06cecac895b2de))
* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/tx-ravenxbsw3/w3up/issues/1141)) ([93980ef](https://github.com/tx-ravenxbsw3/w3up/commit/93980ef8759b01b689a017aa7ae5a06d83284948))
* lint ([#1095](https://github.com/tx-ravenxbsw3/w3up/issues/1095)) ([6b37256](https://github.com/tx-ravenxbsw3/w3up/commit/6b37256cbaac1246812e6200b7a23cd7dd61165d))
* migrate repo ([#1389](https://github.com/tx-ravenxbsw3/w3up/issues/1389)) ([9e18c76](https://github.com/tx-ravenxbsw3/w3up/commit/9e18c761e63c88e395b66b4f7cbadc79fc837dec))
* package metadata ([#1161](https://github.com/tx-ravenxbsw3/w3up/issues/1161)) ([68b41e4](https://github.com/tx-ravenxbsw3/w3up/commit/68b41e49f4e77aabe07594b22691b2febdb3ea91))
* receipt chain has wrong CID because no expiration is set ([#1060](https://github.com/tx-ravenxbsw3/w3up/issues/1060)) ([ef4f886](https://github.com/tx-ravenxbsw3/w3up/commit/ef4f8863bd64e0a7941278b850db74efd10b0c7f))
* rename blob and index client capabilities ([#1478](https://github.com/tx-ravenxbsw3/w3up/issues/1478)) ([ee5a89c](https://github.com/tx-ravenxbsw3/w3up/commit/ee5a89cac2248e634bd4e835270d052cdbb31aef))
* repo URLs ([#1550](https://github.com/tx-ravenxbsw3/w3up/issues/1550)) ([6fd5aa3](https://github.com/tx-ravenxbsw3/w3up/commit/6fd5aa32e9cfb5633ec662363e6a48493b1f8cf0))
* return piece accept receipt error ([#1512](https://github.com/tx-ravenxbsw3/w3up/issues/1512)) ([5266e6a](https://github.com/tx-ravenxbsw3/w3up/commit/5266e6a50626b9da45cdbaead0268cbf61647481))
* revert enable storefront signer to be different from main service signer ([#1075](https://github.com/tx-ravenxbsw3/w3up/issues/1075)) ([ccf78a1](https://github.com/tx-ravenxbsw3/w3up/commit/ccf78a1192020c5189d76a41bfa642ccb12083af))
* storefront content store rename and separation for test ([#1409](https://github.com/tx-ravenxbsw3/w3up/issues/1409)) ([093677d](https://github.com/tx-ravenxbsw3/w3up/commit/093677d862f39ade1a5628dbe9ab7e464134268b))
* storefront events cron with max concurrency ([#1191](https://github.com/tx-ravenxbsw3/w3up/issues/1191)) ([7a7cb17](https://github.com/tx-ravenxbsw3/w3up/commit/7a7cb175c031da0db4b5030b53a94627cf5dc486))
* storefront principal type on cron ([#1055](https://github.com/tx-ravenxbsw3/w3up/issues/1055)) ([a097172](https://github.com/tx-ravenxbsw3/w3up/commit/a09717236d73def70b3f4441aee01983700a2c1f))
* trigger release filecoin api ([#1032](https://github.com/tx-ravenxbsw3/w3up/issues/1032)) ([4e5855b](https://github.com/tx-ravenxbsw3/w3up/commit/4e5855b2dbae79e2748b9d665061add554a6aa88))
* typo dealer event function name ([#1040](https://github.com/tx-ravenxbsw3/w3up/issues/1040)) ([4339d26](https://github.com/tx-ravenxbsw3/w3up/commit/4339d26b5015bc2d33093d9443933410535b116e))
* upgrade data segment v4 ([#996](https://github.com/tx-ravenxbsw3/w3up/issues/996)) ([04b4d1e](https://github.com/tx-ravenxbsw3/w3up/commit/04b4d1e3293dce859a43b433ac76447b4a22b2e0))
* upgrade ucanto core ([#1127](https://github.com/tx-ravenxbsw3/w3up/issues/1127)) ([40b3257](https://github.com/tx-ravenxbsw3/w3up/commit/40b32571b42ff63f37d5020299ebb013e1886286))
* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/tx-ravenxbsw3/w3up/issues/1359)) ([6ca062f](https://github.com/tx-ravenxbsw3/w3up/commit/6ca062fad73a442b81553fc79fd75923ff9e1bcf))
* use one-webcrypto from npm ([#1525](https://github.com/tx-ravenxbsw3/w3up/issues/1525)) ([f72908a](https://github.com/tx-ravenxbsw3/w3up/commit/f72908a60b758c78f5b9d33ba790d3c4ff8c566f))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/tx-ravenxbsw3/w3up/issues/1533)) ([47cc600](https://github.com/tx-ravenxbsw3/w3up/commit/47cc6006b1b7316c6815dfdca0a55122f632fec3))
* appease linter ([0f49e0c](https://github.com/tx-ravenxbsw3/w3up/commit/0f49e0ce451946d909be4a788e934a126fec5812))
* export context utils from filecoin api ([#1031](https://github.com/tx-ravenxbsw3/w3up/issues/1031)) ([9679f17](https://github.com/tx-ravenxbsw3/w3up/commit/9679f1752681769d49f8c227e181255a36762a2d))
* **main:** release filecoin-api 2.0.3 ([#1009](https://github.com/tx-ravenxbsw3/w3up/issues/1009)) ([000f94a](https://github.com/tx-ravenxbsw3/w3up/commit/000f94afd07027f41b0b41bd72d573f36f3f2213))
* **main:** release filecoin-api 3.0.0 ([#1020](https://github.com/tx-ravenxbsw3/w3up/issues/1020)) ([ec0c44e](https://github.com/tx-ravenxbsw3/w3up/commit/ec0c44e6d45c1007ab26def06fc45274dae3458e))
* **main:** release filecoin-api 3.0.1 ([#1023](https://github.com/tx-ravenxbsw3/w3up/issues/1023)) ([0f1d8bf](https://github.com/tx-ravenxbsw3/w3up/commit/0f1d8bf6bd95c4c86633c2971c305c2d6f904b2a))
* **main:** release filecoin-api 3.0.2 ([#1025](https://github.com/tx-ravenxbsw3/w3up/issues/1025)) ([bb6f9eb](https://github.com/tx-ravenxbsw3/w3up/commit/bb6f9ebfd30576fc9869d09b32c74a2ba62e7c74))
* **main:** release filecoin-api 3.0.3 ([#1033](https://github.com/tx-ravenxbsw3/w3up/issues/1033)) ([e8dce72](https://github.com/tx-ravenxbsw3/w3up/commit/e8dce728f8c72819b05c731d53bd90e29bf33630))
* **main:** release filecoin-api 3.0.4 ([#1035](https://github.com/tx-ravenxbsw3/w3up/issues/1035)) ([3c9e047](https://github.com/tx-ravenxbsw3/w3up/commit/3c9e0472977879d9e939b322be9c7b3ec326e6c5))
* **main:** release filecoin-api 3.0.5 ([#1041](https://github.com/tx-ravenxbsw3/w3up/issues/1041)) ([c162dd1](https://github.com/tx-ravenxbsw3/w3up/commit/c162dd1286b02e5a0b1e93bf0f3a2eff86f1c444))
* **main:** release filecoin-api 3.0.6 ([#1043](https://github.com/tx-ravenxbsw3/w3up/issues/1043)) ([264f296](https://github.com/tx-ravenxbsw3/w3up/commit/264f296c9583dcbd53cc2f4b2b35e6470be9e047))
* **main:** release filecoin-api 3.0.7 ([#1049](https://github.com/tx-ravenxbsw3/w3up/issues/1049)) ([b5e3b8b](https://github.com/tx-ravenxbsw3/w3up/commit/b5e3b8b26e31d9aae0386155e64e708327785467))
* **main:** release filecoin-api 3.0.8 ([#1051](https://github.com/tx-ravenxbsw3/w3up/issues/1051)) ([ddb2f1f](https://github.com/tx-ravenxbsw3/w3up/commit/ddb2f1fa2bcb66a6bcb6b52108157a321fff95a5))
* **main:** release filecoin-api 4.0.0 ([#1054](https://github.com/tx-ravenxbsw3/w3up/issues/1054)) ([f8054e5](https://github.com/tx-ravenxbsw3/w3up/commit/f8054e5b4592cd5cc5c0870157037f6e47d93aa1))
* **main:** release filecoin-api 4.0.1 ([#1056](https://github.com/tx-ravenxbsw3/w3up/issues/1056)) ([640c102](https://github.com/tx-ravenxbsw3/w3up/commit/640c102b5a1102895bf84f13c8455a3ba0f555fa))
* **main:** release filecoin-api 4.0.2 ([#1061](https://github.com/tx-ravenxbsw3/w3up/issues/1061)) ([fae204e](https://github.com/tx-ravenxbsw3/w3up/commit/fae204e5c3d115c9e1a0fa5e1016edcbedbc6f7d))
* **main:** release filecoin-api 4.0.3 ([#1064](https://github.com/tx-ravenxbsw3/w3up/issues/1064)) ([aff40c6](https://github.com/tx-ravenxbsw3/w3up/commit/aff40c6d3306ba874d07bbd2917b048297528c52))
* **main:** release filecoin-api 4.0.4 ([#1067](https://github.com/tx-ravenxbsw3/w3up/issues/1067)) ([451375b](https://github.com/tx-ravenxbsw3/w3up/commit/451375bb433544369be719d40e8d6b173deca324))
* **main:** release filecoin-api 4.0.5 ([#1073](https://github.com/tx-ravenxbsw3/w3up/issues/1073)) ([72e11d9](https://github.com/tx-ravenxbsw3/w3up/commit/72e11d9582e0ae6f3fa61110a372b57ee487bffb))
* **main:** release filecoin-api 4.0.6 ([#1077](https://github.com/tx-ravenxbsw3/w3up/issues/1077)) ([8256d28](https://github.com/tx-ravenxbsw3/w3up/commit/8256d285368b3e24fe3c86175add0a2a845422c7))
* **main:** release filecoin-api 4.1.0 ([#1085](https://github.com/tx-ravenxbsw3/w3up/issues/1085)) ([3b7d8ff](https://github.com/tx-ravenxbsw3/w3up/commit/3b7d8ff1f7d9ad18f04f108aa49d08d8b54ed5ed))
* **main:** release filecoin-api 4.1.1 ([#1133](https://github.com/tx-ravenxbsw3/w3up/issues/1133)) ([b66b0f2](https://github.com/tx-ravenxbsw3/w3up/commit/b66b0f28e2fd239805278dec813af258bfbefe41))
* **main:** release filecoin-api 4.1.2 ([#1148](https://github.com/tx-ravenxbsw3/w3up/issues/1148)) ([7317d19](https://github.com/tx-ravenxbsw3/w3up/commit/7317d1959745f30f0acf8bb36e547b1d423faf5f))
* **main:** release filecoin-api 4.2.0 ([#1164](https://github.com/tx-ravenxbsw3/w3up/issues/1164)) ([723ea78](https://github.com/tx-ravenxbsw3/w3up/commit/723ea7852cb1046147abe73bf2412c9f018ade7a))
* **main:** release filecoin-api 4.3.0 ([#1194](https://github.com/tx-ravenxbsw3/w3up/issues/1194)) ([66cf531](https://github.com/tx-ravenxbsw3/w3up/commit/66cf53197cc0cce58f76b79f70a50a8b96aabd8e))
* **main:** release filecoin-api 4.3.1 ([#1205](https://github.com/tx-ravenxbsw3/w3up/issues/1205)) ([51c58b4](https://github.com/tx-ravenxbsw3/w3up/commit/51c58b4f7c27121944fd7b55328242b606dae5a1))
* **main:** release filecoin-api 4.4.0 ([#1303](https://github.com/tx-ravenxbsw3/w3up/issues/1303)) ([07506fd](https://github.com/tx-ravenxbsw3/w3up/commit/07506fd7beb912ee5ad6bec30ed42eb6b8b730ac))
* **main:** release filecoin-api 4.5.0 ([#1314](https://github.com/tx-ravenxbsw3/w3up/issues/1314)) ([ec082de](https://github.com/tx-ravenxbsw3/w3up/commit/ec082dece0bc64aa187ca31db77c099917cda609))
* **main:** release filecoin-api 4.6.0 ([#1346](https://github.com/tx-ravenxbsw3/w3up/issues/1346)) ([5173d87](https://github.com/tx-ravenxbsw3/w3up/commit/5173d87b5fefa5c0421553b14703036a9e1cb861))
* **main:** release filecoin-api 4.6.1 ([#1363](https://github.com/tx-ravenxbsw3/w3up/issues/1363)) ([691fd9d](https://github.com/tx-ravenxbsw3/w3up/commit/691fd9d8fa7188910543ba024103594a10a0b91d))
* **main:** release filecoin-api 5.0.0 ([#1384](https://github.com/tx-ravenxbsw3/w3up/issues/1384)) ([e2b1b11](https://github.com/tx-ravenxbsw3/w3up/commit/e2b1b110550283c3c16e9abc0b3004c6f683d5d7))
* **main:** release filecoin-api 5.0.1 ([#1398](https://github.com/tx-ravenxbsw3/w3up/issues/1398)) ([8c4d8bd](https://github.com/tx-ravenxbsw3/w3up/commit/8c4d8bdd39168d1140282e09b12d95b551137dbe))
* **main:** release filecoin-api 6.0.0 ([#1414](https://github.com/tx-ravenxbsw3/w3up/issues/1414)) ([0f4abfe](https://github.com/tx-ravenxbsw3/w3up/commit/0f4abfe106dfcfda1af19718edfc54a170c31e5c))
* **main:** release filecoin-api 6.0.1 ([#1424](https://github.com/tx-ravenxbsw3/w3up/issues/1424)) ([3dd22e0](https://github.com/tx-ravenxbsw3/w3up/commit/3dd22e0527bbf385d777198c732ea1bedd1e289d))
* **main:** release filecoin-api 7.0.0 ([#1430](https://github.com/tx-ravenxbsw3/w3up/issues/1430)) ([540e0c0](https://github.com/tx-ravenxbsw3/w3up/commit/540e0c0b1ef2b5d852dc392fcfa8673de270a823))
* **main:** release filecoin-api 7.1.0 ([#1481](https://github.com/tx-ravenxbsw3/w3up/issues/1481)) ([f6a6ed8](https://github.com/tx-ravenxbsw3/w3up/commit/f6a6ed8fd1a89cefe17b05106acfa9e8c2ea1c4d))
* **main:** release filecoin-api 7.1.1 ([#1513](https://github.com/tx-ravenxbsw3/w3up/issues/1513)) ([828ca0f](https://github.com/tx-ravenxbsw3/w3up/commit/828ca0f7220dcdd350468e9f23530d6922e61366))
* **main:** release filecoin-api 7.2.0 ([#1522](https://github.com/tx-ravenxbsw3/w3up/issues/1522)) ([51c9c6b](https://github.com/tx-ravenxbsw3/w3up/commit/51c9c6b852c2869c2be2f9458af2a6033d304310))
* **main:** release filecoin-api 7.2.1 ([#1528](https://github.com/tx-ravenxbsw3/w3up/issues/1528)) ([7733351](https://github.com/tx-ravenxbsw3/w3up/commit/77333518ad2eacc70db977afa94243a7f44047ec))
* **main:** release filecoin-api 7.3.0 ([#1540](https://github.com/tx-ravenxbsw3/w3up/issues/1540)) ([d281277](https://github.com/tx-ravenxbsw3/w3up/commit/d281277d06fe9582926f840b4778c96c10dbf480))
* **main:** release filecoin-api 7.3.1 ([#1561](https://github.com/tx-ravenxbsw3/w3up/issues/1561)) ([f8d6667](https://github.com/tx-ravenxbsw3/w3up/commit/f8d66678be92c3a53c337ab0177fecffa409fc4e))
* **main:** release filecoin-api 7.3.2 ([#1567](https://github.com/tx-ravenxbsw3/w3up/issues/1567)) ([f5cbdba](https://github.com/tx-ravenxbsw3/w3up/commit/f5cbdba24b1fa62f685a8d20a2ba9c5d8e6c493e))
* **main:** release filecoin-api 8.0.0 ([#1580](https://github.com/tx-ravenxbsw3/w3up/issues/1580)) ([e7cda54](https://github.com/tx-ravenxbsw3/w3up/commit/e7cda54125fbabf79f7ba5865dde0221573e3ea9))
* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/tx-ravenxbsw3/w3up/issues/1577)) ([bdaa5e2](https://github.com/tx-ravenxbsw3/w3up/commit/bdaa5e297fef7e7ddca6a63c12ab071000cc7d2b))
* no longer depends on hd-scripts, packages use/configure eslint directly, fixes warnings from npm lint script ([#1058](https://github.com/tx-ravenxbsw3/w3up/issues/1058)) ([3a99cc0](https://github.com/tx-ravenxbsw3/w3up/commit/3a99cc02941f9d563cac1838e1e67a3faa42c3de))
* upgrade dependencies for better de-duplication ([#1620](https://github.com/tx-ravenxbsw3/w3up/issues/1620)) ([081120e](https://github.com/tx-ravenxbsw3/w3up/commit/081120e5ad823be84922ad863acf5e48618cb69b))

## [8.0.0](https://github.com/storacha/w3up/compare/filecoin-api-v7.3.2...filecoin-api-v8.0.0) (2024-12-09)


### ⚠ BREAKING CHANGES

* content serve authorization ([#1590](https://github.com/storacha/w3up/issues/1590))

### Features

* content serve authorization ([#1590](https://github.com/storacha/w3up/issues/1590)) ([8b553a5](https://github.com/storacha/w3up/commit/8b553a53253f55a3f0a2980557fa5c3b92427f3f))


### Other Changes

* **main:** release w3up-client 16.4.1 ([#1577](https://github.com/storacha/w3up/issues/1577)) ([1482d69](https://github.com/storacha/w3up/commit/1482d69c28baff1c27b1baf5f3e5c76f844e5576))

## [7.3.2](https://github.com/storacha/w3up/compare/filecoin-api-v7.3.1...filecoin-api-v7.3.2) (2024-10-20)


### Fixes

* configure max pieces ([#1566](https://github.com/storacha/w3up/issues/1566)) ([71674ed](https://github.com/storacha/w3up/commit/71674ed90022f499a144bcc201416e2568bd4d24))

## [7.3.1](https://github.com/storacha/w3up/compare/filecoin-api-v7.3.0...filecoin-api-v7.3.1) (2024-10-08)


### Fixes

* **filecoin-api:** parallel put to piece accept queue ([#1560](https://github.com/storacha/w3up/issues/1560)) ([e7cbb6d](https://github.com/storacha/w3up/commit/e7cbb6dc7930b7b19335286bf1908d2ed3cb9437))

## [7.3.0](https://github.com/storacha/w3up/compare/filecoin-api-v7.2.1...filecoin-api-v7.3.0) (2024-09-20)


### Features

* **filecoin-api:** allow custom hashing function to be passed to aggregate builder ([#1553](https://github.com/storacha/w3up/issues/1553)) ([e2653d4](https://github.com/storacha/w3up/commit/e2653d40c45070e2ccdc5cbda4eb4a35dab302e5))


### Fixes

* repo URLs ([#1550](https://github.com/storacha/w3up/issues/1550)) ([e02ddf3](https://github.com/storacha/w3up/commit/e02ddf3696553b03f8d2f7316de0a99a9303a60f))


### Other Changes

* Add `pnpm dev` to watch-build all packages ([#1533](https://github.com/storacha/w3up/issues/1533)) ([07970ef](https://github.com/storacha/w3up/commit/07970efd443149158ebbfb2c4e745b5007eb9407))

## [7.2.1](https://github.com/storacha-network/w3up/compare/filecoin-api-v7.2.0...filecoin-api-v7.2.1) (2024-07-29)


### Fixes

* use one-webcrypto from npm ([#1525](https://github.com/storacha-network/w3up/issues/1525)) ([9345c54](https://github.com/storacha-network/w3up/commit/9345c5415bc0b0d6ce8ccdbe92eb155b11835fd8))

## [7.2.0](https://github.com/storacha-network/w3up/compare/filecoin-api-v7.1.1...filecoin-api-v7.2.0) (2024-07-23)


### Features

* **filecoin-api:** paginated queries ([#1521](https://github.com/storacha-network/w3up/issues/1521)) ([25ed7d7](https://github.com/storacha-network/w3up/commit/25ed7d7e5208d85c49c18585adb5d8667b81f085))

## [7.1.1](https://github.com/storacha-network/w3up/compare/filecoin-api-v7.1.0...filecoin-api-v7.1.1) (2024-06-21)


### Fixes

* return piece accept receipt error ([#1512](https://github.com/storacha-network/w3up/issues/1512)) ([05283cf](https://github.com/storacha-network/w3up/commit/05283cfc8ace5e8716d6557a8e29402ef4a2e3c0))

## [7.1.0](https://github.com/w3s-project/w3up/compare/filecoin-api-v7.0.0...filecoin-api-v7.1.0) (2024-05-30)


### Features

* use digest in `blob/accept` location commitment ([#1480](https://github.com/w3s-project/w3up/issues/1480)) ([ade45eb](https://github.com/w3s-project/w3up/commit/ade45eb6f9b71f4bb4fcc771345ad21e966db730))


### Fixes

* rename blob and index client capabilities ([#1478](https://github.com/w3s-project/w3up/issues/1478)) ([17e3a31](https://github.com/w3s-project/w3up/commit/17e3a3161c6585b1844abcf7ed27252fa8580870))

## [7.0.0](https://github.com/w3s-project/w3up/compare/filecoin-api-v6.0.1...filecoin-api-v7.0.0) (2024-05-23)


### ⚠ BREAKING CHANGES

* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/w3s-project/w3up/issues/1444))

### Features

* add blob protocol to upload-client ([#1425](https://github.com/w3s-project/w3up/issues/1425)) ([49aef56](https://github.com/w3s-project/w3up/commit/49aef564a726d34dbbedbd83f5366d9320180f99))
* **upload-api:** integrate agent store for idempotence & invocation/receipt persistence  ([#1444](https://github.com/w3s-project/w3up/issues/1444)) ([c9bf33e](https://github.com/w3s-project/w3up/commit/c9bf33e5512397a654db933a5e6b5db0c7c22da5))


### Fixes

* check service did in w3filecoin ([#1476](https://github.com/w3s-project/w3up/issues/1476)) ([11b00bf](https://github.com/w3s-project/w3up/commit/11b00bf880dbbbc40b657d2417a4b13aa8c60a7d))


### Other Changes

* appease linter ([782c6d0](https://github.com/w3s-project/w3up/commit/782c6d0b3ca93ee801b38126339a262bcd713ede))

## [6.0.1](https://github.com/w3s-project/w3up/compare/filecoin-api-v6.0.0...filecoin-api-v6.0.1) (2024-04-30)


### Fixes

* filecoin test use blob ([#1422](https://github.com/w3s-project/w3up/issues/1422)) ([359c0b7](https://github.com/w3s-project/w3up/commit/359c0b736cad8e4375d75af4f60e97e20057e7aa))

## [6.0.0](https://github.com/w3s-project/w3up/compare/filecoin-api-v5.0.1...filecoin-api-v6.0.0) (2024-04-26)


### ⚠ BREAKING CHANGES

* dataStore in storefront renamed to contentStore

### Fixes

* storefront content store rename and separation for test ([#1409](https://github.com/w3s-project/w3up/issues/1409)) ([05e5db3](https://github.com/w3s-project/w3up/commit/05e5db35544c935a6c8e65e8f27583cffcf224e1))

## [5.0.1](https://github.com/w3s-project/w3up/compare/filecoin-api-v5.0.0...filecoin-api-v5.0.1) (2024-04-24)


### Fixes

* migrate repo ([#1389](https://github.com/w3s-project/w3up/issues/1389)) ([475a287](https://github.com/w3s-project/w3up/commit/475a28743ff9f7138b46dfe4227d3c80ed75a6a2))

## [5.0.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.6.1...filecoin-api-v5.0.0) (2024-04-23)


### ⚠ BREAKING CHANGES

* not possible to skip submit queue on storefront service anymore

### Fixes

* drop filecoin storefront skip submit queue option ([#1371](https://github.com/web3-storage/w3up/issues/1371)) ([1114383](https://github.com/web3-storage/w3up/commit/111438395dbd4530fade17b0d216ff056df7d832))

## [4.6.1](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.6.0...filecoin-api-v4.6.1) (2024-04-12)


### Fixes

* upgrade ucanto libs and format filecoin api ([#1359](https://github.com/web3-storage/w3up/issues/1359)) ([87ca098](https://github.com/web3-storage/w3up/commit/87ca098186fe204ff3409a2684719f1c54148c97))

## [4.6.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.5.0...filecoin-api-v4.6.0) (2024-03-26)


### Features

* api waits for trigger filecoin pipeline from the client ([#1332](https://github.com/web3-storage/w3up/issues/1332)) ([421bacb](https://github.com/web3-storage/w3up/commit/421bacb9bac8c251cb41f887144e953feaa5558f))

## [4.5.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.4.0...filecoin-api-v4.5.0) (2024-03-21)


### Features

* upgrade ucanto/transport to 9.1.0 in all packages to get more verbose errors from HTTP transport on non-ok response ([#1312](https://github.com/web3-storage/w3up/issues/1312)) ([d6978d7](https://github.com/web3-storage/w3up/commit/d6978d7ab299be76987c6533d18e6857f6998fe6))

## [4.4.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.3.1...filecoin-api-v4.4.0) (2024-02-06)


### Features

* add support to prepend pieces while buffering to aggregate ([#1301](https://github.com/web3-storage/w3up/issues/1301)) ([dff1846](https://github.com/web3-storage/w3up/commit/dff1846ad8b6ff5bb9e5fd8ff71f79df5bf79e4d))

## [4.3.1](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.3.0...filecoin-api-v4.3.1) (2024-01-15)


### Fixes

* avoid duplicates on aggregator buffer concat ([#1259](https://github.com/web3-storage/w3up/issues/1259)) ([9e64bab](https://github.com/web3-storage/w3up/commit/9e64babe93edeb474fc740d9be74c709d47bed1a))

## [4.3.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.2.0...filecoin-api-v4.3.0) (2023-11-29)


### Features

* move aggregate information out of deals in filecoin/info ([#1192](https://github.com/web3-storage/w3up/issues/1192)) ([18dc590](https://github.com/web3-storage/w3up/commit/18dc590ad50a023ef3094bfc1a2d729459e5d68e))

## [4.2.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.1.2...filecoin-api-v4.2.0) (2023-11-28)


### Features

* aggregator keeping oldest piece ts ([#1188](https://github.com/web3-storage/w3up/issues/1188)) ([97a7def](https://github.com/web3-storage/w3up/commit/97a7defa433b57591f23eddee692445437a718a1))


### Fixes

* package metadata ([#1161](https://github.com/web3-storage/w3up/issues/1161)) ([b8a1cc2](https://github.com/web3-storage/w3up/commit/b8a1cc2e125a91be582998bda295e1ae1caab087))
* storefront events cron with max concurrency ([#1191](https://github.com/web3-storage/w3up/issues/1191)) ([11010c9](https://github.com/web3-storage/w3up/commit/11010c94b9682e93b6209a169871021d37b76011))

## [4.1.2](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.1.1...filecoin-api-v4.1.2) (2023-11-16)


### Bug Fixes

* issue where typedoc docs would only show full docs for w3up-client ([#1141](https://github.com/web3-storage/w3up/issues/1141)) ([0b8d3f3](https://github.com/web3-storage/w3up/commit/0b8d3f3b52918b1b4d3b76ea6fea3fb0c837cd73))

## [4.1.1](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.1.0...filecoin-api-v4.1.1) (2023-11-15)


### Bug Fixes

* upgrade ucanto core ([#1127](https://github.com/web3-storage/w3up/issues/1127)) ([5ce4d22](https://github.com/web3-storage/w3up/commit/5ce4d2292d7e980da4a2ea0f1583f608a81157d2))

## [4.1.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.0.6...filecoin-api-v4.1.0) (2023-11-08)


### Features

* add usage/report capability ([#1079](https://github.com/web3-storage/w3up/issues/1079)) ([6418b4b](https://github.com/web3-storage/w3up/commit/6418b4b22329a118fb258928bd9a6a45ced5ce45))
* filecoin info ([#1091](https://github.com/web3-storage/w3up/issues/1091)) ([adb2442](https://github.com/web3-storage/w3up/commit/adb24424d1faf50daf2339b77c22fdd44faa236a))


### Bug Fixes

* lint ([#1095](https://github.com/web3-storage/w3up/issues/1095)) ([f9cc770](https://github.com/web3-storage/w3up/commit/f9cc77029d7c0651cb2961d08eca6f94dc1aef6c))

## [4.0.6](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.0.5...filecoin-api-v4.0.6) (2023-11-05)


### Bug Fixes

* revert enable storefront signer to be different from main service signer ([#1075](https://github.com/web3-storage/w3up/issues/1075)) ([80cdde0](https://github.com/web3-storage/w3up/commit/80cdde0f5b610cf6328dc17cb505759eddda821a))

## [4.0.5](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.0.4...filecoin-api-v4.0.5) (2023-11-04)


### Bug Fixes

* enable storefront signer to be different from main service signer ([#1072](https://github.com/web3-storage/w3up/issues/1072)) ([21ded3c](https://github.com/web3-storage/w3up/commit/21ded3c171ca66480e4f74329943527dcc2bac3e))

## [4.0.4](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.0.3...filecoin-api-v4.0.4) (2023-11-03)


### Bug Fixes

* dealer offer store keys without space ([#1066](https://github.com/web3-storage/w3up/issues/1066)) ([301f411](https://github.com/web3-storage/w3up/commit/301f411de74bca6b70c6b867c1bdc724a0a3af20))

## [4.0.3](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.0.2...filecoin-api-v4.0.3) (2023-11-03)


### Bug Fixes

* aggregate offer invocation cid wrong ([#1063](https://github.com/web3-storage/w3up/issues/1063)) ([90a5a4d](https://github.com/web3-storage/w3up/commit/90a5a4d815cff19d9421811a78dbefa01d486ebf))

## [4.0.2](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.0.1...filecoin-api-v4.0.2) (2023-11-03)


### Bug Fixes

* receipt chain has wrong CID because no expiration is set ([#1060](https://github.com/web3-storage/w3up/issues/1060)) ([dfb46d8](https://github.com/web3-storage/w3up/commit/dfb46d8185c684a18452e1325abcf74d59c48159))

## [4.0.1](https://github.com/web3-storage/w3up/compare/filecoin-api-v4.0.0...filecoin-api-v4.0.1) (2023-11-01)


### Bug Fixes

* storefront principal type on cron ([#1055](https://github.com/web3-storage/w3up/issues/1055)) ([3821804](https://github.com/web3-storage/w3up/commit/382180470add316dd48d01842f302e30edf870a0))

## [4.0.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v3.0.8...filecoin-api-v4.0.0) (2023-11-01)


### ⚠ BREAKING CHANGES

* add storefront filecoin api to upload api ([#1052](https://github.com/web3-storage/w3up/issues/1052))

### Features

* add storefront filecoin api to upload api ([#1052](https://github.com/web3-storage/w3up/issues/1052)) ([39916c2](https://github.com/web3-storage/w3up/commit/39916c25cbbfce6392fbb7cc71112987185c798c))

## [3.0.8](https://github.com/web3-storage/w3up/compare/filecoin-api-v3.0.7...filecoin-api-v3.0.8) (2023-10-31)


### Bug Fixes

* aggregator events inclusion record type simplified ([#1050](https://github.com/web3-storage/w3up/issues/1050)) ([2131eac](https://github.com/web3-storage/w3up/commit/2131eac64c5225508be41ca3cba5f924cb1e596a))

## [3.0.7](https://github.com/web3-storage/w3up/compare/filecoin-api-v3.0.6...filecoin-api-v3.0.7) (2023-10-31)


### Bug Fixes

* aggregator event tests ([#1048](https://github.com/web3-storage/w3up/issues/1048)) ([4263d12](https://github.com/web3-storage/w3up/commit/4263d12ad7eeb73ddd741752113c3babc93a3025))

## [3.0.6](https://github.com/web3-storage/w3up/compare/filecoin-api-v3.0.5...filecoin-api-v3.0.6) (2023-10-30)


### Bug Fixes

* dealer aggregate store query type does not need aggregate anymore ([#1042](https://github.com/web3-storage/w3up/issues/1042)) ([0b3c1d0](https://github.com/web3-storage/w3up/commit/0b3c1d0b891208d035abdb5bf7bf43dba853d8a7))

## [3.0.5](https://github.com/web3-storage/w3up/compare/filecoin-api-v3.0.4...filecoin-api-v3.0.5) (2023-10-30)


### Bug Fixes

* aggregate accept should rely on deal tracker response to issue receipt ([#1038](https://github.com/web3-storage/w3up/issues/1038)) ([42985ea](https://github.com/web3-storage/w3up/commit/42985ea526984dbc51d9afbdd1e1dc35a08c0639))
* aggregator service types have unused types ([#1039](https://github.com/web3-storage/w3up/issues/1039)) ([eba8e51](https://github.com/web3-storage/w3up/commit/eba8e514e90d266408b1271f438a339359206b1f))
* typo dealer event function name ([#1040](https://github.com/web3-storage/w3up/issues/1040)) ([7900624](https://github.com/web3-storage/w3up/commit/7900624469e3ec79f83adccd591e1c47a7034724))

## [3.0.4](https://github.com/web3-storage/w3up/compare/filecoin-api-v3.0.3...filecoin-api-v3.0.4) (2023-10-27)


### Bug Fixes

* filecoin api test service context explicit exported ([#1034](https://github.com/web3-storage/w3up/issues/1034)) ([aeceec8](https://github.com/web3-storage/w3up/commit/aeceec8007426db9104b67fd68b2eace23bde0c5))

## [3.0.3](https://github.com/web3-storage/w3up/compare/filecoin-api-v3.0.2...filecoin-api-v3.0.3) (2023-10-27)


### Bug Fixes

* trigger release filecoin api ([#1032](https://github.com/web3-storage/w3up/issues/1032)) ([7289a6b](https://github.com/web3-storage/w3up/commit/7289a6b2d735db76cd0159c5b7d9fc881ff0c903))

## [3.0.2](https://github.com/web3-storage/w3up/compare/filecoin-api-v3.0.1...filecoin-api-v3.0.2) (2023-10-26)


### Bug Fixes

* aggregate accept must query with aggregate only ([#1024](https://github.com/web3-storage/w3up/issues/1024)) ([6fd909c](https://github.com/web3-storage/w3up/commit/6fd909ccdc108a83b3ea122e2d66b0663c6f3484))

## [3.0.1](https://github.com/web3-storage/w3up/compare/filecoin-api-v3.0.0...filecoin-api-v3.0.1) (2023-10-26)


### Bug Fixes

* filecoin api store has returns false ([#1022](https://github.com/web3-storage/w3up/issues/1022)) ([1960130](https://github.com/web3-storage/w3up/commit/1960130d2e39135b6b2327c08a9dae3cce59b2c3))

## [3.0.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v2.0.3...filecoin-api-v3.0.0) (2023-10-26)


### ⚠ BREAKING CHANGES

* upgrade data segment v4 ([#996](https://github.com/web3-storage/w3up/issues/996))

### Bug Fixes

* upgrade data segment v4 ([#996](https://github.com/web3-storage/w3up/issues/996)) ([348e4b0](https://github.com/web3-storage/w3up/commit/348e4b065909e48ab1e97c0eaee9fa0b5ad2e223))

## [2.0.3](https://github.com/web3-storage/w3up/compare/filecoin-api-v2.0.2...filecoin-api-v2.0.3) (2023-10-25)


### Bug Fixes

* fix arethetypesworking errors in all packages ([#1004](https://github.com/web3-storage/w3up/issues/1004)) ([2e2936a](https://github.com/web3-storage/w3up/commit/2e2936a3831389dd13be5be5146a04e2b15553c5))

## [2.0.2](https://github.com/web3-storage/w3up/compare/filecoin-api-v2.0.1...filecoin-api-v2.0.2) (2023-10-24)


### Bug Fixes

* export tests in lib for events ([#1001](https://github.com/web3-storage/w3up/issues/1001)) ([e442f32](https://github.com/web3-storage/w3up/commit/e442f32ce09d1457bc1df6c96ad006ec082d428d))

## [2.0.1](https://github.com/web3-storage/w3up/compare/filecoin-api-v2.0.0...filecoin-api-v2.0.1) (2023-10-24)


### Bug Fixes

* import exports and types ([#998](https://github.com/web3-storage/w3up/issues/998)) ([844d938](https://github.com/web3-storage/w3up/commit/844d93837f0ac503f93533899f22984a7b293cd2))

## [2.0.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.4.4...filecoin-api-v2.0.0) (2023-10-24)


### ⚠ BREAKING CHANGES

* see latest specs https://github.com/web3-storage/specs/blob/cbdb706f18567900c5c24d7fb16ccbaf93d0d023/w3-filecoin.md

### Features

* upgrade to ucanto@9 ([#951](https://github.com/web3-storage/w3up/issues/951)) ([d72faf1](https://github.com/web3-storage/w3up/commit/d72faf1bb07dd11462ae6dff8ee0469f8ae7e9e7))


### Bug Fixes

* upgrade ucanto in filecoin api ([c95fb54](https://github.com/web3-storage/w3up/commit/c95fb54cdb04f50ff78e5113e70d73c1cd6d8b47))


### Code Refactoring

* filecoin api services events and tests ([#974](https://github.com/web3-storage/w3up/issues/974)) ([953537b](https://github.com/web3-storage/w3up/commit/953537bcb98d94b9e9655797a7f9026643ab949f))

## [1.4.4](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.4.3...filecoin-api-v1.4.4) (2023-09-06)


### Bug Fixes

* aggregator queue must send storefront in queue message ([#901](https://github.com/web3-storage/w3up/issues/901)) ([e5873fb](https://github.com/web3-storage/w3up/commit/e5873fb5b2f929c7493480b30c034344ad766b1a))

## [1.4.3](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.4.2...filecoin-api-v1.4.3) (2023-09-01)


### Bug Fixes

* dealer test ([#897](https://github.com/web3-storage/w3up/issues/897)) ([5ae5eac](https://github.com/web3-storage/w3up/commit/5ae5eacc47440c5749f85751d496198e17cdb8da))

## [1.4.2](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.4.1...filecoin-api-v1.4.2) (2023-09-01)


### Bug Fixes

* rename dealer offer store ([#895](https://github.com/web3-storage/w3up/issues/895)) ([d3f8e06](https://github.com/web3-storage/w3up/commit/d3f8e06590c5608420d61e20b98007076da0b6f7))

## [1.4.1](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.4.0...filecoin-api-v1.4.1) (2023-08-31)


### Bug Fixes

* extend queue add errors ([#890](https://github.com/web3-storage/w3up/issues/890)) ([0ecd4bb](https://github.com/web3-storage/w3up/commit/0ecd4bb8db5c7e296f62ec1d48ecece6bcb4a8d5))

## [1.4.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.3.1...filecoin-api-v1.4.0) (2023-08-30)


### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))


### Bug Fixes

* types when storefront is not in capability nb ([#886](https://github.com/web3-storage/w3up/issues/886)) ([448a7d1](https://github.com/web3-storage/w3up/commit/448a7d13ea3f90bc5ad6104a04c6d2f940b2817c))
* upgrade data segment ([#850](https://github.com/web3-storage/w3up/issues/850)) ([fba281f](https://github.com/web3-storage/w3up/commit/fba281f8cd3ce2a0a00ffd50a4a73d7701b489ce))
* w3filecoin spec separate capabilities to queue and enqueue ([#856](https://github.com/web3-storage/w3up/issues/856)) ([6bf9142](https://github.com/web3-storage/w3up/commit/6bf9142636fa65367faed8414c50beb9c1791726)), closes [#855](https://github.com/web3-storage/w3up/issues/855)

## [1.3.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.2.2...filecoin-api-v1.3.0) (2023-08-30)


### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))


### Bug Fixes

* upgrade data segment ([#850](https://github.com/web3-storage/w3up/issues/850)) ([fba281f](https://github.com/web3-storage/w3up/commit/fba281f8cd3ce2a0a00ffd50a4a73d7701b489ce))
* w3filecoin spec separate capabilities to queue and enqueue ([#856](https://github.com/web3-storage/w3up/issues/856)) ([6bf9142](https://github.com/web3-storage/w3up/commit/6bf9142636fa65367faed8414c50beb9c1791726)), closes [#855](https://github.com/web3-storage/w3up/issues/855)

## [1.2.1](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.2.0...filecoin-api-v1.2.1) (2023-08-30)


### Bug Fixes

* w3filecoin spec separate capabilities to queue and enqueue ([#856](https://github.com/web3-storage/w3up/issues/856)) ([6bf9142](https://github.com/web3-storage/w3up/commit/6bf9142636fa65367faed8414c50beb9c1791726)), closes [#855](https://github.com/web3-storage/w3up/issues/855)

## [1.2.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.1.0...filecoin-api-v1.2.0) (2023-08-10)


### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))


### Bug Fixes

* upgrade data segment ([#850](https://github.com/web3-storage/w3up/issues/850)) ([fba281f](https://github.com/web3-storage/w3up/commit/fba281f8cd3ce2a0a00ffd50a4a73d7701b489ce))

## 1.0.0 (2023-08-10)


### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))


### Bug Fixes

* upgrade data segment ([#850](https://github.com/web3-storage/w3up/issues/850)) ([fba281f](https://github.com/web3-storage/w3up/commit/fba281f8cd3ce2a0a00ffd50a4a73d7701b489ce))

## [1.1.0](https://github.com/web3-storage/w3up/compare/filecoin-api-v1.0.0...filecoin-api-v1.1.0) (2023-08-09)


### Features

* w3filecoin new client and api ([#848](https://github.com/web3-storage/w3up/issues/848)) ([7a58fbe](https://github.com/web3-storage/w3up/commit/7a58fbe8f6c6fbe98e700b7affd5825ddccf6547))
