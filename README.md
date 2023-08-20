
# [精 銳 矩 陣 計 算 求 解 器 ( SMS Solver ) ：](https://github.com/myyeh2/Docs_2A/blob/main/README.md)  

## 【完全精確，而不是近似】求解動態系統，包含狀態空間變數(state-space variables)的響應值(是實數值)、系統特徵值(頻率，是複數值)、和特徵向量(模態，是複數值)，於微軟 Visual Studio 的開發環境上，使用C#程式語言專案實作和執行。    

### 如果實際去量測(measurement)頻率和模態時，就是特徵值和特徵向量(兩者都是複數值)的絕對值(absolute value)或稱模數(modulus)。

### 複數(a + b i) = SQRT(a ^ 2 + b ^ 2) * ( Cos(theta) + i * Sin(theta) ) 或稱歐拉公式、Polar Form    

## 動態系統的計算 : 系統矩陣(或稱狀態矩陣)是實數，求得的特徵值和特徵向量是複數，實數的部分與虛數的部分，必需完全整合在一起運算，不可將實數值和虛數值(即複數值)分開運算，但最後運算的結果，顯示狀態變數的響應值(即時間軸上的振幅)是實數。本軟體計算動態系統時，都是使用複數矩陣的運算，這也是本軟體的最大特色。  

<!--  myyeh2.github.com   --> 

#### 1. 本實例驗證參考 Dennis G. Zill, " Differential Equations with Boundary-Value Problems 9th edition "  Page 322 Example 1。  

#### 2. 本實例繪圖係採用 Python 程式語言的 Matplotlib 套件，但亦可使用 Excel 繪圖。  

#### 3. 其他實例驗證，請參考 [ 精 銳 矩 陣 計 算 求 解 器 ( GitHub 儲存庫 ) ](https://github.com/myyeh2/)  
