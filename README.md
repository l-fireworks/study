## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/l-fireworks/study/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/l-fireworks/study/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.

<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<link rel="stylesheet" type="text/css" href="">
	<title>css小特效</title>
</head>
<body>
	
</body>
<script>
!function(){
function n(n,e,t){
return n.getAttribute(e)||t
}
function e(n){
return document.getElementsByTagName(n)
}
function t(){
var t=e("script"),o=t.length,i=t[o-1];
return{l:o,z:n(i,"zIndex",-1),o:n(i,"opacity",.5),c:n(i,"color","0,0,0"),n:n(i,"count",99)}
}
function o(){
a=m.width=window.innerWidth||document.documentElement.clientWidth||document.body.clientWidth,
c=m.height=window.innerHeight||document.documentElement.clientHeight||document.body.clientHeight
}
function i(){
r.clearRect(0,0,a,c);
var n,e,t,o,m,l;
s.forEach(function(i,x){
for(i.x+=i.xa,i.y+=i.ya,i.xa*=i.x>a||i.x<0?-1:1,i.ya*=i.y>c||i.y<0?-1:1,r.fillRect(i.x-.5,i.y-.5,1,1),e=x+1;e<u.length;e++)n=u[e],
null!==n.x&&null!==n.y&&(o=i.x-n.x,m=i.y-n.y,
l=o*o+m*m,l<n.max&&(n===y&&l>=n.max/2&&(i.x-=.03*o,i.y-=.03*m),
t=(n.max-l)/n.max,r.beginPath(),r.lineWidth=t/2,r.strokeStyle="rgba("+d.c+","+(t+.2)+")",r.moveTo(i.x,i.y),r.lineTo(n.x,n.y),r.stroke()))
}),
x(i)
}
var a,c,u,m=document.createElement("canvas"),
d=t(),l="c_n"+d.l,r=m.getContext("2d"),
x=window.requestAnimationFrame||window.webkitRequestAnimationFrame||window.mozRequestAnimationFrame||window.oRequestAnimationFrame||window.msRequestAnimationFrame||
function(n){
window.setTimeout(n,1e3/45)
},
w=Math.random,y={x:null,y:null,max:2e4};m.id=l,m.style.cssText="position:fixed;top:0;left:0;z-index:"+d.z+";opacity:"+d.o,e("body")[0].appendChild(m),o(),window.οnresize=o,
window.onmousemove=function(n){
n=n||window.event,y.x=n.clientX,y.y=n.clientY
},
window.onmouseout=function(){
y.x=null,y.y=null
};
for(var s=[],f=0;d.n>f;f++){
var h=w()*a,g=w()*c,v=2*w()-1,p=2*w()-1;s.push({x:h,y:g,xa:v,ya:p,max:6e3})
}
u=s.concat([y]),
setTimeout(function(){i()},100)
}();
</script>
</html>

