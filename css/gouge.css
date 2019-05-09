$(function(){
	//当js_number被选中
	var lj_number1="0";
	
	//数字操作
	$(".js_number").click(function(){
//		console.log(this.innerText)
		//将数值打印到显示框
		if(lj_number1==="0"){
			lj_number1=this.innerText;
		}else{
			lj_number1+=this.innerText;
		}
		$(".content").text(lj_number1);
	})
	
	//为零操作
	$(".weiling").click(function(){
		$(".content").text(0);
		lj_number1="0";
	})
	
	//一般运算操作
	$(".yiban").click(function(){
		//将值转化为number
//		console.log(this.innerText);
		if(lj_number1[lj_number1.length-1]=="+"||lj_number1[lj_number1.length-1]=="*"||lj_number1[lj_number1.length-1]=="-"||lj_number1[lj_number1.length-1]=="/"){
			//替换掉最后一位
			lj_number1=lj_number1.substring(0,lj_number1.length-1)+this.innerText;
			$(".content").text(lj_number1);			
//			return false;
		}else{
			lj_number1+=this.innerText;
			$(".content").text(lj_number1);	
		}
//		console.log(lj_number1[lj_number1.length-2]);
	})
	

	//dian运算操作
	$(".dian").click(function(){
		//将值转化为number
//		console.log(this.innerText);
//		console.log(lj_number1.indexOf("."));
		if(lj_number1[lj_number1.length-1]=="+"||lj_number1[lj_number1.length-1]=="*"||lj_number1[lj_number1.length-1]=="-"||lj_number1[lj_number1.length-1]=="/"){
			//替换掉最后一位
			$(".content").text("错误");		
			lj_number1="0";
		}else{	
			if(lj_number1[lj_number1.length-1]=="."){
				//文本里存在点的情况  不变 不生效
				return false;
			}else{
				lj_number1+=this.innerText;
				$(".content").text(lj_number1);
			}
		}
	})
	
	//百分比操作
	$(".baifen").click(function(){
		if(lj_number1[lj_number1.length-1]=="+"||lj_number1[lj_number1.length-1]=="*"||lj_number1[lj_number1.length-1]=="-"||lj_number1[lj_number1.length-1]=="/"){
			//替换掉最后一位
			$(".content").text("错误");
			lj_number1="0";
		}else{	
			$(".content").text(lj_number1/100);
			//lj_number1也跟着变化
			lj_number1=lj_number1/100;
		}
	})
	
	//去位操作
	$(".quwei").click(function(){
		$(".content").text(lj_number1.substring(0,lj_number1.length-1));
		lj_number1=lj_number1.substring(0,lj_number1.length-1);
	})
	
	//等号操作
	$(".denghao").click(function(){
		var $jieguo=eval($(".content").text());
		//数值进行计算
		$(".content").text($jieguo);
		//将lj_number进行更新
//		console.log($jieguo);
		lj_number1=$jieguo.toString();
//		console.log(lj_number1)
	})
	
	
	//时针  让span透明度变化
	setInterval(function(){
		$("span").css("opacity",1);
		setTimeout(function(){
			$("span").css("opacity",0)
		},900);
	},1800)

	
})
