<link
	rel="stylesheet"
	href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
	integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
	crossorigin=""
/>

<!-- Make sure you put this AFTER Leaflet's CSS -->
<script
	src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
	integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
	crossorigin=""
></script>

## 律师名片

!!! tip "Kathy Zhang - Jade Sunrise Law"
	**地址:** 500-1110 Centre Street NE Calgary, AB T2E 2R2 <br>
	**电话:** [1 (403) 456-3977](tel:4034563977)<br>
	**传真:** 1(844) 272-3932<br>
	**Email:** [info@jadesunriselaw.com](mailto:info@jadesunriselaw.com)<br>

## 办公地址

按空格键或刷新页面，显示地图

<div id="map" style="height: 320px"></div>
<script src="../../assets/js/leaf-map.js"></script>

<script> 
document.addEventListener("keydown", (e)=>{
	// console.log(e.keyCode);
	if (e.keyCode == 32 ) document.location.reload()});
</script>
