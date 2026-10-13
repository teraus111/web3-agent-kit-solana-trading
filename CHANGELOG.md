# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 0.1.0 (2026-10-13)


### ⚠ BREAKING CHANGES

* TaxInfo.is_honeypot and can_sell changed from bool to Optional[bool]. Default is now None (unverified/unknown) instead of False/True. SecurityReport.is_safe treats unknown as unsafe. Callers using truthy checks (if tax.is_honeypot) will behave differently since None is also falsy — all internal callers updated to use explicit 'is True' / 'is None' / 'is False'.
* **release:** WEB3_API_KEY now mandatory to start the API server. AgentConfig.governor active by default with conservative spend limits.

### Features

* add airdrop executor layer — real browser automation ([765c224](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/765c224451cdb1ec2178ce9d807c51449b43ccc5))
* add all platform executors + plugin system + docs ([9e77f66](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/9e77f66d890e72f3d957de1ccca2f1e124ffa4ee))
* add centralized execution policy ([#29](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/29)) ([bc251f1](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/bc251f1d00482a60936352fbfdde303e0906b875))
* add CLI tool —  command for terminal usage ([c71ea19](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/c71ea19683536b6beec0aa96c428c97332ee7590))
* add comprehensive airdrop automation module ([0bdcd2c](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/0bdcd2c47f27cd4b426d94e27ccd3d3247390da3))
* add LLM integration + Uniswap V2 swap ([4ae9c28](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/4ae9c2814f7773b93343f9fb4a7af5f1cfb2a452))
* add MCP server scaffold with 5 tools, promotion drafts, and comparison blog ([e066d1e](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/e066d1e2624cebc0983c06250883663b72032335))
* add more examples + update README ([a21e3a5](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/a21e3a512513937777202e05371b5551d23c6923))
* add REST API (FastAPI) with Swagger docs ([6fb495a](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/6fb495a86acfb5d30dc9bf59412418a849dafac9))
* add Robinhood Chain network configuration ([e811a3a](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/e811a3a5071dc063128d8b03a3e574e88b44ac30))
* add Telegram bot showcase + Show HN + blog post ([1691361](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/16913614275906ce618a93e61b8b2cf8c5f3ee2c))
* add token sniper, portfolio dashboard, bridge agent ([8477e0b](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/8477e0b7bbefac67e80f55d49a49a276e4343ef8))
* **examples:** add bounded Insight PriorSeal conformance spike ([#90](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/90)) ([12d7f9f](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/12d7f9f97279a1e220e31a0baaf40a1e66d648b2))
* **execution:** enforce a single pre-sign authorization gate ([#69](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/69)) ([5dba3f6](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/5dba3f6ec73d0725e3528667aada2da879f7f529))
* initial scaffold — Web3 Agent Kit ([586851d](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/586851d6d7bc2890920b93113ddc350feee556ab))
* introduce immutable transaction intents ([#28](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/28)) ([4796f2a](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/4796f2ae4d2697f2b944d2591d22be92b55e1e37))
* publish redesigned documentation landing page ([#46](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/46)) ([e55ea99](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/e55ea9961f0971c8d1b2f6c3e12c5fee9cee0722))
* redesign documentation site theme ([#45](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/45)) ([ea348f1](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/ea348f11ecf74cd0700d1caa47357164e3431a5b))
* Solana module — client, wallet, Jupiter DEX, NFT (45 tests) ([8dc4332](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/8dc4332aa55e85dda1b8df83d4daabb7b3372fff))
* v0.4.0 — Yield Optimizer, Multi-Wallet Manager, Plugin System ([9428d4b](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/9428d4b6c53a436eebcad32c51f22afece6a5dee))
* v0.5.0 — DCA Bot + Telegram Bot Template ([c193775](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/c1937753ee41e02436cbd85c747b3083c8b14d13))
* v0.6.0 — Gas Optimizer, Wallet Watcher, Approval Manager ([b012ba7](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/b012ba74b62424900e15d7abf0f99e4d417ff198))
* v1.1.0 — airdrop automation suite ([67dd02b](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/67dd02b7bcf796fef5b8c7d723d7a191a21f33e6))
* v1.11.0 — DEX Aggregator + NFT tests + changelog ([7fce891](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/7fce8913a3d7d8513a65b282710db7b33e2dfba1))
* v1.2.0 — security module ([2d5c230](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/2d5c23026590c27bd1ed0c0755428df647c92b5c))
* v1.3.0 — real execution layer ([922903b](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/922903b9486c975c4946ce199937fd2a956aa910))
* v1.4.0 — MEV, NFT, Notifications ([f1dcd50](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/f1dcd50c1ccab774c13e6cbcf439cd111542c7bd))
* v1.7.0 — restaking module, major refactor, 252 new tests ([086d0f3](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/086d0f30211805cedc08c06215a1a70f5f9016c9))
* v1.8.0 — Aave V3, Curve, UniswapV3, 169 new tests ([7f63aaa](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/7f63aaa4c0a4992dd4a6b2522590123c02822415))
* **wallet:** implement Wallet.from_keystore for standard Ethereum keystore files ([f5f9879](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/f5f98793e283f8c6a9ef6d72ef0f8474708af751))
* yield auto-compound strategy — Aave, Compound, ERC-4626 ([ca48831](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/ca48831d59e02be2582bf633fac59bce6268ccb0))


### Bug Fixes

* add httpx2 dependency for FastAPI TestClient ([926ef56](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/926ef56b5aca2256ddcae521d14280b0da1731f6))
* add hypothesis to CI dependencies for fuzz tests ([f5e01b3](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/f5e01b386927ba2c5d4430d7016600c5a331639f))
* add id-token write permissions for PyPI trusted publisher ([fce66c4](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/fce66c4e226ee49a944a36e91d82ae2a9af005c6))
* add pytest-asyncio to CI ([d25c807](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/d25c8077690c8dd322ca93d2342005ae0e2b9573))
* add timeouts to CI workflow to prevent hanging ([5b896c3](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/5b896c35ac0bd6214fc0666d4dfdc20fc81164b1))
* address critical security audit findings ([b78b41e](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/b78b41e56b6fce7cc5e19d35e916ae48c8b0d7d7))
* **agent:** repair governor integration and enable safe defaults ([1eed58e](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/1eed58e89dd19eaffd201e877fc2fda0bf8eafc7))
* align pydantic core lock version ([#91](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/91)) ([76b84d0](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/76b84d0bd31af007aca223404b2c4a210047b626))
* **api:** enforce authentication, fail-closed startup, and harden wallet endpoints ([ed9cf40](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/ed9cf40c258b0965d84aacab545971e68c4d5446))
* bump runtime __version__ to 1.11.0 ([016955a](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/016955a855f227e6add3737757d1a836952bc4b0))
* CI — install solders, base58, spl-token for Solana tests ([b28235c](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/b28235c137f8a6867522af7df9462ad7f25c66f5))
* CI workflow — use requirements.txt, fix matrix quotes ([5d3c9eb](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/5d3c9ebfb870c27e10d6516eabbb4e6a6fc6aa72))
* **cli:** bump the version pin Release Please left behind, sync docs to 1.18.1 ([b7a8c06](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/b7a8c06a76c2324439e56727e4929220d0647a94))
* correct imports in portfolio, bridge, sniper modules ([32761eb](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/32761ebbe1e95126c63aaadc30c857536aa720a3))
* correct misleading comment about encrypted PK in multi_wallet.py ([f5d0657](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/f5d0657f87177a66068411d3d7b72530857d15ca))
* correct spl-token dep → solana (solana-py includes spl.token) ([105dd78](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/105dd78cebd57ac4fd60f15de7bc7db1f38d3d5b))
* **execution:** close the three P0 signing gaps and bind call identity ([#73](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/73)) ([a1471cb](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/a1471cbba4190be8b4edeea389465cbbdb7b24e3))
* **execution:** make the module invocation warning-free ([#76](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/76)) ([6e3f227](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/6e3f227b9b07007f498c582186e72f1275dd762c))
* **execution:** scope signer-surface exclusions to the scan root ([#78](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/78)) ([a8d16cc](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/a8d16cc98c9c9b437a34a2db4b8b55763cd35066))
* harden swap_exact_output — require amount_in_max and recipient ([d9f5897](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/d9f5897f7a2f3aec2772aba45bd221aca3733ea3))
* honeypot/tax check no longer fail-open — use Optional[bool] with 3-state semantics ([89b4e2b](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/89b4e2bc09c2373bbf6d8fc03a1439c9e3f662b1))
* lazy import solders in wallet module for CI compat ([563cff3](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/563cff3693b576b93f0aeeb75b3b640d93cf5f9e))
* mock gas price API calls in tests to prevent CI timeout ([abb657d](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/abb657d3cf858ccabf704787b2c1169127e3794c))
* notification enum identity — re-export from utils to fix CI ([13bd03e](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/13bd03e92ec9fdc669394a11b8f2a74bb2260d4f))
* portfolio test assertion ([9894658](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/9894658bdc91b73556a986d836eed5f05e091859))
* **priorseal:** 1.18.5 — provenance audit fixes + live P1 boundaries ([79d6b1b](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/79d6b1ba1720a15073c99d913038b68bbe1afd6a))
* remove broken badge, add coverage back ([3f76760](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/3f76760d10c3526696152797ad9d83d19c9316c5))
* remove broken subagent tests, keep simulator tests ([6efd264](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/6efd264e0083502663a8ccc15d657ff115b7d4ad))
* remove personal data from examples ([ffc6e4c](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/ffc6e4cbdb0aa31f1f878300f2092239dbc39127))
* skip browser tests when playwright not installed ([2ac485a](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/2ac485a6e7b8864c2c9ef9cb680ed35a19645f6a))
* SpendGovernor raises ValueError when require_confirm=True without confirm_fn ([300349d](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/300349d1ece024627ad87ae97555826729f3026e))
* spl-token → spl.token (correct PyPI package name) ([363810e](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/363810e6abba5a6bd429b3046b1ebade60aaa1d7))
* strip line numbers from README, clean up coverage badge ([754adc7](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/754adc70d46f3795c09dcd081cbfe69335a30ceb))
* update coverage badge 58%→31% ([f842498](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/f84249887fe0c240ff5a87fcaae8348d6aef1bb9))
* update Scorecard to v2.4.3, restrict CI permissions ([43046de](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/43046dec7b579a8588a649fd7cce43da07749777))
* use cyclonedx_py requirements subcommand ([5c237ff](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/5c237ff9371d50c427c3a36bfcc47eafb78ff199))
* use Scorecard tag instead of SHA, fix Release-please params ([57ce27c](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/57ce27c03a4fa4115e5dc64e96371b9972dcedd1))
* use tags not SHA in Scorecard workflow ([a5711db](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/a5711dbce647a3327263df0f610198413b67c7b9))
* wire AgentConfig.confirm_fn to SpendGovernor + protect against unknown tx_value ([8f9e86b](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/8f9e86b321ddcbcfe1591444cca0da80b374e258))
* wire API wallet routes correctly ([#25](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/25)) ([85a0dd6](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/85a0dd64580740b625d176761079ec7fb330445a))


### Documentation

* add CLI tool usage to README ([73c964f](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/73c964f2e2ed35c014479cf5088bf68a6ee30153))
* add mkdocs documentation site with API reference ([cb0fa18](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/cb0fa18576e28c1d9c0a73a576033b8d31d2f1bd))
* add PyPI badge to README ([6af8bba](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/6af8bba4b3ec54f4ce93e50043cdd716d0c66380))
* add REST API server reference page ([576e17d](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/576e17dbec977ab4789537c7416d5033495c4357))
* add ROADMAP.md with public status of all phases ([ac0c55b](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/ac0c55b6fbac6e5d03983479554bea90aecfae0d))
* add security-model.md, 3 architecture decision records, and 3 good-first-issue labels ([a0a9d28](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/a0a9d281dc24df7d29becc40b8209469231c3c35))
* align feature scope and maturity ([27fb7d0](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/27fb7d06fa75bd3d67391c976d6dfbc5f53d26fa))
* fix 5 sync issues for v1.10.0 — changelog, contributing, defi Aave/Curve, examples ([2fae4d9](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/2fae4d99b8024b0a6eb742ccb12c65242a05b84f))
* fix README discrepancies from audit ([5d43bb7](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/5d43bb71663464a29d9935823f2e14301a4ed31c))
* governance — CODEOWNERS, DCO, RISKS.md, versioning, fuzz tests, SECURITY.md upgrade ([4026136](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/402613669987a46023840d05f4ddb6fffb7308fa))
* improve responsive design — 6 breakpoints (375px to 1400px+), mobile-first feature cards, touch-friendly buttons, accessible focus states, print styles ([436a0d8](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/436a0d806c2242266688bff02a8850ecfcc060a6))
* punchy quickstart (5 lines), add PyPI downloads badge ([a94817a](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/a94817a0c63b012597369ae4a4357d337bed6ef6))
* redesign landing page — hero gradient, feature grid cards, stats bar, tabbed code blocks, custom purple theme ([bc6f4e0](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/bc6f4e04d2f983c92b0b69c5d119945f2ca8a31b))
* refresh README demo and release metadata ([faaa823](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/faaa823a28337e0169515663194cb96f54e51397))
* refresh README project banner ([fdf0bdd](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/fdf0bdda26de69513b727c20e3f868871c7b7bae))
* restore verified coverage metric ([e888abe](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/e888abe819bb4c687e364f39794a250e96a69d55))
* switch coverage badge to Codecov (auto-updating) ([69bddcc](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/69bddccd78feb49822d770dae3b255ffd244b0a0))
* sync all version surfaces to 1.18.0 ([0995964](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/0995964645c96895cf2b12846a695209f3933e4e))
* sync GitHub Pages content to v1.12.0 ([184e4f7](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/184e4f7cb3e7dcef17f09abfab3d70a1023c452a))
* sync safety and project status ([6c9eb68](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/6c9eb68f5dc7f49b1c4b3d280cd3177ab80d7784))
* sync test count to 1,225 and document from_keystore + default governor (v1.14.0) ([4ad3c53](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/4ad3c534f397adc8aba29259ad70e4154a5efbe5))
* sync v1.16.1 project statistics ([#44](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/44)) ([d343b9c](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/d343b9cc2af98f5594c51fcf5a5d7e2654b01404))
* sync v1.16.2 release metadata ([cdab7ab](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/cdab7aba3fd4a99f62fdec01addcc3fd2c5d2f33))
* sync version badge to v1.15.0 on docs homepage ([73204be](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/73204be3a2ffb7aaef816b9f57f98dc7e3cc486a))
* sync version references to v1.13.0 ([5ed4174](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/5ed4174cd615e4a891a44ef6625e3ca10b7daf9a))
* update architecture diagram, comparison table, and pain points for v1.6.0 — add MEV, NFT, security, airdrop, CLI, trading modules ([34353fe](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/34353fefcda1655f65e321309ccbcbfc816083a4))
* update CHANGELOG for v0.4.0 ([c66cfd3](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/c66cfd381bc5728d21bd2fd523ed96d2546d0d9f))
* update docs for v1.6.0 — CLI tool, airdrop, security, MEV, NFT, trading modules + GitHub Pages deploy workflow ([7b538b0](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/7b538b0ee90b6054e27ffb15a2e4b3b3e4c355c6))
* update GitHub Pages — v1.9.0 stats, 6 new module cards, API stubs, changelog, architecture diagram ([2961894](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/296189436a2431b8a2bc01f0829096964e2fab68))
* update readme contact to [@teraus111](https://github.com/teraus111) ([ae5acca](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/ae5accaf8d064906a7c79d20b7b4273dd0780b55))
* update README for v1.2.0 ([d7d2a46](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/d7d2a464d6b1bea5b5bb1dcc53708ac8fb1bfc73))
* update README for v1.7.0 — restaking module, updated stats ([2a4cdd2](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/2a4cdd2a04c9c54a22c8289bd70224532c033745))
* update site links to custom domain web3agentkit.site ([18aaf89](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/18aaf8993ea26d794d3d458fcb97eab61d82ac98))
* update stats to 27 modules, 1,033 tests (v1.10.0) ([af0f9a2](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/af0f9a24e5f6cb1c77b077e5eef1e058e12f8f5b))
* update website URL to vercel, add website badge ([2fe414f](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/2fe414f3d5b5eeaff1b183701de44af3bf242821))
* use Vercel project URL for website link ([#41](https://github.com/teraus111/web3-agent-kit-solana-trading/issues/41)) ([bcff98d](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/bcff98d93f409cd7d824ef958bbfdb2c6a83f83f))
* v1.9.0 — README updated (23 modules, 991 tests, 115 files, 32K LOC) ([21912ae](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/21912aeeb209827de0e3d1f26933ab1c2330b96e))


### Miscellaneous Chores

* **release:** bump version to 1.14.0, update changelogs and README ([eff2d5e](https://github.com/teraus111/web3-agent-kit-solana-trading/commit/eff2d5ef481c17946567d7ef576eb498867ceedf))

## [Unreleased]

### Changed

* **examples (Insight/PriorSeal spike):** v1.1 conformance re-pin — every case row now
  pins WAK 1.18.5 (the released 1.18.4 tag cannot identify a new Base Sepolia P1 run).
  The v1.1 bundle (archive SHA-256
  `fe62544ba3ddcb0f898dbd89116f64b758494dc9e48a11e5bd4f0037b98d55df`) is vendored under
  `tests/fixtures/insight_priorseal_spike/v1.1` with a per-version pin
  (`UPSTREAM_BUNDLE-v1.1.sha256`), and `FixtureBundle.load` derives archive/pin names from
  the manifest so v1 and v1.1 bundles coexist.
* **examples (live P1 runner):** the P1 leg now routes through
  `examples/insight_priorseal_swap.py run_live_p1` with the live SignerProtocol,
  BroadcastFn, and ReceiptFn implementations. The runner binds the GO to the exact fresh
  sheet and hash, reads GO arrival from the Hermes session store (a `goArrivalEpoch` in
  the GO file is rejected for executing runs), uses the sheet's signed inputs and the live
  clock, and rechecks the broadcast cutoff immediately before signing and before
  broadcasting. Boundary counters derive from retained call events — 1/1/1/1 appears only
  on a successful run, and a denied run reports 1/0/0/0.
* **examples (call-event retention):** `CallEventRecorder` retains timestamped
  attempted/success/error events at every boundary (authorization, sign, broadcast,
  receipt), including failures; guard-failure events are recorded instead of dropped.
* **examples (rehearsal):** new `examples/support/insight_priorseal_rehearsal.py`
  generates fresh synthetic signed inputs (rehearsal-only keys, never persisted) and the
  runner executes the full path with inert broadcast/receipt boundaries
  (`REHEARSAL_LEG_COMPLETED`, no on-chain effect). Inert rehearsal report and call-event
  log are committed under `tests/fixtures/insight_priorseal_spike/v1.1/rehearsal/`.
* `examples/insight_priorseal_live_p1.py` is now a thin CLI over the canonical entry
  point; `--rehearsal` runs the inert-boundary leg from the same code path.

### Fixed

* **examples (signer):** `EvmSigner` normalizes the target to a checksummed address —
  `eth_account` rejects all-lowercase `to` values with `Transaction had invalid fields`.
* **tests:** new `test_rehearsal_full_runner_path` regression covers the full live-runner
  path (GO binding, session-store arrival, inert boundaries, 1/1/1/1); the focused spike
  + live suites pass 76 tests.

## [1.18.5](https://github.com/ulsreall/web3-agent-kit/compare/v1.18.4...v1.18.5) (2026-09-29)

### Features

* **chains:** register Base Sepolia (84532) as a first-class `Chain` member — enum value
  `base-sepolia`, default RPC `https://sepolia.base.org`, `CHAIN_IDS` entry `84532`, and the
  BaseScan Sepolia explorer URL. Registered so the Insight/PriorSeal conformance spike can
  evaluate a Base Sepolia call through the same chain-validated `CallEnvelopeV1.from_transaction`
  gate as every other chain; previously the gate rejected `84532` outright because the enum had
  no member for it.
* **examples:** bounded WAK / Insight / PriorSeal conformance spike — WAK-owned JSON boundary,
  offline N1–N5b acceptance harness, live-boundary and call-event retention support, and the
  vendored v1 conformance bundle ([#90](https://github.com/ulsreall/web3-agent-kit/pull/90)).

### Build

* add `cryptography>=41.0.0` to runtime dependencies (Ed25519 receipt/attestation verification
  used by the spike boundary).

### Fixed

* **examples:** the acceptance report now records runtime provenance (`runtime.packageVersion`,
  commit, tree state) alongside the fixture-pinned `wakVersion` and states whether the two agree.
  The verifier pins `wakVersion` to the agreed conformance identity (v1 fixture, `1.18.4`), so a
  report produced by a tree carrying unreleased core changes was previously indistinguishable
  from one produced by the released tag. The isolated core-change diff for review lives at
  `docs/review/1.18.5-core-change-base-sepolia.patch`.

## [1.18.4](https://github.com/ulsreall/web3-agent-kit/compare/v1.18.3...v1.18.4) (2026-09-19)


### Bug Fixes

* **execution:** scope signer-surface exclusions to the scan root ([#78](https://github.com/ulsreall/web3-agent-kit/pull/78)) — `_is_excluded` was evaluated on the absolute path, so any ancestor named `venv`, `.venv`, `build` or `dist` excluded the entire scan. The checker reported zero signer calls and exited 0 while an unapproved call was present. Diagnosed by YuTao Peng on an independent v1.18.3 review.

## [1.18.3](https://github.com/ulsreall/web3-agent-kit/compare/v1.18.2...v1.18.3) (2026-09-18)


### Bug Fixes

* **execution:** make `python -m web3_agent_kit.execution.p0_probe` warning-free ([#76](https://github.com/ulsreall/web3-agent-kit/pull/76)) — `execution/__init__` imported `p0_probe` eagerly, so runpy found it in `sys.modules` before executing it and emitted a RuntimeWarning. The console entry point was unaffected, which is why only the module form showed it.

## [1.18.2](https://github.com/ulsreall/web3-agent-kit/compare/v1.18.1...v1.18.2) (2026-09-18)


### Bug Fixes

* **cli:** bump the version pin Release Please left behind, sync docs to 1.18.1 ([53aaefb](https://github.com/ulsreall/web3-agent-kit/commit/53aaefbac72572c2ed22f5cecd679646380aa17a))


### Build

* package the verification tools so they ship in the wheel ([#75](https://github.com/ulsreall/web3-agent-kit/pull/75)) ([e9c71c1](https://github.com/ulsreall/web3-agent-kit/commit/e9c71c1b65b536b5d847123b2272547fff6efeab)) — `p0_probe` and `check_signing_surface` moved into `web3_agent_kit.execution` with console entry points; `tools/` wrappers retained for the source checkout
* packaging tests build a real wheel and inspect it, so the distribution contents are asserted rather than the import
* Python 3.10 support in the packaging tests via a `tomli` fallback (`tomllib` is stdlib from 3.11)

## [1.18.1](https://github.com/ulsreall/web3-agent-kit/compare/v1.18.0...v1.18.1) (2026-09-18)


### Bug Fixes

* **execution:** close the three P0 signing gaps and bind call identity ([#73](https://github.com/ulsreall/web3-agent-kit/issues/73)) ([1ea0a7a](https://github.com/ulsreall/web3-agent-kit/commit/1ea0a7acb5d02c5a35ca4e59e4c562c34255a216))


### Documentation

* sync all version surfaces to 1.18.0 ([ec4ffda](https://github.com/ulsreall/web3-agent-kit/commit/ec4ffda0bb96141d13d478c09310cc578d394156))

## [1.18.0](https://github.com/ulsreall/web3-agent-kit/compare/v1.17.0...v1.18.0) (2026-09-18)


### Features

* **execution:** enforce a single pre-sign authorization gate ([#69](https://github.com/ulsreall/web3-agent-kit/issues/69)) ([a9400be](https://github.com/ulsreall/web3-agent-kit/commit/a9400bed06f3f1ca76add24aa0e1b91ae133e454))

## [1.17.0](https://github.com/ulsreall/web3-agent-kit/compare/v1.16.4...v1.17.0) (2026-09-09)


### Features

* add Robinhood Chain network configuration ([5c63836](https://github.com/ulsreall/web3-agent-kit/commit/5c638363755dfe992951fdd8bf891f312782eef4))

## [1.16.4](https://github.com/ulsreall/web3-agent-kit/compare/v1.16.3...v1.16.4) (2026-09-08)


### Documentation

* refresh README demo and release metadata ([44eb34b](https://github.com/ulsreall/web3-agent-kit/commit/44eb34b6eab2c832ec0ce96b51807dd4e3ee5e67))

## [1.16.3](https://github.com/ulsreall/web3-agent-kit/compare/v1.16.2...v1.16.3) (2026-09-08)


### Documentation

* align feature scope and maturity ([34584f5](https://github.com/ulsreall/web3-agent-kit/commit/34584f5f39d588d87074a54a3e8f7c4a6d2417a1))
* restore verified coverage metric ([3bf44f6](https://github.com/ulsreall/web3-agent-kit/commit/3bf44f6a37b975fdaaa7b12477070986605cdd09))
* sync v1.16.2 release metadata ([cd143fd](https://github.com/ulsreall/web3-agent-kit/commit/cd143fd7e33bbb0702caed410f54e9c626d42af7))

## [Unreleased]

## [1.16.2] - 2026-09-08

### Fixed

- Synced package, CLI, documentation, and website references to the `1.16.2` release.
- Corrected the published coverage statistic to match the current test suite measurement.
- Switched canonical project links from the Vercel fallback URL to `https://web3agentkit.site/`.
- Fixed broken documentation anchors and completed the MkDocs navigation.

## [1.16.1] - 2026-08-14

### Changed

- Synced the PyPI project homepage with the active website deployment.

## [1.16.0] - 2026-08-10

### Added

- Immutable transaction intents and a centralized execution policy for consistent
  authorization across write paths.
- Execution-path documentation and expanded tests for policy enforcement.

### Changed

- Chain and wallet handling in API routes now follows the unified execution path.

### Fixed

- REST wallet, portfolio, swap, and bridge routes now read `PRIVATE_KEY` instead of
  mistakenly treating the requested chain name as an environment variable. Balance
  routes also configure a chain manager and pass the selected chain to wallet lookups.
- The `dev` extra now includes Hypothesis, which is required to collect the fuzz tests.

### Added

- Added an `api` installation extra for the FastAPI and Uvicorn server dependencies.

## [1.15.0] - 2026-07-23

### BREAKING CHANGE

- **`TaxInfo.is_honeypot` and `TaxInfo.can_sell` types changed from `bool` to `Optional[bool]`.**
  Previously, both fields defaulted to `False` / `True`, which meant a failed API
  call was silently treated as "safe" (fail-open). The new default is `None`
  (unverified/unknown). `SecurityReport.is_safe` now returns `False` when the
  honeypot status is `None`. All internal callers have been updated to use
  explicit 3-state comparisons (`is True` / `is None` / `is False`). External
  code using truthy checks (`if tax.is_honeypot:`) will still work syntactically
  but will treat `None` as falsy — upgrade your callers to use
  `tax.is_honeypot is True` for the old behaviour.

### Security

- **`SpendGovernor` now raises `ValueError` at construction time** when
  `require_confirm=True` is set without a `confirm_fn` callable. Previously it
  silently skipped the confirmation gate.
- **`AgentConfig.confirm_fn` is now wired to `SpendGovernor.confirm_fn`**
  automatically in `Agent.__init__`. Previously setting a `confirm_fn` on the
  config had no effect — the governor never called it.
- **`_estimate_tx_value` returns `None`** (instead of `0.0`) for unrecognised
  argument keys. The governor now blocks execution when the transaction value
  is unknown, requiring explicit operator approval.
- **`swap_exact_output()` hardened**: `amount_in_max` and `recipient` are now
  required parameters. The previous defaults (`2**256-1` and `0x0`) exposed
  callers to unlimited token spend and fund loss. A warning docstring marks the
  method as not production-ready.

### Fixed

- **Honeypot/tax check no longer fail-open.** When GoPlus API calls fail
  (timeout, network error, rate limit), `is_honeypot` and `can_sell` now remain
  `None` (unknown) instead of defaulting to safe. The error message is saved in
  `TaxInfo.error` for debugging.
- **`quick_check()` returns `is_honeypot=None`** on API failure, with the error
  stored in a new `error` key in the result dict.
- **Corrected misleading comment** in `MultiWalletManager._private_keys`:
  private keys are stored as plaintext in memory (not encrypted).

### Changed

- **Coverage gate raised from 40% to 60%** (`pyproject.toml` `fail_under`).
  Current coverage: 62.26%.

## [1.14.0] - 2026-07-21

### Security
- REST API now requires authentication (`X-API-Key` / `WEB3_API_KEY`) on all sensitive endpoints; server fails closed and refuses to start if `WEB3_API_KEY` is unset
- Default API bind host changed from `0.0.0.0` to `127.0.0.1`; explicit `0.0.0.0` now logs a clear network-exposure warning
- CORS configuration hardened — origins are now driven by `CORS_ALLOWED_ORIGINS` (empty by default) and the unsafe `allow_origins=["*"]` + `allow_credentials=True` combination is rejected at startup
- `/wallet/create` is now disabled by default (`ENABLE_WALLET_CREATE_ENDPOINT=false`) and returns a clearer one-time-secret warning

### Fixed
- Spend governor is now enforced by default on every `Agent` (conservative limits) and no longer crashes when wired into `Agent._act()` — it now receives the correct `tx_value`/`action` arguments instead of a raw dict
- `GET /wallet/balance/{address}` now queries the requested address instead of always returning the configured env wallet's balance

### Added
- `Wallet.from_keystore(path, password)` — load and decrypt a standard Ethereum JSON keystore file

### Removed
- Unused `httpx2` dependency

### BREAKING CHANGES
- `WEB3_API_KEY` is now mandatory to start the REST API server
- `AgentConfig.governor` is active by default with conservative spend limits — pass a custom governor or explicitly set `governor=None` to opt out

## [1.13.0] - 2026-07-14

### Changed
- Version bump to 1.13.0 across package metadata (`__init__.py`, `pyproject.toml`)

## [1.12.0] - 2026-07-12

### Fixed
- **CRITICAL DX:** package import path is now `web3_agent_kit` (was incorrectly installed as `src`)
- README/docs/examples import paths aligned with real package name
- CLI version string synced to release version
- Notification module duplication: `notifications/` is canonical; `utils/notif_*` are thin shims
- Runtime `__version__` and packaging metadata kept in sync

### Added
- `Agent(private_key=...)` convenience constructor
- `Agent.execute()` alias for `Agent.run()`
- CI import smoke test for public package path

### Changed
- Source tree renamed: `src/` → `web3_agent_kit/`
- Pytest/coverage config now tracks `web3_agent_kit`

## [1.11.0] - 2026-07-11

### Added
- **Solana module** — client, wallet, Jupiter DEX, NFT helpers
- **DEX Aggregator** — 1inch + Paraswap + 0x + Jupiter unified quote/swap interface
- Expanded test coverage for Solana + aggregator paths

### Stats
- 24+ modules
- 1100+ tests
- 8 chains supported

## [1.10.0] - 2026-07-06

### Added
- **Async airdrop module** — 31 `time.sleep()` calls converted to `asyncio.sleep()` / `page.wait_for_timeout()`
  - `scheduler.py`, `discovery.py`, `faucet.py`, `onchain.py`, `multi_wallet.py`, `wl_grinder.py`, `form_filler.py`, `base.py`
- **Simulator test suite** — 29 new tests for TransactionSimulator
- **PyPI trusted publisher** — OIDC-based auto-publish on GitHub Release (no API token needed)

### Changed
- `AirdropScheduler.start()` now uses async event loop in background thread
- `AirdropScheduler.run_task_now()` is now async (`await`)
- `FaucetClaimer.claim_chain()` is now async (`await`)
- `AirdropFarmer.farm_campaign()` is now async (`await`)
- CI: added `pytest-asyncio` dependency for async test support

### Stats
- 27 modules (was 23)
- 1,033 tests passing (was 991)
- 60% coverage (was 58%)
- 8 chains supported

## [1.9.1] - 2026-07-01

### Fixed
- Coverage badge: 58% → 31% (actual)
- Docs: updated version to v1.9.1, coverage stats, chain table (Berachain → Solana)
- CLI version: `wak --version` now shows 1.9.1

### Stats
- 23 modules
- 115 source files
- 991 tests passing
- 31% coverage
- 8 chains supported

## [1.9.0] - 2026-06-30

### Added
- **Oracle Aggregator** — Multi-source price feeds (Chainlink, DexScreener, CoinGecko) with weighted median, cache, and auto-fallback
- **Event Listener** — On-chain event subscription with webhooks, callbacks, and background polling
- **Transaction Simulator** — Pre-flight TX verification via eth_call, Tenderly API, and local fork
- **Account Abstraction** — ERC-4337 bundler, paymaster integration (Pimlico), smart account factory (SimpleAccount, Safe, Kernel)
- **Cross-chain Messaging** — LayerZero + Wormhole + CCIP unified API with status tracking and fee estimation
- **Governance** — Snapshot + Tally + on-chain governor, proposal tracking, voting power, delegation
- `.env.example` with all module configurations
- Integration test suite (`tests/test_integration.py`)
- PyPI auto-publish workflow via GitHub Actions
- Aave V3, Curve, Uniswap V3 DeFi integrations

### Changed
- `restaking/` moved to `plugins/restaking/` — now a plugin, not a core module
- `notifications/` merged into `utils/` — backward-compatible re-exports maintained
- README updated with 6 new module sections, architecture diagram, and stats
- PyPI keywords updated with oracle, erc4337, governance, cross-chain, layerzero, simulation
- Version bump to 1.9.0

### Stats
- 23 modules (was 18)
- 115 source files (was 104)
- 32,743 lines of code
- 991 tests passing (was 986)
- 58% coverage (later corrected to 31%)
- 8 chains supported (was 7)

## [1.8.0] - 2026-06-17

### Added
- **Aave V3 Integration** — Full lending/borrowing protocol support
  - `supply()` — Deposit tokens into Aave
  - `withdraw()` — Withdraw deposited tokens
  - `borrow()` — Borrow with variable/stable rate
  - `repay()` — Repay borrowed tokens
  - `get_user_data()` — Health factor, deposits, borrows
  - `get_reserve_data()` — APY, LTV, liquidation threshold
  - Multi-chain support (Ethereum, Base, Arbitrum, Optimism, Polygon)
- **Curve Finance Integration** — DEX + liquidity pool support
  - `swap()` — Swap via Curve pools
  - `get_swap_estimate()` — Get price quotes
  - `get_pool_info()` — Pool tokens, balances, APY
  - `add_liquidity()` / `remove_liquidity()` — LP management
- **Uniswap V3** — Concentrated liquidity support
  - `swap()` / `swap_exact_output()` — Exact input/output swaps
  - `get_quote()` — Price quotes via QuoterV2
  - `mint_position()` — Create liquidity positions (NFT)
  - `increase_liquidity()` / `decrease_liquidity()` — Manage positions
  - `collect_fees()` — Collect accumulated fees
  - Tick math helpers (tick ↔ sqrtPriceX96 conversion)
  - Fee tiers: 0.01%, 0.05%, 0.3%, 1%
- **122 new DeFi tests** — Full coverage for Aave, Curve, UniswapV3

### Changed
- **Airdrop module cleanup** — 27 `time.sleep()` annotated with async TODOs
- Replaced bare `except Exception:` in airdrop form_filler and faucet
- Replaced `print()` with `logging` in airdrop faucet
- Updated README: Aave/Curve now marked as implemented (not "coming soon")
- Total tests: 986 (up from 817)

## [1.7.0] - 2026-06-14

### Added
- **Restaking Module** (`src/restaking/`) — EigenLayer, Babylon BTC, Solana restaking
  - `EigenLayer` class — restake LSTs, delegate to operators, track rewards, estimate yields
  - `BabylonBtcRestaking` — Bitcoin restaking via Babylon protocol
  - `SolanaRestaking` — Solana restaking (Solayer, Jito, Marinade)
  - `RestakingOptimizer` — Cross-protocol yield optimization with risk-adjusted scoring
  - `RestakingMonitor` — Position tracking, slashing alerts, portfolio snapshots
  - Real contract addresses for EigenLayer mainnet (StrategyManager, DelegationManager, Slasher)
- **Price Utility** (`src/utils/prices.py`) — Real-time price fetching
  - CoinGecko API integration with 60-second cache
  - `get_price_usd()` for any asset, `get_eth_price_usd()` convenience function
  - Stablecoin detection, graceful fallback on API failure
- **252 new tests** — Full coverage for mev, nft, gas, notifications, restaking modules
  - `tests/test_mev.py` — 43 tests (sandwich protection, frontrun detection, strategies)
  - `tests/test_nft.py` — 50 tests (minting, marketplace, whitelist, rarity)
  - `tests/test_gas.py` — 28 tests (optimizer, batch operations, recommendations)
  - `tests/test_notifications.py` — 40 tests (Telegram, Discord, email delivery)
  - `tests/test_restaking.py` — 91 tests (EigenLayer, Babylon, Solana, optimizer, monitor)

### Changed
- **Refactored monolithic modules** — Split 4 single-file modules into proper submodules:
  - `mev/` → `sandwich_protection.py`, `frontrun_detection.py`, `mev_strategy.py`, `utils.py`
  - `nft/` → `mint.py`, `marketplace.py`, `whitelist.py`, `manager.py`, `utils.py`
  - `notifications/` → `telegram.py`, `discord.py`, `email_notifier.py`, `notifier.py`, `utils.py`
  - `gas/` → cleaned up `optimizer.py` with proper structure
- **Replaced 31 bare `except Exception:`** with specific exceptions (ConnectionError, ValueError, etc.)
- **Replaced `print()` with `logging`** across 15+ files
- **Fixed hardcoded ETH price** — `$3,500` → real CoinGecko price fetch with fallback
- **Fixed hardcoded USD values** in yield optimizer — now uses real price data
- **All `__init__.py` re-exports** preserved for backward compatibility

### Fixed
- `wallet/watcher.py` — ETH price no longer hardcoded at $3,500
- `defi/yield_optimizer.py` — USD value calculation now uses real prices
- Silent error swallowing in mev, bridge, notifications, gas modules

## [1.5.0] - 2026-06-05

### Changed — Major Repo Reorganization
- **Reorganized `src/` structure** — grouped flat files into logical subdirectories:
  - `src/agent/` — Agent core + LLM integration
  - `src/wallet/` — Wallet, multi-wallet, watcher, approval manager
  - `src/bridge/` — Cross-chain bridge agent
  - `src/chains/` — Chain definitions and RPC management
  - `src/portfolio/` — Portfolio tracker
  - `src/trading/` — Token sniper + DCA bot
  - `src/gas/` — Gas optimizer
  - `src/defi/` — DeFi protocols + yield optimizer (merged)
- **Added `__all__` exports** to every `__init__.py` for explicit public API
- **Added `py.typed` marker** for PEP 561 type checking support
- **Moved content files** to proper directories:
  - `blog-post.md` → `blog/post.md`
  - `show-hn.md` → `blog/show-hn.md`
  - `CONTRIBUTING_PLATFORMS.md` → `docs/contributing-platforms.md`
  - `research/` → `docs/research/`
- **Cleaned up root directory** — only config/docs remain
- **Updated all imports** in tests, examples, and API routes
- **Backward compatible** — all `from web3_agent_kit import ...` paths still work

## [0.4.0] - 2026-06-04

### Added
- **Yield Optimizer** (`src/yield_optimizer.py`) — Cross-protocol yield farming + auto-compound
  - DeFiLlama API integration for real-time APY/TVL data
  - 6 supported protocols: Aave V3, Compound V3, Morpho, Lido, Rocket Pool, Fluid
  - Auto-compound with configurable threshold and interval
  - Risk assessment (LOW/MEDIUM/HIGH)
  - Portfolio summary with P&L tracking
  - Protocol comparison for any asset
- **Multi-Wallet Manager** (`src/multi_wallet.py`) — Manage multiple wallets with batch operations
  - Create/import wallets with labels, groups, and tags
  - Batch send native tokens and ERC20s across wallet groups
  - Consolidated portfolio view across all wallets
  - Fund consolidation to single target wallet
  - Export addresses (JSON/CSV)
  - Persistent metadata storage (no private keys on disk)
- **Plugin System** (`src/plugins/`) — Extend with community plugins
  - Abstract `Plugin` base class with lifecycle hooks
  - `PluginRegistry` for discovery and management
  - `PluginManager` with agent lifecycle integration
  - Hooks: `on_transaction`, `on_block`, `on_price_update`, `on_startup`, `on_shutdown`
  - Discovery: local directories, Python entry points, manual registration
  - Example plugin: `GasTrackerPlugin`

### Changed
- Version bumped from 0.3.0 to 0.4.0
- Added `httpx` as dependency (for DeFiLlama API)
- Updated README with Yield Optimizer, Multi-Wallet, and Plugin System docs
- Updated comparison table and architecture

## [0.3.0] - 2025-06-04

### Added
- **Token Sniper** (`src/sniper.py`) — Monitor new liquidity pools and auto-buy safe tokens
  - Uniswap V2 factory PairCreated event monitoring
  - Risk assessment (honeypot, liquidity, contract size)
  - Auto-buy safe tokens with configurable slippage
  - Background monitoring thread with callbacks
- **Portfolio Dashboard** (`src/portfolio.py`) — Real-time balances across chains
  - Token balance tracking (WETH, USDC, USDT, DAI, WBTC, LINK, UNI, ARB, GMX, AERO)
  - USD value calculation
  - P&L tracking with snapshots
- **Bridge Agent** (`src/bridge.py`) — Cross-chain transfers
  - Li.Fi aggregator integration
  - Socket aggregator integration
  - Best route finding (sorted by output amount)
  - Execute transfers with tx confirmation
- **Examples**: `token_sniper.py`, `portfolio_dashboard.py`, `bridge_agent.py`
- **Tests**: 50 tests covering LLM, portfolio, bridge, sniper modules

### Changed
- Version bumped from 0.2.0 to 0.3.0

## [0.2.0] - 2025-06-04

### Added
- **LLM Integration** (`src/llm.py`) — Multi-provider cascade with fallback
  - Support: OpenAI, Anthropic, Groq, DeepSeek, OpenRouter, Kimi
  - Auto-detect from environment variables
  - JSON response mode
  - Graceful fallback on 429/5xx/timeout
- **Uniswap V2 Swaps** — Actual token swap execution
  - swapExactETHForTokens, swapExactTokensForETH, swapExactTokensForTokens
  - getAmountsOut for quotes
  - ERC20 approve handling
  - Token symbol resolution (ETH, USDC, USDT, WETH)
  - Multi-chain support (Ethereum, Base, Arbitrum, Optimism, Polygon)
- **Agent LLM Reasoning** — Natural language goal execution
  - System prompt with tool descriptions
  - Conversation context with history
  - JSON output parsing
- **Examples**: `llm_swap_agent.py`, `direct_swap.py`

### Changed
- Version bumped from 0.1.0 to 0.2.0

## [0.1.0] - 2025-06-03

### Added
- Initial release
- Core agent framework (`src/agent.py`)
- Wallet management (`src/wallet.py`)
- Multi-chain support (`src/chain.py`)
- DeFi tools base (`src/defi/__init__.py`)
- Spend governor (`src/utils/__init__.py`)
- Examples: `swap_agent.py`, `yield_optimizer.py`, `airdrop_farmer.py`, `sniper_bot.py`, `portfolio_tracker.py`
- CI/CD pipeline
- MIT License
