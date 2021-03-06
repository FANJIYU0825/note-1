#PHP筆記

#基本語法
* PHP的程式碼要放在
```
<?php
     
?>
```
之中

* 跟Java一樣，以`;`來斷句
* 可被放入HTML之中
* 檔名以`.php`結尾，就算置於HTML之中也一樣，因為這樣才會執行PHP程式碼的部份。

##註解
```php
//單行註解
/*
多
行
註
解
*/
```

##I/O
###standard output
```php
echo "Hello World!";
```

##運算子
###算術運算子

###邏輯運算子
```php
> // 大於
>= // 大於等於
< // 小於
<= // 小於等於
== // 等於
!= // 不等於
```

###boolean operator
```php
|| // or
```

##變數
* 變數名稱以`$`開頭，且為case-sensitive
* 以`=`賦值

例子：
```php
$var = "something"; // a string variable
$num = 0.01; // a number variable
$condition = true; // a boolean variable
echo $num; // output a variable
```

##陣列
* 宣告時元素間以`,`分隔  
* 陣列的index由0開始  
* 取用元素時可以用`[]`或`{}`  

```php
$array = array("item1", "item2", "item3"); //宣告一個陣列
echo $array[1]; // 輸出編號為1的元素，也就是item1
echo $array{1}; //結果同上，只是換一種符號
unset($array[1]); //刪除編號為1的元素
unset($array); //刪除整個陣列
```

###多維陣列

###associative array (map)

###相關內建函數
* array_push($array, $element)：將$element插入到$array的最後
* count($array)：回傳$array的元素個數
* sort($array), rsort($array)：遞增／減排序$array
* join($str, $array)：將$array中的元素以$str串接起來

##條件判斷式
### if/else
```php
if($booleanVal){
    // do something
} elseif ($booleanVal2){
    // do something
} else{
    // do something
}
```

###switch case
####style 1
類似Java的switch

```php
switch ($val) {
    case 0:
        // do something
        break;
    case 1:
        // do something
        break;
    default:
        // do something
}
```

####style 2
```php
switch ($val):
	case 0:
        // do something
        break;
    case 1:
        // do something
        break;
    default:
        // do something
endswitch;
```


##迴圈
###for
類似Java

```php
for ($i = 0; $i < 10; $i++) {
    // do something!
}
```

###foreach
```php
foreach ($array as $element){
    // do something!
}
```

###while
####style1
類似Java的while loop
```php
while($booleanVal) {
   // do something!
}
```

####style2
```php
while($booleanVal):
   // do something!
endwhile;
```

###do/while
類似Java的do/while  
```php
do {
    // do something!
} while ($booleanVal);
```

##字串
* 字串以`""`包覆
* 串接運算子為`.`，例如`"Hello" . "World"`的結果等同於"HelloWorld"

###相關內建函數
* strlen($str)：取得字串長
* substr($str, startIndex, length)：取得$str中開始於startIndex，長length的子字串
* strtoupper($str)：將$str轉換成大寫
* strtolower($str)：將$str轉換成小寫
* strpos($str, $target)：在$str中找尋$target，若有，則回傳起始index；若無，則回傳false

##函數
###常用內建函數
####數學函數
* round($float) / round($float, $precision)：四捨五入$float／四捨五入$float至小數點後$precision位
* rand() / rand(min, max)：隨機產生一個介於0~32767之間的數字／隨機產生一個位於[min,max]的數字


###自訂函數
自訂函數的語法如下

```php
function funcName($para0, $para1, ...){
    // do something!
    return ...
}
```

注意：
1. 參數的個數可為0至多個
2. 可以沒有`return`
3. function name是大小寫**無關**(case insensitive)
4. function name可包含英數、底線及dash

##物件
###相關內建函數
`is_a(＄obj, Sstr)`：回傳$obj是否屬於名稱為$str的物件  
`property_exists(＄obj, $str)`：回傳$obj是否有名稱為$str的property  
`method_exists(＄obj, Sstr)`：回傳$obj是否有名稱為$str的method  

##內建常數
* M_PI：圓周率pi