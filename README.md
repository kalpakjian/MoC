# MoC — Master of Cube

一個基於 Unity Universal Render Pipeline（URP）的 3D 專案，以方塊（Cube）為核心元素進行場景與材質設計。

---

## 專案資訊

| 項目 | 內容 |
|------|------|
| 引擎 | Unity 2022.3.62f3 (LTS) |
| 渲染管線 | Universal Render Pipeline (URP) |
| 分支 | `master` |
| 場景 | `Assets/MoC.unity` |
| 核心 Prefab | `Assets/master_of_Cube.prefab` |

---

## 環境需求

- **Unity Hub**（最新版）
- **Unity 2022.3.x LTS**（建議使用 2022.3.62f3）
  - 可於 [Unity Download Archive](https://unity.com/releases/editor/archive) 下載對應版本
- **Git**（用於 Clone 專案）
- Windows 10/11 或 macOS 12+

---

## Clone 專案

開啟終端機（Terminal / Command Prompt / PowerShell），執行以下指令：

```bash
git clone https://github.com/kalpakjian/MoC.git
```

Clone 完成後，專案資料夾 `MoC` 會出現在當前目錄。

---

## 用 Unity 開啟專案

### 方法一：透過 Unity Hub（推薦）

1. 開啟 **Unity Hub**
2. 點選左側 **Projects**
3. 點選右上角 **Open > Add project from disk**
4. 瀏覽至剛 Clone 下來的 `MoC` 資料夾，選擇該資料夾並點擊 **Open**
5. Unity Hub 會自動偵測到專案使用的 Unity 版本（2022.3.62f3）
   - 若尚未安裝該版本，Unity Hub 會提示你安裝，點選 **Install** 安裝即可
6. 安裝完成後，點選專案名稱即可開啟

### 方法二：直接從 Unity Editor 開啟

1. 開啟 Unity 2022.3.x
2. 在啟動畫面選擇 **Open**
3. 選擇 Clone 下來的 `MoC` 資料夾
4. 點擊 **Open**

> **注意**：首次開啟時，Unity 會自動匯入所有 Assets，可能需要數分鐘，請耐心等待。

---

## 開啟主場景

專案開啟後，若未自動載入場景，請手動開啟：

1. 在 **Project** 視窗中，瀏覽至 `Assets/`
2. 雙擊 **`MoC.unity`** 開啟主場景
3. 點選 Unity 頂部的 **▶ Play** 按鈕即可執行

---

## 專案結構

```
MoC/
├── Assets/
│   ├── MoC.unity                          # 主場景
│   ├── master_of_Cube.prefab              # 核心 Cube Prefab
│   ├── A.mat / A 1.mat … A 8.mat         # 材質檔案（Cube 用）
│   ├── Settings/                          # URP 渲染設定
│   ├── UniversalRenderPipelineGlobalSettings.asset
│   ├── TutorialInfo/                      # Unity 樣板教學資訊
│   └── Unity.VisualScripting.Generated/   # Visual Scripting 生成檔
├── Packages/                              # Unity Package 相依設定
├── ProjectSettings/                       # 專案設定
│   └── ProjectVersion.txt                 # Unity 版本記錄
├── .gitattributes
└── .gitignore
```

---

## 常見問題

**Q: 開啟時出現 URP 相關警告或錯誤？**  
A: 確保已安裝 `Universal RP` package。可前往 **Window > Package Manager**，搜尋 `Universal RP` 並安裝或更新。

**Q: 場景顯示為粉紅色（材質錯誤）？**  
A: 這通常是 URP Shader 未正確套用。前往 **Edit > Rendering > Render Pipeline Converter**，執行材質升級。

**Q: Unity 版本不符合怎麼辦？**  
A: 建議使用 **2022.3.x LTS** 系列版本（任一 patch 版本皆可），避免使用 2023.x 或更高版本以防相容性問題。

---

## License

This project is for learning and portfolio purposes.
