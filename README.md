# mkv-chapter-splitter
我做的 macOS MKV 章節分割工具：分段影片與無損 FLAC、內建預覽、歌單命名與 Talking 標記，以及含封面的 Apple Music／ALAC 匯入。

## 使用條件與限制
- 編譯目標為 macOS 13 以上；預編譯檔只提供 arm64，目前僅完成單台 Apple Silicon Mac 實機測試。
- 需另外安裝 FFmpeg 與 MKVToolNix：brew install ffmpeg mkvtoolnix。
- 輸入為已可讀取且含章節的 MKV，來源需有支援的無損音軌。
- 影片切點受關鍵影格影響；Talking 抽樣分類可能需要人工修正。
- App 未取得 Apple Developer ID 簽章與公證，系統可能限制直接開啟下載版；可審閱原始碼後自行編譯。
- 原始 FLAC 保留；成功後清除轉檔暫存，資料庫播放所需音檔保留。
