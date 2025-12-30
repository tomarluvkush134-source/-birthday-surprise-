# -birthday-surprise-
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Priyanshi</title>
<style>
body{
 margin:0;
 background:#ffd6e8;
 overflow:hidden;
 font-family:'Segoe UI',sans-serif;
}
h1{
 text-align:center;
 margin-top:40vh;
 color:#ff2f7d;
 font-size:28px;
 animation:fade 3s infinite;
}
.balloon{
 position:absolute;
 bottom:-100px;
 width:40px;
 height:55px;
 background:#ff7aa2;
 border-radius:50%;
 animation:float linear infinite;
}
@keyframes float{
 to{transform:translateY(-120vh);}
}
@keyframes fade{
 0%{opacity:0}
 50%{opacity:1}
 100%{opacity:0}
}
.tap{
 position:fixed;
 bottom:20px;
 width:100%;
 text-align:center;
 color:#fff;
 font-size:14px;
}
</style>
</head>
<body onclick="next()">

<h1>Something Beautiful Is Coming For You 💖</h1>
<div class="tap">Tap anywhere 💫</div>

<script>
for(let i=0;i<12;i++){
 let b=document.createElement("div");
 b.className="balloon";
 b.style.left=Math.random()*100+"vw";
 b.style.animationDuration=(4+Math.random()*4)+"s";
 document.body.appendChild(b);
}
function next(){ location.href="countdown.html"; }
</script>

</body>
</html>
