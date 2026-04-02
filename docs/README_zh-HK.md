# 小米自訂開機動畫
[English](/README.md) | [简体中文](/README_zh-CN.md) | 繁體中文

文檔最後更新：16/03/2026

## 介紹
一個簡單的模組，可以將預設的開機動畫替換為自訂動畫，並且幾乎適用於所有小米裝置。所以應該可以幫你節省搭建或排除問題的時間。此模組也兼容平板裝置，因為與手機不同，平板裝置通常會根據裝置方向調整其動畫。

此模組使用 systemless 掛載方式將開機動畫檔案掛載到指定位置，確保不會對系統分區進行任何修改。

## 要求
- Magisk v26.1+ / KernelSU v0.8.0+ / APatch 10568+
- Android 11+ (API 30+) 運行 MIUI / HyperOS

> [!WARNING]
> 此模組也可以在其他具有掛載功能的 Root 管理器或具有類似檔案結構的裝置上運行，歡迎自行測試，但不會提供支援，也不保證功能正常。

## 測試記錄

| 裝置 | 系統版本 | 狀態 | RM |
|------|----------|:----:|------|
| liuqin | V14.0.9.0.TMYCNXM | ✅ | Magisk |
| liuqin | OS2.0.203.0.VMYCNXM | ✅ | Magisk |
| liuqin | OS2.0.212.0.VMYCNXM | ✅ | Magisk |
| liuqin | OS3.0.5.0.VMYCNXM | ✅ | Magisk / KSU + 任何元模組 |

<details>
<summary>裝置代碼對照表</summary>

