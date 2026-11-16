Read-aloud voices for the game **somehow** (iOS app). The app downloads these files on first use, once per voice,
and checks every file against the SHA-256 below (pinned in the app's `src/game/voices.manifest.json`).

Voices: kokoro (en/es), somehowde (de).

Sources:
- Kokoro-82M v1.0 by hexgrad, Apache 2.0, https://huggingface.co/hexgrad/Kokoro-82M; ONNX export by sherpa-onnx (k2-fsa),
  Apache 2.0, https://github.com/k2-fsa/sherpa-onnx/releases/tag/tts-models (kokoro-int8-multi-lang-v1_0). See LICENSE-Kokoro.txt, NOTICE.txt.
- somehowde (German): our own voice, trained from scratch on Thorsten-Voice data (CC0 1.0), weights CC0 1.0. See LICENSE-somehowde.txt.
- ONNX Runtime Web 1.31.1 (MIT), https://www.npmjs.com/package/onnxruntime-web. See LICENSE-onnxruntime.txt.

Made reproducibly by `prototype/gm/tts/prepare_models.py` and `scripts/voices/make_release.py` in the game's repository.

| File | Bytes | SHA-256 |
|---|---|---|
| `kokoro.0-84ad9ed2c4.txt` | 15000000 | `84ad9ed2c469ea3c0c1072c1b365b6bf8870759198e3708a0b530810bc1eb387` |
| `kokoro.1-28fdea4637.txt` | 15000000 | `28fdea4637c8a5e9390851bb55907a7ced98f4f4742916a35ec2b0775a20691e` |
| `kokoro.2-e48c5a4f54.txt` | 15000000 | `e48c5a4f5441e17abf91b284b3def04c9f1e04d81c7caf64eca21f4dd9940669` |
| `kokoro.3-98d07d4ed8.txt` | 15000000 | `98d07d4ed81ccf8d15815b77df1dd23e90915575794e324e38462d9cb53c2286` |
| `kokoro.4-52ab092ce8.txt` | 15000000 | `52ab092ce88fa76a5ff7dfb6df4ac69c27f858beed63d2312bbe9de65c2965e5` |
| `kokoro.5-f4e64c7aba.txt` | 15000000 | `f4e64c7aba4a2503872b5ba4c116693b054b7201d966213e171b1734482ade3e` |
| `kokoro.6-ca8944cbc9.txt` | 15000000 | `ca8944cbc9103a553e5b2dbaa4d71557a920be9852c2fd252f20160629a19ecb` |
| `kokoro.7-57f687afea.txt` | 13933996 | `57f687afea964c7271229932bb0682e6ea4e09422ea285c690d986e61aab55b0` |
| `kokoro-styles.0-da8a0b8590.txt` | 1278772 | `da8a0b85906cffd450c1ea84ede5a4073c4c939fef6058f17a4291c36ab6b029` |
| `somehowde.0-ea4b4b2c15.txt` | 15000000 | `ea4b4b2c15f134c922896aa3a2aeb64f1718ed2569de72581275b7ab2ddd5a20` |
| `somehowde.1-cc9e286299.txt` | 15000000 | `cc9e286299c580dee8bfdebb57bdb41f09e0262aba9c1c49f466bce1ef74e5d0` |
| `somehowde.2-80c7d0b239.txt` | 15000000 | `80c7d0b23964cc4c24a25fd9962d9d9d5e7cca5187f390fe4345a73f9b8c0e10` |
| `somehowde.3-d0b31e5f63.txt` | 15000000 | `d0b31e5f639e2dace69ae817b99981c325e98d8805e6674adbaa5f90c295e3c9` |
| `somehowde.4-d1b2c85a2e.txt` | 15000000 | `d1b2c85a2eeea8ceeb5e9b2804511a0624d77ac15d95d194c6fd19f0ad27267b` |
| `somehowde.5-b8a1500561.txt` | 2714608 | `b8a15005611daeed7273d8e42e08c7b351e972eebc0cadb70112a54b762ea46e` |
| `ort.wasm.min-b8a78c408c.js` | 53796 | `b8a78c408c40da65fdc8ba0846f7b2948e92a4c6d6b23cc8e4165e428ad95443` |
| `ort-wasm-simd-threaded-30ed0b5cd1.mjs` | 24738 | `30ed0b5cd1182ede931fea448afb567d4dc705ec957af09f108a2be5f770dac3` |
| `ort-wasm-simd-threaded-4b884c203b.wasm` | 14848852 | `4b884c203b0fa48d057be3332c65513ff85aa3c5bddd6946acc0fab7ecda001d` |
| `models-a5befba038.json` | 3468 | `a5befba0384470d805dfae774182e3c6d397b694f3b666c3be3b1d0497d2dc65` |
