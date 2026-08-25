1 index.html
<!Doctype html>
               <html lang="sw">
               <head >
<meta charset="utf-8">
< meta name="viewport">
content="width=device-width,initial- scale=1.0>
<title >mazao yetu<\title><head><body>
<h1>MAZAO YETU<\h1>
< p> karibu kwenye soko la mazao
< body<\html>

2 style.css

*{box- sizing; border - box;}
body { margin:0; fort-family: Arial,sans-serig; 
background:#f4f7f2;
color:#222;

header{background;#2 e7d32;
color: white;
textalign: center; 
padding:2px 15px;}

header h1{ margin:00 8px}
main{ max- width:700px;
margin: auto;
padding:20px}

section {background: white; margin- bottom:18px
padding: 18px 
box-shadow:0 2px 8px rgba (0,0,0,0.08}

product {border:1px solid #ddd;
border-radius: 10px; 
padding: 15px;
margin-bottom:12px}

product h3{margin-top:0
font-weight: bold;}

#callbutton{display: inline-block;
background:#2e7d32;
color: white;
text-decoration: green;
padding:12px 20px;
border-radius: 8px;
margin-top: 8px;}

footer{text-align: center;
padding:20px;
color:#666;


3 Products.js
const product=[{name: "Mchele",
price:2000,
unit: "kg"}{name="maharage",
price:2500
unit:kg}{name: "mahindi"
price:550
unit:"kg"}]


4 script.js 
const products container=document.getelementById("products");
const location Element ById("location");
const phoneElement= document. getElementById("phone");
const call button=document.getElementById("call button");

location Element. text content= appconfig location;
phoneElement.textcontent=appconfig.phone;

call button.href="tel;"+
appconfig. phone.split("/")[ 0];

products.for Each(product=>{ const productsDvi= document.creatElement(" dvi"); productDvi.
class name= "product"

let price text=product.price> 0
?Tsh$
{ product.price.tolocalestring(0)}|${ product.unit}
:" bei inapatikana kwa mawasiliano";
productDvi.innerHTML=< h3> $ { product.name} <\ h3>
< p class= " price"> ${ price text}<\ p>

products container.appendchild( productDvi);})


5 config.js
const appconfig={ location:" Kaliua, Tabora, Tanzania ",
phone 22569118543/225753538623"};