| 代碼 | 裝置名稱 |
|------|----------|
| myron | 紅米K90 Pro Max / POCO F8 Ultra |
| annibale | 紅米K90 / POCO F8 Pro |
| popsicle | 小米17 Pro Max |
| pandora | 小米17 Pro |
| pudding | 小米17 |
| piano | 小米平板8 Pro |
| yupei | 小米平板8 |
| klimt | 小米15T Pro |
| goya | 小米15T |
| organ | 紅米平板2 Pro 5G |
| flute | 紅米平板2 Pro / POCO Pad M1 |
| dew | 紅米15C / POCO C85 |
| tornado | 紅米15C 5G / 紅米15R 5G |
| kunzite | 紅米Note15 5G |
| lapis | 紅米Note15 Pro |
| flourite | 紅米Note15 Pro+ |
| creek | 紅米15 4G |
| spring | 紅米Note15R / 紅米15 5G / POCO M7 Plus 5G |
| dali | 紅米K80 至尊版 |
| bixi | 小米MIX Flip 2 |
| turner | 紅米K平板 / 小米平板Mini |
| violin | 小米平板7S Pro 12.5 |
| taiko | 紅米平板2 |
| koto | 紅米平板2 4G |
| dijun | 小米15S Pro |
| jinghu | 小米平板7 Ultra |
| luming | 小米Civi5 Pro |
| onyx | 紅米Turbo 4 Pro / POCO F7 |
| serenity | POCO C71 / 紅米A5 |
| emerald | 紅米Note 14S |
| xuanyuan | 小米15 Ultra |
| obsidian | 紅米Note 14 Pro 4G |
| tanzanite | 紅米Note 14 4G |
| rodin | 紅米Turbo 4 / POCO X7 Pro |
| miro | 紅米K80 Pro / POCO F7 Ultra |
| zorn | 紅米K80 / POCO F7 Pro |
| warm | POCO C75 5G / 紅米A4 5G |
| haotian | 小米15 Pro |
| dada | 小米15 |
| muyu | 小米平板7 Pro |
| uke | 小米平板7 / POCO Pad X1 |
| degas | 小米14T |
| amethyst | 紅米Note14 Pro+ |
| malachite | 紅米Note14 Pro / POCO X7 |
| beryl | 紅米Note14 5G / POCO M7 Pro 5G |
| flame | 紅米14R 5G / POCO M7 5G |
| lake | 紅米14C / 紅米A3 Pro / POCO C75 |
| flare | 紅米平板SE 8.7 WiFi |
| spark | 紅米平板SE 8.7 4G |
| breeze | 紅米13 5G / 紅米Note 13R / POCO M6 Plus 5G |
| ruyi | 小米MIX Flip |
| goku | 小米MIX Fold 4 |
| rothko | 紅米K70 至尊版 / 小米14T Pro |
| klein | 紅米A3x |
| peridot | 紅米Turbo 3 / POCO F6 |
| ruan | 紅米平板 Pro 5G / POCO Pad 5G |
| dizi | 紅米平板 Pro |
| chenfeng | 小米CIVI 4 Pro / 小米14 Civi |
| blue | 紅米A3 / POCO C61 |
| aurora | 小米14 Ultra |
| shennong_t | 小米14 Pro 鈦金屬版 |
| sheng | 小米平板6S Pro 12.4 |
| sapphiren | 紅米Note13 4G NFC |
| sapphire | 紅米Note13 4G |
| moon | 紅米13 / POCO M6 |
| air | 紅米13R 5G / 紅米13C 5G |
| duchamp | 紅米K70E / POCO X6 Pro 5G |
| manet | 紅米K70 Pro |
| vermeer | 紅米K70 / POCO F6 Pro |
| gale | 紅米13C / POCO C65 |
| shennong | 小米14 Pro |
| houji | 小米14 |
| aristotle | 小米13T |
| garnet | 紅米Note 13 Pro 5G / POCO X6 |
| gold | 紅米Note 13 5G / 13R Pro |
| zircon | 紅米Note 13 Pro+ 5G |
| xun | 紅米平板SE |
| babylon | 小米MIX Fold 3 |
| corot | 紅米K60 至尊版 / 小米13T Pro |
| yudi | 小米平板6 Max |
| sky | 紅米Note 12R / POCO M6 Pro 5G / 紅米12 5G |
| fire | 紅米12 |
| pearl | 紅米Note 12T Pro |
| yuechu | 小米CIVI3 |
| sea | 紅米Note 12S |
| ishtar | 小米13 Ultra |
| liuqin | 小米平板6 Pro |
| pipa | 小米平板6 |
| sweet_k6a | 紅米Note 12 Pro 4G |
| topaz | 紅米Note 12 4G NFC |
| tapas | 紅米Note 12 4G |
| marble | 紅米Note 12 Turbo / POCO F5 5G |
| water | POCO C51 / 紅米A2 / A2+ |
| earth | 紅米12C / POCO C55 |
| redwood | 紅米Note 12 Pro 極速版 / POCO X5 Pro 5G |
| rembrandt | 紅米K60E |
| socrates | 紅米K60 Pro |
| mondrian | 紅米K60 / POCO F5 Pro |
| nuwa | 小米13 Pro |
| fuxi | 小米13 |
| moonstone | POCO X5 5G |
| sunstone | 紅米Note 12 5G / 紅米Note 12R Pro |
| ruby | 紅米Note 12 Pro+ |
| plato | 小米12T |
| yunluo | 紅米平板 |
| ziyi | 小米CIVI 2 / 小米13 Lite |
| ice | POCO C50 / 紅米A1 |
| rosemary_p | POCO M5S |
| rock | POCO M5 / 紅米11 Prime 4G |
| dagu | 小米平板5 Pro 12.4 |
| diting | 紅米K50 至尊版 / 小米12T Pro |
| zizhan | 小米MIX Fold 2 |
| mayfly | 小米12S |
| thor | 小米12S Ultra |
| unicorn | 小米12S Pro |
| daumier | 小米12 Pro 天璣版 |
| taoyao | 小米12 Lite |
| frost | POCO C40 |
| xaga | 紅米Note 11T Pro / Pro+ / POCO X4 GT / Pro / 紅米K50i / Pro |
| zijin | 小米CIVI 1S |
| lilac | 紅米Note 10T |
| dandelion | 紅米10A |
| fog | 紅米10C |
| rubens | 紅米K50 |
| matisse | 紅米K50 Pro |
| munch | 紅米K40S / POCO F4 |
| viva | 紅米Note 11 Pro |
| lightcm | 紅米Note 11R |
| light | 紅米Note 11E / POCO M4 5G / 紅米10 Prime+ 5G |
| ingres | 紅米K50 電競版 / POCO F4 GT |
| spesn | 紅米Note 11 NFC |
| spes | 紅米Note 11 |
| veux | 紅米Note 11E Pro / 紅米Note 11 Pro 5G |
| opal | 紅米Note 11S 5G |
| fleur | 紅米Note 11S / POCO M4 Pro 4G |
| zeus | 小米12 Pro |
| psyche | 小米12X |
| cupid | 小米12 |
| evergreen | POCO M4 Pro 5G |
| pissarro | 紅米Note 11 Pro / Pro+ |
| evergo | 紅米Note 11 5G |
| selenes | 紅米Note 11 4G |
| mona | 小米CIVI |
| lisa | 小米11青春活力版 |
| agate | 小米11T |
| vili | 小米11T Pro |
| selene | 紅米10 |
| odin | 小米MIX4 |
| elish | 小米平板5 Pro (WiFi) |
| enuma | 小米平板5 Pro (5G) |
| nabu | 小米平板5 |
| chopin | 紅米Note 10 Pro (China) / POCO X3 GT |
| camellia | 紅米Note 10 (China) / POCO M3 Pro / 紅米Note 11 SE |
| biloba | 紅米Note 8 (21年款) |
| ares | 紅米K40 遊戲增強版 / POCO F3 GT |
| cetus | 小米MIX Fold |
| renoir | 小米11 青春版 |
| star | 小米11 Pro / Ultra |
| courbet | 小米11 Lite 4G |

</details>

> [!NOTE]
> 此模組應該可以在其他型號、品牌和系統上運行，但仍需進一步測試。歡迎反饋您的測試結果！

