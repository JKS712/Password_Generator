# 密碼產生器：資料結構與演算法實作專案

## 專案簡介

基於Java的密碼產生器應用程式，深入探討資料結構設計與演算法效能分析。實作三種Hash Function演算法（簡單除法、乘法、通用Hash），並比較ArrayList、LinkedList、HashMap、TreeMap等資料結構的效能表現，展示理論知識在實際軟體開發中的應用價值。

## 主要功能

- **密碼產生**：支援4-50字符長度調整，多種字符集選擇
- **演算法比較**：三種Hash Function實作與效能測試
- **歷史管理**：ArrayList儲存完整歷史，LinkedList管理最近密碼
- **效能分析**：資料結構操作效能比較與視覺化報告
- **GUI介面**：完整的Swing圖形化使用者介面

## 技術特色

### Hash Function 實作
- **簡單除法Hash**：`h(k) = k mod m`
- **乘法Hash**：使用黃金比例常數優化分布
- **通用Hash**：隨機係數確保最佳均勻性

### 資料結構比較
- **ArrayList vs LinkedList**：存取與插入效能分析
- **HashMap vs TreeMap**：查找效能與排序支援比較

## 系統需求

- Java JDK 8 或更高版本
- 最少 512MB RAM
- 支援 Windows、macOS、Linux

## 快速開始

```bash
# 編譯並執行
javac *.java
java PasswordGenerator

# 或使用批次檔案
compile_and_run.bat    # Windows
./compile_and_run.sh   # Unix/Linux/Mac

#備註 :
編碼問題中文會有亂碼
亦可使用 compile_english.bat 的英文版
```

## 實驗結果

# Hash Function 效能測試 (10,000次測試)
Password Length: 32 characters
- Simple Hash (Division Method): Total   132.77 ms, Average   0.0133 ms
- Multiplication Hash (Fixed)  : Total   225.06 ms, Average   0.0225 ms
- Universal Hash               : Total   249.45 ms, Average   0.0249 ms%

# 資料結構效能比較 (10,000次操作)
- Insert 10000 elements:
  ArrayList: 3.81 ms
  LinkedList: 2.46 ms

- Random access 1000 times:
  ArrayList: 0.51 ms
  LinkedList: 6.62 ms
