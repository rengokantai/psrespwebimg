#### psrespwebimg
######42 picture
```
<picture>
  <source media="(min-width: 600px)" srcset="/images/1.jpg">  <!-- 600+-->
  <source media="(min-width: 300px)" srcset="/images/2.jpg, /images/2x.jpg 2x">  <!-- 300+-->
  <!-- fallback-->
  <img src="/..jpg" srcset="/images/...jpg 2x" alt="">
</picture>
```
######43
######45 picturefill (a github project)
######48 srcset
```
<img src="fallback" sizes="100vw" srcset="1.jpg 256w, 2.jpg 512w" />
```
######50 Client Hints
```
<meta http-equiv="Acctpt-CH" content="DPR, Width">
..
<img src="a.jpg?ch" size="20vw"/>
```
######51 sizes
example: if >900px, then 33vw,otherwise 100vw
```
(min-width: 900px) 33vw,100vw
```
######53 choose physical sizes
responsivebreakpoints.com
######63 HTTP compression
for image formats only support SVG
######68 lazy loading
lazysizes
