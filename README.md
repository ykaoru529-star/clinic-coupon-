<!DOCTYPE html>

<html lang="ja">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>クーポン管理</title>

<style>

body{

font-family:sans-serif;

background:#f5f7f9;

padding:20px;

}

.container{

max-width:400px;

margin:auto;

background:white;

padding:24px;

border-radius:20px;

box-shadow:0 4px 10px rgba(0,0,0,0.08);

}

h1{

font-size:24px;

margin-bottom:20px;

text-align:center;

}

input{

width:100%;

padding:14px;

margin-bottom:16px;

border:1px solid #ddd;

border-radius:12px;

font-size:16px;

box-sizing:border-box;

}

button{

width:100%;

padding:14px;

border:none;

background:#4CAF50;

color:white;

font-size:16px;

border-radius:12px;

}

.result{

margin-top:20px;

padding:16px;

background:#eef7ee;

border-radius:12px;

display:none;

}

</style>

</head>

<body>

<div class="container">

<h1>無料クーポン</h1>

<input type="text" id="coupon" placeholder="クーポンコード">

<input type="text" id="name" placeholder="患者様名">

<button onclick="submitCoupon()">

クーポンを使用する

</button>

<div class="result" id="result">

クーポンを受け付けました。

</div>

</div>

<script>

function submitCoupon(){

const coupon =

document.getElementById("coupon").value;

const name =

document.getElementById("name").value;

if(coupon === "" || name === ""){

alert("入力してください");

return;

}

document.getElementById("result").style.display="block";

}

</script>

</body>

</html>