## 安裝

> [!CAUTION]
> 請勿直接下載並刷入發佈版本，除非您想手動替換開機動畫檔案。請使用下方的 **GitHub Actions 工作流程** 來構建包含您自訂動畫的模組。

1. 使用 [GitHub Actions 工作流程](#github-actions構建您自己的模組) 構建您的自訂模組
2. 從 Artifacts 下載構建好的模組
3. 在 Magisk / KernelSU / APatch 應用中直接刷入下載的 ZIP（無需先解壓）
4. 重啟

## 備份與還原

在**首次安裝**時，系統會提示您備份當前的開機動畫。備份功能可幫助您在需要時還原原始動畫。

### 備份行為

**首次安裝：**
- 首次安裝模組時，如果不存在備份，系統會提示備份當前的開機動畫
- 備份儲存在 `/data/adb/boot-backups/` 中，包含您所選位置的所有 `bootanimation*.zip` 檔案

**模組更新：**
- 更新模組時，如果已存在備份，備份過程將自動跳過
- 您的原始開機動畫從首次安裝時就已安全備份

### 還原原始動畫

要還原原始開機動畫：

1. 在 Magisk/KernelSU/APatch 中**停用或解除安裝此模組**
2. **重啟**裝置

## 待辦事項
1. ~~添加 GitHub Actions 工作流程以自動構建模組~~（完成）
2. ~~自動偵測並選擇相應型號的路徑~~（由於裝置偽裝模組的普遍使用，可能不會實現）
3. 影片轉開機動畫

## GitHub Actions（構建您自己的模組）

您可以使用 GitHub Actions 構建自訂開機動畫模組，無需任何本機工具！工作流程會自動下載最新版本作為基礎。

### 方法一：使用範本

1. **Fork** 此倉庫
2. 前往 **Actions** → **"Build Custom Module"**
3. 點擊 **"Run workflow"**
4. 將 **Source** 設定為 `template`
5. 選擇您的**裝置型號**（例如 `liuqin`）
6. 選擇**範本**（例如 `HyperOS`）
7. 選擇**目標位置**
8. 從 **Artifacts** 下載構建好的模組

> [!NOTE]
> 如果沒有適用於您裝置的範本，您必須使用[方法二](#method-2-upload-custom-files)並上傳您自己的開機動畫檔案。

### 方法二：上傳自訂檔案

1. **Fork** 此倉庫
2. 將您的 `bootanimation.zip` 檔案添加到 `upload/` 資料夾
3. 提交並推送您的變更
4. 前往 **Actions** → **"Build Custom Module"**
5. 點擊 **"Run workflow"**
6. 選擇 `upload` 作為來源
7. 選擇**目標位置**
8. 從 **Artifacts** 下載構建好的模組

> [!TIP]
> 如果您的裝置是手機，您只需要一個 `bootanimation.zip` 檔案。多個動畫檔案僅適用於會根據裝置方向變更動畫的平板裝置。

> [!WARNING]
> `upload/` 資料夾僅供在您自己的 Fork 中個人使用。請勿提交包含此資料夾變更的 Pull Request，否則將被自動關閉。

### 可用目標位置

| 位置 | 描述 |
|------|------|
| `/product/media` | 預設位置 |
| `/system/media` | 傳統位置 |
| `/system_ext/media` | 系統擴展媒體 |

> [!TIP]
> 如果安裝後開機動畫沒有任何變化，可能選擇了錯誤的路徑。請嘗試重新刷入模組並選擇其他位置。

### 檔案命名規範

- `bootanimation.zip` - 主開機動畫
- `bootanimation01.zip` - 備選動畫 1（其他旋轉角度）
- `bootanimation02.zip` - 備選動畫 2
- ... 以此類推

### 開機動畫檔案要求

每個 `bootanimation.zip` 應包含：

```
bootanimation.zip
├── desc.txt          # 必需：動畫描述符
├── part0/            # 必需：第一個動畫部分
│   ├── 00000.png
│   ├── 00001.png
│   └── ...
├── part1/            # 可選：第二個動畫部分
│   ├── 00000.png
│   └── ...
└── ...
```

#### desc.txt 格式

```
<高度> <寬度> <幀率>
<類型> <循環次數> <暫停幀數> <路徑>
...
```

示例：
```
1880 2880 60
p 0 5 part0
```

- `c` = 完整播放， `p` = 播放並重複
- 第一個數字 = 循環次數（0 = 無限）
- 第二個數字 = 循環後暫停（以幀為單位）
- 路徑 = 包含幀的資料夾

> [!NOTE]
> GitHub Actions 工作流程會自動使用標準壓縮格式建立適合 Magisk 的模組 ZIP 檔案。

## 免責聲明
**儘管刷寫此模組導致裝置進入引導循環的可能性很小，但仍強烈建議使用引導循環保護模組。對於使用此模組對您的裝置或資料造成的任何損害，我概不負責。使用風險自負。**

## 許可證
    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>.
