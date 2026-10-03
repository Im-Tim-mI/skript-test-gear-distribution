# 測試裝備發放系統

[English](README.md) | **繁體中文**

替測試人員直接穿上臨時測試裝備：鑽石盔甲與鞘翅（皆附綁定詛咒與消失詛咒），並給予 320 個煙火，且禁止丟棄或放入容器。

> 本儲存庫包含同一個腳本的兩個版本：**繁體中文（zh-TW）** 是作者伺服器實際使用的原始版本；**English** 為完整英文翻譯版（指令、訊息與變數名稱皆為英文），功能相同。

## 功能特色

- 直接穿到裝備欄（頭盔、鞘翅、護腿、靴子）
- 綁定詛咒 + 消失詛咒：無法脫下、死亡後消失
- 耐久 III + 經驗修補，另給 320 個煙火
- 禁止丟棄或放入容器
- 可回收單一或全體玩家的裝備（煙火保留），並查詢誰穿著

## 需求

- [Paper](https://papermc.io/) 伺服器（開發環境 Paper 26.2 / Minecraft 26.2）
- [Skript](https://github.com/SkriptLang/Skript)（開發環境 2.16.2）

## 安裝

1. 先安裝[需求](#需求)中列出的插件。
2. 下載**其中一個**版本：

   | 版本 | 檔案 |
   |---|---|
   | 繁體中文（原始版本） | [`zh-TW/測試裝備發放系統.sk`](zh-TW/%E6%B8%AC%E8%A9%A6%E8%A3%9D%E5%82%99%E7%99%BC%E6%94%BE%E7%B3%BB%E7%B5%B1.sk) |
   | English（英文） | [`en/test-gear-distribution.sk`](en/test-gear-distribution.sk) |

3. 把 `.sk` 檔案放進伺服器的 `plugins/Skript/scripts/`。
4. 執行 `/sk reload 測試裝備發放系統`（請換成你放入的檔名），或重新啟動伺服器。

> [!IMPORTANT]
> **只能安裝其中一個版本。** 兩個版本是同一個腳本的不同語言，同時載入會互相衝突或重複執行。

## 指令

| 指令（中文版） | 英文版 | 說明 | 權限 |
|---|---|---|---|
| `/發放測試裝備 [玩家]` | `/givetestgear [player]` | 發放給指定玩家；省略時發給全體在線玩家 | OP |
| `/回收測試裝備 <玩家>` | `/recalltestgear <player>` | 回收指定玩家的測試裝備 | OP |
| `/回收全部測試裝備` | `/recallalltestgear` | 回收全體在線玩家的測試裝備 | OP |
| `/查看測試裝備` | `/checktestgear` | 列出穿著測試裝備的在線玩家 | OP |

## 設定

- `options:` 的 `item_name` 用來辨識測試裝備，請確保名稱獨一無二。

## 注意事項

- ⚠️ 發放時會**直接覆蓋**玩家身上原本的裝備，原裝備不會歸還。

## 相關專案

- [skript-tester-thank-you-kit](https://github.com/Im-Tim-mI/skript-tester-thank-you-kit)－測試人員感謝套裝發放
- [skript-special-item-lock](https://github.com/Im-Tim-mI/skript-special-item-lock)－特殊物品封鎖系統

## 授權

**MIT + Commons Clause**，完整條款請見 [LICENSE](LICENSE)。

- ✅ 可自由使用、複製、修改與分享本腳本。
- ✅ 本授權明確允許在收費或營利的 Minecraft 伺服器上安裝與運行本插件（含修改版）。
- ❌ 禁止的僅限於直接或間接販售本插件本體、修改版本，或以付費方式取得其檔案或原始碼。

Copyright (c) 2026 廷廷小教室、廷廷的家（Tim945）
