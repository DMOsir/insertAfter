/**
 * 把一个节点插入到另外一个节点之后
 */

function insertAfter(newElement,targetElement){
	//获取它的父元素
	var parent = targetElement.parentNode;
	//如果指定元素是最后一个元素
	if(parent.lastChild == targetElement ) {
	//把它插入进父元素的子元素之中
		parent.appendChild(newElement);
	}else{
		//把新元素插入到目标元素和目标元素的下一个兄弟元素之间
		parent.insertBefore(newElement,targetElement.nextSibling);
		
	}
}
