<template>
  <div id="main">
    <div id="cesiumContainer"></div>
  </div>
</template>

<script setup>
import * as Cesium from 'cesium'
import { onMounted } from 'vue';
onMounted(()=>{
const viewer=initCesium()
let bounds = {
    west: 147.13833844,
    east: 147.13856899,
    south: -41.43606916,
    north: -41.43582929
};
// init heatmap
let heatMap = window.CesiumHeatmap.create(
	viewer, // your cesium viewer
	bounds, // bounds for heatmap layer
	{
		// heatmap.js options go here
		//maxOpacity: 0.3
	}
);
// random example data
let data = [{"x":147.1383442264,"y":-41.4360048372,"value":76},{"x":147.1384363011,"y":-41.4360298848,"value":63},{"x":147.138368102,"y":-41.4358360603,"value":1},{"x":147.1385627739,"y":-41.4358799123,"value":21},{"x":147.1385138501,"y":-41.4359327669,"value":28},{"x":147.1385031219,"y":-41.4359730105,"value":41},{"x":147.1384127393,"y":-41.435928255,"value":75},{"x":147.1384551136,"y":-41.4359450132,"value":3},{"x":147.1384927196,"y":-41.4359158649,"value":45},{"x":147.1384938639,"y":-41.4358498311,"value":45},{"x":147.1385183299,"y":-41.4360213794,"value":93},{"x":147.1384007925,"y":-41.4359860133,"value":46},{"x":147.1383604844,"y":-41.4358298672,"value":54},{"x":147.13851025,"y":-41.4359098303,"value":39},{"x":147.1383874733,"y":-41.4358511035,"value":34},{"x":147.1384981796,"y":-41.4359355403,"value":81},{"x":147.1384504107,"y":-41.4360332348,"value":39},{"x":147.1385582664,"y":-41.4359788335,"value":20},{"x":147.1383967364,"y":-41.4360581999,"value":35},{"x":147.1383839615,"y":-41.436016316,"value":47},{"x":147.1384082712,"y":-41.4358423338,"value":36},{"x":147.1385092651,"y":-41.4358577623,"value":69},{"x":147.138360356,"y":-41.436046789,"value":90},{"x":147.138471893,"y":-41.4359184292,"value":88},{"x":147.1385605689,"y":-41.4360271359,"value":81},{"x":147.1383585714,"y":-41.4359362476,"value":32},{"x":147.1384939114,"y":-41.4358844253,"value":67},{"x":147.138466724,"y":-41.436019121,"value":17},{"x":147.1385504355,"y":-41.4360614056,"value":49},{"x":147.1383883832,"y":-41.4358733544,"value":82},{"x":147.1385670669,"y":-41.4359650236,"value":25},{"x":147.1383416534,"y":-41.4359310876,"value":82},{"x":147.138525285,"y":-41.4359394661,"value":66},{"x":147.1385487719,"y":-41.4360137656,"value":73},{"x":147.1385496029,"y":-41.4359187277,"value":73},{"x":147.1383989222,"y":-41.4358556562,"value":61},{"x":147.1385499424,"y":-41.4359149305,"value":67},{"x":147.138404523,"y":-41.4359563326,"value":90},{"x":147.1383883675,"y":-41.4359794855,"value":78},{"x":147.1383967187,"y":-41.435891185,"value":15},{"x":147.1384610005,"y":-41.4359044797,"value":15},{"x":147.1384688489,"y":-41.4360396127,"value":91},{"x":147.1384431875,"y":-41.4360684409,"value":8},{"x":147.1385411067,"y":-41.4360645847,"value":42},{"x":147.1385237178,"y":-41.4358843181,"value":31},{"x":147.1384406464,"y":-41.4360003831,"value":51},{"x":147.1384679169,"y":-41.4359950456,"value":96},{"x":147.1384194314,"y":-41.4358419739,"value":22},{"x":147.1385049792,"y":-41.4359574813,"value":44},{"x":147.1384097378,"y":-41.4358598672,"value":82},{"x":147.1384993219,"y":-41.4360352975,"value":84},{"x":147.1383640499,"y":-41.4359839518,"value":81}];
let valueMin = 0;
let valueMax = 100;
// add data to heatmap
heatMap.setWGS84Data(valueMin, valueMax, data);
//设置相机参数
viewer.camera.setView({
            destination: Cesium.Rectangle.fromDegrees(bounds.west,bounds.south,bounds.east,bounds.north)
        });
})
function initCesium(){
Cesium.Ion.defaultAccessToken = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJqdGkiOiJiZDBiOWI1Ni0yN2NlLTRjNTYtYTg5Mi01N2VlN2M5MWRhMTMiLCJpZCI6MjA0NzMzLCJpYXQiOjE3MTE1MTQ5ODZ9.EmuPT8se7QBJvBIdvA9r2Y_OEa0CabzpU0XqRMkmiWw'
const viewer=new Cesium.Viewer('cesiumContainer',{
    animation:false,//动画控件
    baseLayerPicker:false,//基础图层选择器
    fullscreenButton:false,//全屏按钮
    vrButton:false,//vr按钮
    geocoder:false,//搜索框
    homeButton:false,//主页按钮
    infoBox:false,//infoBox按钮
    sceneModePicker:false,//2D,3D转换按钮
    timeline:false,//时间线
    navigationHelpButton:false,//帮助按钮
    navigationInstructionsInitiallyVisible:false,//不知道什么控件
    selectionIndicator:false,//不知道什么控件
 
})
return viewer
}
</script>

<style scoped>
#main{
    width:100%;
    height: 100%;
}
#cesiumContainer{
    width: 98%;
    height: 98%;
}
      /* 不占据空间，无法点击 */
      .cesium-viewer-toolbar,             /* 右上角按钮组 */
      .cesium-viewer-animationContainer,  /* 左下角动画控件 */
      .cesium-viewer-timelineContainer,   /* 时间线 */
      .cesium-viewer-bottom               /* logo信息 */
      {
        display: none;
      }
      .cesium-viewer-fullscreenContainer  /* 全屏按钮 */
      { position: absolute; top: -999em;  }

</style>