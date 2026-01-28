# Moltbot Tactical Pro Cam (v5.1)

這是一個專為 iPhone 12 最佳化的高階 WebGL 即時濾鏡相機 PWA。它透過 GPU 加速的片段著色器（Fragment Shaders）提供專業攝影師級別的即時影像處理。

## 📸 主要用途
本應用旨在模擬專業底片與數位相機的成像質感，提供比 iOS 原生相機更具風格化的即時拍攝體驗。特別針對**日系清新**、**港風富士**以及經典的 **CCD** 色彩進行了硬體級參數模擬。

## 🚀 核心功能
- **全螢幕 iOS 擬真 UI**：完全復刻 iOS 原生相機的交互介面與視覺感受。
- **WebGL 著色器引擎**：利用 GPU 執行 3x3 卷積矩陣運算，達成高品質的銳利化（Sharpness）與分區色調映射（Tone Mapping）。
- **專業底片預設**：內建 CCD、柯達 (Kodak)、富士 (Fuji)、日落、電影等 6 種精密校準的濾鏡。
- **十張連拍選片系統**：支援即時連拍暫存，提供燈箱式選片介面，僅儲存您滿意的照片至 iOS 相簿。
- **戰術手勢**：支援「雙擊畫面」快速翻轉鏡頭，提升實戰操作速度。
- **4K 高解析度支援**：解鎖 iPhone 12 的硬體極限解析度。

## 🛠 技術棧
- **Frontend**: HTML5, CSS3 (iOS SF Pro UI 擬真)
- **Graphics**: WebGL 1.0 (Fragment Shaders, Vertex Shaders)
- **API**: `navigator.mediaDevices.getUserMedia` (相機串流), `navigator.share` (iOS 原生儲存對接)
- **Deployment**: Vercel (PWA 全球分發)

## 📲 安裝說明
1. 在 iPhone 上使用 Safari 開啟 [部署連結](https://moltbot-webgl-camera.vercel.app)。
2. 點擊瀏覽器底部的「分享」按鈕。
3. 選擇「加入主畫面 (Add to Home Screen)」。
4. 從桌面開啟應用，享受全螢幕專業攝影體驗。

## 🧬 Shader 參數映射
本系統嚴格模擬以下 ISP 參數：
- 曝光 (Exposure)
- 鮮明度 (Brilliance)
- 高光/陰影 (Highlights/Shadows)
- 黑點 (Black Point)
- 銳利度 (Sharpness - 卷積矩陣)
- 飽和度/自然飽和度 (Saturation/Vibrance)
- 色溫/色調 (Temperature/Tint)

---
*Developed by Moltbot (System Name: 铁柱)*
