
<!--  C:\2302\github\io.github     -->


![](Images\09-11-01.png)  
<!--   
# \[ { \color{Brown}精\;銳\;矩\;陣\;計\;算\;求\;解\;器} \]  
#### \[ { \color{Green}【Sharp \; Matrix \; Solver \quad\; S\; M\; S】} \]
-->



![](Images\09-11-02.png)  
<!--   
##### \[ { \color{Red}Dennis\quad G.\quad Zill} \]  
##### \[ { \color{Red} Differential \; Equations\; with \; Boundary \_ Value \; Problems \; 9th\;Ed.\; 第322頁 \; Ex \_1 } \]
-->




![](Images\09-11-03.png)  
<!-->
## \( { \color{Green} 動態系統的精確正解法（非近似求解法）} \) 
### 求解動態系統，包含狀態空間變數(state-space variables)的響應值【實數值】、系統特徵值【頻率，複數值】、和對應之特徵向量【模態，複數值】，由學公式的推導，更重要的是C#程式語言的實作，在微軟 Visual Studio 開發環境上，相關專案的測試、執行與驗證。    
### 如果實際去\({\color{red}量測}\)【measurement】\({\color{fuchsia}頻率和模態}\)時，就是對應\( {\color{red}複數特徵值和複數特徵向量的絕對值}\)【absolute value】或稱\({\color{red}模數}\)【Modulus】。以上是本人以CSharp程式碼實作所得到的結論，雖然電機系與電子系的學科，譬如訊號與系統等等，有用到複數的計算，但好像也沒有人實際實作過，而且在Matlab軟體或是相關的論文上，好像也找不到相關的論述，若有發現時也請通知本人，並在此表示謝意。
-->  



  
![](Images\09-11-04.png)
<!-->
## \( { \color{Green}歐拉公式}  \)
#### \( { \color{red} { 複數(a + b \; i) = SQRT( a^2 + b^2  ) * ( Cos( \theta ) + i * Sin( \theta ) ) } } \)    
### \( { \color{red}e^{(a + b \, i)*t} = e^{a*t} * ( Cos( b * t ) + i * Sin( b * t ) )} \)
-->  




![](Images\09-11-05.png)  
<!--  
## \( { \color{Green}SMS = 直接求解矩陣微分方程式 + 使用程式庫 } \)
##### \( \ddot{y}(t) = \ddot{y_h}(t) + \ddot{y_p}(t) , \quad \dot{y}(t) = \dot{y_h}(t) + \dot{y_p}(t) , \quad y(t) = y_h(t) + y_p(t) \)    
#### \( A \ast Q = Q \ast D, \quad if \quad DET(Q) \not= 0 \quad then \quad \Longrightarrow \quad  { \color{red} A = Q \ast D \ast Q_i} \)
#### \( [ \; \ddot{y_h}(t) \; | \; \dot{y_h}(t) \; ] =  \begin{bmatrix} \ddot{y_h}(t) \\ \dot{y_h}(t)  \end{bmatrix} = { \color{red} A } \ast \begin{bmatrix} \dot{y_h}(t) \\ y_h(t) \end{bmatrix}  \)
#### \(  [ \; \dot{y_h}(t) \; | \; y_h(t) \; ] =  \begin{bmatrix} \dot{y_h}(t) \\ y_h(t)  \end{bmatrix} \; = \; { \color{red} H_{exp}(D, \; Q, \; t) \ast \; d_h \; } \)  
#### \( {\color{red}A} 是狀態(系統)矩陣， \quad {\color{red}D} 是特徵值矩陣， \quad {\color{red}Q} 是特徵向量矩陣。 \quad \)
##### \( { \color{red} H_{exp}(D, Q, t) } \quad 是狀態變數響應函數(本人自已定義，未有人推導與實作） \)
#### \( { \color{red} d_h } \quad 純係數向量，由初始值或邊界值待定，不是時間 \; t \;的函數  \)
-->  




![](Images\09-11-06.png)    
<!--  
## \( { \color{Green}討論議題 :} \)   
#### 1. 系統矩陣(或稱狀態矩陣)是實數，但求得的特徵值和特徵向量均為複數，實數的部分與虛數的部分，必需完全整合在一起運算，不可將實數值和虛數值(即複數值)單獨分開運算，但最後複數矩陣運算的結果，也是狀態變數的響應值(即時間軸上的振幅)是實數。本軟體計算動態系統時，都是使用複數矩陣的運算，這也是本軟體的最大特色。   
#### 2. 本實例的繪圖部分係採用 Python 程式語言的 Matplotlib 套件繪圖，但也可使用 Excel 繪圖。  
#### 3. 其他實例驗證，請參考 [ 精 銳 矩 陣 計 算 求 解 器 ( 相關的實例驗證，即儲存庫中的各種檔案 ) ]  
#### 4. Fourier Transform, Laplace Transfor, Z Transform, 以及Convolution Integer 是近似的求解法，而且僅適用於1度空間點(m=1)多階(r>1)的情況，但本法是先進的求解法，可直接求解多度空間點(m>1)多階(r>1)的微分方程式，更可使用類別庫程式碼，求解很方便。但使用各種轉換(Transform)技術，間接且不容易求解，原因是沒有一定的步驟，程式碼撰寫也不容易。  
-->  

# \[ \] 
# \[ \]  
