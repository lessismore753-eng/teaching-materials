# Tab-Stroke 使用規範

## 元件目的

`Tab-Stroke` 用於以底線（stroke）標示目前選中的分頁或導航項目。

來源顯示 `Tab-Stroke` 支援 Desktop 與 Mobile 兩種裝置尺寸，並可呈現 Icon＋文字、純文字、純 Icon 三種顯示模式。

## 適用情境

- 網站頂部主要導航。
- Desktop 上以 Icon＋文字模式協助使用者辨識功能區域。
- Mobile 上以純 Icon 模式節省螢幕空間。
- Mobile 上作為底部導航或功能分頁。
- Mobile 上以純文字模式呈現功能分頁。

## 元件選擇方式

```text
Desktop 尺寸
→ Tab-Stroke/Desktop

Mobile 尺寸
→ Tab-Stroke/Mobile

需要同時顯示圖示與文字
→ Show icon = true；Show Text = true

只顯示文字
→ Show icon = false；Show Text = true

只顯示圖示
→ Show icon = true；Show Text = false
```

## 元件特有的使用與禁止規則

### 使用規則

- `Tab-Stroke` 由原子元件 `Tab-Stroke/Desktop` 與 `Tab-Stroke/Mobile` 組成。
- 使用底線（stroke）標示選中狀態。
- `Tab-Stroke` 之間的間距可彈性設定。
- 顯示模式透過 `Show icon` 與 `Show Text` 布林屬性控制。
- Icon＋文字模式用於完整展示。
- 純文字模式需隱藏 Icon。
- 純 Icon 模式需隱藏文字。
- Desktop 網站主導航可使用 Icon＋文字模式。
- Mobile 可使用純 Icon 模式節省螢幕空間。

### 禁止規則

- 不得將示意文案視為 Tab 名稱規格，例如「住宅火災保險」、「汽車保險」、「旅行平安險」、「基本資料」、「進階設定」、「通知偏好」。
- 不得自行新增 Figma 未定義的顯示模式。
- 不得自行推測 `Show icon` 與 `Show Text` 以外的 Variant Property。
- 不得自行推測固定間距、尺寸、padding、gap、stroke 寬度或色彩 Token。
- 不得將 Desktop 與 Mobile 原子元件互換使用。

## 衝突與尚未定義事項

### 衝突

- undefined

### 尚未定義

- `componentId` 未在此 Figma node 可見內容中定義。
- `Tab-Stroke` 的正式分類未在此 Figma node 可見內容中定義。
- 選中狀態以外的狀態集合未定義。
- `Show icon` 與 `Show Text` 的正式 Figma Property 型別除布林敘述外未提供機器值。
- Icon 的正式資產名稱、替換規則與可用清單未定義。
- Text label 的字級、字重、行高與 Text Style 未定義。
- Stroke 的色彩、寬度、位置與 Token 未定義。
- Desktop 與 Mobile 的完整尺寸、padding、gap、min width、max width 未定義。
- 多個 Tab 之間「間距可彈性設定」的可用範圍未定義。
- 鍵盤操作、Focus、ARIA 與讀屏名稱未定義於此元件 node。
- 純 Icon 模式是否必須提供 tooltip 或可見輔助文字未定義於此元件 node。
