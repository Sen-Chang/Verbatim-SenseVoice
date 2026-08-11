# Verbatim-SenseVoice
Verbatim 是一個語音轉成文字的 windows APP, https://github.com/GalaxyRuler/Verbatim<br>
SenseVoice 是一個語音模型 https://github.com/QwenAudio/SenseVoice<br>
這個 Repository 是爲了讓 SenseVoice 輸出繁體中文.

安裝  Verbatim  後, 可以選擇模型來辨認, SenseVoicee 是其中一個. 但因爲 token 是簡體中文, 所以所有的輸出都是簡體字. 這個 Repository 的檔案是把 token 轉成繁體並重新 hash. 只需將這兩個檔案 .verbatim-integrity.json 和 tokens.txt 覆蓋在 Verbatim/Data/models/sense-voice-int8 既能將語音辨識輸出的簡體中文替換成繁體中文.

測試的版本 Verbatim v0.14.2

Verbatim is a Windows app that converts speech to text. https://github.com/GalaxyRuler/Verbatim<br>
SenseVoice is a speech recognition model. https://github.com/QwenAudio/SenseVoice<br>
This repository is intended to make SenseVoice output Traditional Chinese.

After installing Verbatim, you can choose which model to use for speech recognition. SenseVoice is one of the available models. However, because its tokens are in Simplified Chinese, all recognised text is output in Simplified Chinese.

The files in this repository replace the original tokens with Traditional Chinese equivalents and recalculate their hashes.

Simply overwrite the two files .verbatim-integrity.json and tokens.txt in:

`Verbatim/Data/models/sense-voice-int8`

with the files provided in this repository. Verbatim will then convert the Simplified Chinese output from SenseVoice into Traditional Chinese.

**Tested with:** Verbatim v0.14.2
