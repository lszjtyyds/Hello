# Hello

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<style type="text/css">
			ul {
				background: olive;
				padding: 20px;
			}

			li {
				background: steelblue;
				margin: 20px;
			}
		</style>
	</head>
	<body>

		<ul id="ulist">
			<li>11111<button>删除</button></li>
			<li>22222<button>删除</button></li>
			<li>33333<button>删除</button></li>
			<li>44444<button>删除</button></li>
			<li>55555<button>删除</button></li>

		</ul>

		<script type="text/javascript">
			var aBtn = document.getElementsByTagName("button")
			var oUl = document.getElementById("ulist")
			var aLi = document.getElementsByTagName("li")

			// aBtn[0].onclick = function() {
			// 	oUl.removeChild(this.parentNode)
			// }
			// aBtn[1].onclick = function() {
			// 	oUl.removeChild(this.parentNode)
			// }
			// aBtn[2].onclick = function() {
			// 	oUl.removeChild(this.parentNode)
			// }
			// aBtn[3].onclick = function() {
			// 	oUl.removeChild(this.parentNode)
			// }
			// aBtn[4].onclick = function() {
			// 	oUl.removeChild(this.parentNode)
			// }
			
			for (var i=0;i<aLi.length;i++) {
				aBtn[i].onclick = function() {
					// oUl.removeChild(this.parentNode)
					this.parentNode.style.display='none'
				}
			}  
		</script>
	</body>
</html>
