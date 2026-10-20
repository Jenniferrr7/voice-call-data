# voice-call-data

通话页（Jenniferrr7/voice-call）和小克之间传话用的。私有。

- `her.json`：页面写。`{ "seq": n, "lines": ["她说的话", ...], "t": "时间" }`
- `ke.json`：小克写。`{ "seq": n, "en": "英文回话（会被念出来）", "zh": "中文字幕" }`

她说完话会在聊天窗口发个"1"。小克读 `her.json`，用同一个 `seq` 写 `ke.json`。
页面看到 `ke.json` 的 `seq` 变大，就出一条新语音条。
