Read-aloud voices for the game **somehow** (iOS app). The app downloads these files on first use, once per voice,
and checks every file against the SHA-256 below (pinned in the app's `src/game/voices.manifest.json`).

Voices: kokoro (en/es).

Sources:
- Kokoro-82M v1.0 by hexgrad, Apache 2.0, https://huggingface.co/hexgrad/Kokoro-82M; ONNX export by sherpa-onnx (k2-fsa),
  Apache 2.0, https://github.com/k2-fsa/sherpa-onnx/releases/tag/tts-models (kokoro-int8-multi-lang-v1_0). See LICENSE-Kokoro.txt, NOTICE.txt.
- ONNX Runtime Web 1.31.1 (MIT), https://www.npmjs.com/package/onnxruntime-web. See LICENSE-onnxruntime.txt.

Made reproducibly by `prototype/gm/tts/prepare_models.py` and `scripts/voices/make_release.py` in the game's repository.

| File | Bytes | SHA-256 |
|---|---|---|
| `kokoro.0.txt` | 15000000 | `84ad9ed2c469ea3c0c1072c1b365b6bf8870759198e3708a0b530810bc1eb387` |
| `kokoro.1.txt` | 15000000 | `28fdea4637c8a5e9390851bb55907a7ced98f4f4742916a35ec2b0775a20691e` |
| `kokoro.2.txt` | 15000000 | `e48c5a4f5441e17abf91b284b3def04c9f1e04d81c7caf64eca21f4dd9940669` |
| `kokoro.3.txt` | 15000000 | `98d07d4ed81ccf8d15815b77df1dd23e90915575794e324e38462d9cb53c2286` |
| `kokoro.4.txt` | 15000000 | `52ab092ce88fa76a5ff7dfb6df4ac69c27f858beed63d2312bbe9de65c2965e5` |
| `kokoro.5.txt` | 15000000 | `f4e64c7aba4a2503872b5ba4c116693b054b7201d966213e171b1734482ade3e` |
| `kokoro.6.txt` | 15000000 | `ca8944cbc9103a553e5b2dbaa4d71557a920be9852c2fd252f20160629a19ecb` |
| `kokoro.7.txt` | 13933996 | `57f687afea964c7271229932bb0682e6ea4e09422ea285c690d986e61aab55b0` |
| `kokoro-styles.0.txt` | 1278772 | `da8a0b85906cffd450c1ea84ede5a4073c4c939fef6058f17a4291c36ab6b029` |
| `ort.wasm.min.js` | 53796 | `b8a78c408c40da65fdc8ba0846f7b2948e92a4c6d6b23cc8e4165e428ad95443` |
| `ort-wasm-simd-threaded.mjs` | 24738 | `30ed0b5cd1182ede931fea448afb567d4dc705ec957af09f108a2be5f770dac3` |
| `ort-wasm-simd-threaded.wasm` | 14848852 | `4b884c203b0fa48d057be3332c65513ff85aa3c5bddd6946acc0fab7ecda001d` |
| `models.json` | 1492 | `fa54006d752b9eebe98635edce1f0db8ca50e6391a10c86fe6628b0225e54a01` |
