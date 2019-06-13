# blog
網頁位址：[blog](https://fairy042026.github.io/wd107b/exercise/%E6%9C%9F%E6%9C%AB%E5%B0%88%E6%A1%88/tf%E5%B0%8D%E7%85%A7%E7%89%88.html)

功能

1.下拉式選單
```
<div class="dropdown" style="float:right;">
  <button class="dropbtn">tfboys</button>
  <div class="dropdown-content">
    <a href="https://www.instagram.com/karrywang921kw/?hl=zh-tw">karry IG</a>
    <a href="https://www.instagram.com/roy_____wang/?hl=zh-tw">roy IG</a>
    <a href="https://www.instagram.com/__4444x__/?hl=zh-tw">jackson IG</a>
  </div>
</div>

.dropbtn {
    background-color: rgb(243, 176, 52);
    color: white;
    margin: 10PX;
    padding: 20px;
    font-size: 20px;
    border: none;
    cursor: pointer;
}

.dropdown {
    position: relative;
    display: inline-block;
}

.dropdown-content {
    display: none;
    position: absolute;
    right: 0;
    background-color: sandybrown;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
}

.dropdown-content a {
    color: white;
    padding: 30px 20px;
    text-decoration: none;
    display: block;
}

.dropdown-content a:hover {background-color: wheat}

.dropdown:hover .dropdown-content 
{
    display: block;
}

.dropdown:hover .dropbtn {
    background-color: navajowhite;
}
```

2.側欄
```
.menu
{
    position: absolute;/* 固定nav位置 */
    margin: 0;
    padding:0px 10px;
    color: rgb(194, 227, 255);/*字體色*/
    background-color:rgb(221, 147, 11);
    height:1200px;/*元素高度*/
    width: 50px;
    text-align:left;/*字體靠左*/
    font-size: 20px;
    line-height: 40px;
    overflow: hidden;
    transition:width 2s;
    -webkit-transition:width 2s;
}
.menu:hover
{
    width:150px;
    font-size:20px;
}
```
3.嵌入圖片，並讓圖片產生超連結
```
<div P1="position:relative;" style='position:relative; left:150px' >
        <a href="https://www.weibo.com/tfwangjunkai?from=feed&loc=nickname&is_hot=1"><img src="image/tenor (1).gif" ></a>
        <a href="https://www.weibo.com/tfwangyuan?is_hot=1"><img src="image/20170825093210936.gif" style='position:relative; left:220px'></a>
        <a href="https://www.weibo.com/tfyiyangqianxi?is_hot=1"><img src="image/56B3478EBBD6E408E0740EDABB81E2AF04900F79_size374_w240_h240.gif" style='position:relative; left:450px' ></a>
</div>
```

4.跑馬燈
```
 <marquee direction="right" scrollamount="10" height= "20"  style="color: white" >Hello!</marquee>
 ```

5.文字型計算機
```
<script>
            function calculate() {
              var a = document.getElementById('a')
              var op = document.getElementById('op')
              var b = document.getElementById('b')
              var result = document.getElementById('result')
              result.innerText = eval(a.value + op.value + b.value)
            }
          </script>    
              <input id="a" type="text" value="3"/>
              <select id="op">
                <option value="+">+</option>
                <option value="-">-</option>
                <option value="*" selected>*</option>
                <option value="/">/</option>
              </select>
          <!--    <input id="op" type="text" value="*"/>-->
              <input id="b" type="text" value="5"/>
               = <label id="result"></label><br/><br/>
              <button onclick="calculate()">計算</button>
              ```

6.BMI計算
```
bmi計算<br>
    <center><table border="10">
            <tr>
            <th></th>
            <th>BMI值(kg/m2)</th>
            </tr>
            <tr>
            <th>體重過輕</th>
            <td>BMI ＜ 18.5</td>
            </tr>
            <tr>
            <th>正常範圍</th>
            <td>18.5≦BMI＜24</td>
            </tr>
            <tr>
            <th>異常範圍</th>
            <td>過重：24≦BMI＜27<br>
                輕度肥胖：27≦BMI＜30<br>
                中度肥胖：30≦BMI＜35<br>
                重度肥胖：BMI≧35<br>
            </td>	
            </tr>	
        </table></center>
    身高(m): <input type="text"  id="box1" value=""><br>
    體重(kg): <input type="text"  id="box2" value=""><br>	
    <input type="button" value="重置" onClick="reset()">
    <input type="button" value="計算" onClick="equal()"><br>
	您的BMI值為:<input type="text" name="height" id="box3" value="">
	<script>
            function equal(){
            x = document.getElementById("box1").value;
            y = document.getElementById("box2").value;
            z = y/(x*x);
            document.getElementById("box3").value = parseFloat(z.toFixed(2));
            }
            function reset(){
            document.getElementById("box1").value="";
            document.getElementById("box2").value="";
            document.getElementById("box3").value="";
            }
		
   </script>
   ```
