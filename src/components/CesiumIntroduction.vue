<template>
  <el-scrollbar height="86%" style="margin-left:2%;">
   <div> 
    <el-card style="background-image:url('/前端页面资源/bgc/bgcMain7.gif');min-width:220px;max-width: 220px;float:right;margin-right:2%;margin-top:50px;background-color:#363434;width:30%">
    <template #header><p>Cesium.JS介绍</p></template>
    <img
      src="/前端页面资源/CesiumIcon2.png"
      style="width: 100%;opacity:0.6"
    />
  <el-card style="background-image:url('/前端页面资源/bgc/bgcMain4.gif');max-width: 300px;background-color:#363434;">
    <p><a style="color:yellow;" href="http://cesium.xin/cesium/cn/Documentation1.95/index.html" target="_blank">Cesium.JS手册</a></p>
  </el-card>
  </el-card>
  <h1 id="about">Cesium.JS介绍</h1>
<div id="text" style="margin-right: 260px;">
  <p id="textP" style=" line-height: 1.6">
    Cesium 可以在多种操作系统和浏览器上运行,无需额外的插件支持,前提是浏览器支持 WebGL。
支持 Windows、Linux、macOS 以及 iOS 等多种平台。通过 WebGL 进行硬件加速,
Cesium 能够高效渲染复杂的 3D 图形,提供高精度的地理空间分析能力。支持大规模数据集的可视化和分析。
支持多种数据格式,包括 3D Tiles、glTF、KML 等,能够高效加载和渲染大规模的三维模型和地形数据。
支持 2D、2.5D 和 3D 地图展示,提供多种地图和地形图层选择。
提供地址搜索、信息窗口、全屏查看以及 WebVR 支持等交互功能。
支持基于时间轴的动态数据展示,适用于实时监控和历史回放等场景。
Cesium 广泛应用于多个领域,包括但不限于:

地理信息系统(GIS):用于创建交互式地图和地理数据可视化应用。
城市规划与交通管理:帮助进行城市设计和交通流量模拟。
航空航天与无人机应用:用于模拟飞行路径和无人机监控。
虚拟现实(VR)和增强现实(AR):提供沉浸式的地理空间数据体验。

Cesium 的设计理念是为开发者提供一个强大的平台,用于创建交互式、动态的地理空间应用,满足现代 Web 应用的需求。
  </p>

</div>
<br>
<h1 id="about" >Cesium.JS与GIS结合</h1>
<div id="text" style="margin-right: 3%;">
  <p id="textP" style=" line-height: 1.6">
    Cesium支持多种GIS数据格式,如GeoJSON、KML、3D Tiles等。这使得开发者可以轻松加载和处理来自不同来源的地理数据。
  
Cesium引入了3D Tiles格式,用于高效加载和渲染大规模的三维模型和地形数据。这种格式特别适用于需要处理大量地理数据的GIS应用。

Cesium提供了ImageryLayer、ImageryProvider和ImageryLayerCollection等类,用于加载和管理影像图层。这些图层可以来自不同的GIS服务,如ArcGIS、Bing Maps等。

支持加载矢量数据,如矢量地图服务(WMTS),这对于需要显示详细地理信息的应用非常有用。

Cesium支持基于时间轴的动态数据展示,适用于实时监控和历史数据回放。这在GIS应用中非常常见,尤其是在交通管理、城市规划和环境监测等领域。

Cesium提供了丰富的地理空间分析功能,如距离测量、面积计算等,帮助用户进行深入的空间分析。

Cesium可以与Vue.js、React等现代Web框架无缝集成,允许开发者构建复杂的GIS应用。

Cesium支持插件和扩展,开发者可以通过这些工具扩展其功能,以满足特定的应用需求。

Cesium的3D可视化能力使其成为城市规划、交通流量模拟和应急响应的理想选择。
  
通过实时数据展示和地理空间分析,Cesium可以帮助进行环境监测和灾害预警。

Cesium在数字孪生和虚拟现实应用中也有广泛应用,提供沉浸式的地理空间体验。

Cesium与GIS的结合为开发者提供了一个强大的平台,用于创建功能丰富、交互性强的地理空间应用,满足现代Web应用的需求。
  </p>

</div>
<br>
<h1 id="about">Cesium.JS学前基础</h1>
<div id="text" style="margin-right: 3%;">
   <p id="textP" style="line-height: 1.6" >
    1.Web开发基础:
Cesium.js 是一个基于JavaScript的库,因此需要掌握HTML、CSS和JavaScript的基本知识。了解如何构建网页、样式设计和JavaScript编程是学习Cesium的基础。
理解文档对象模型(DOM)以及如何使用JavaScript操作DOM元素,这对于Cesium.js的交互功能至关重要。

2. WebGL基础:
图形渲染: Cesium.js 使用WebGL进行图形渲染,因此对WebGL的基本概念有一定了解会有所帮助。了解WebGL如何与GPU交互进行图形渲染的基本原理。
3D图形基础: 了解3D图形的基本概念,如坐标系、变换矩阵、投影等。

3. GIS基础:
地理信息系统(GIS): 了解GIS的基本概念和数据格式,如GeoJSON、KML、3D Tiles等,这些数据格式在Cesium.js中经常使用。
地图投影: 理解地图投影的基本原理,如WGS84坐标系,这对于在Cesium.js中处理地理数据非常重要。

4. 开发工具与环境:
Node.js和npm: 熟悉Node.js和npm(或pnpm)的基本使用,因为Cesium.js项目通常使用这些工具进行包管理和构建。
版本控制: 了解Git等版本控制工具的基本操作,以便在开发过程中管理代码。

5. 其他相关技术:
Web框架: 了解如何使用Vue.js、React等现代Web框架与Cesium.js集成,可以帮助你构建复杂的应用。
性能优化: 了解基本的Web性能优化技巧,因为Cesium.js处理的是大量地理数据,优化性能是一个重要方面。
在学习Cesium.js之前,建议先掌握Web开发的基础知识,并对WebGL和GIS有一定的了解。此外,熟悉开发工具和环境以及相关技术（如Web框架和性能优化）将有助于更有效地学习和使用Cesium.js。通过这些基础知识的学习，你可以更好地理解和应用Cesium.js的功能和特性。
   </p>

</div>
    </div>
    
  <div style="width: 100%;height:100%;position:absolute;left:0px;top:0px;z-index:-1">
    <canvas ref="webgl" id='webGL' width="1520" height="888"></canvas>
  </div>
  </el-scrollbar>
</template>

<script setup>

import { onMounted,ref } from 'vue';
const webgl=ref(null)
onMounted(()=>{
const gl=webgl.value.getContext('webgl')
//顶点着色器
const vertexSource=`
attribute vec4 a_pos;
attribute vec2 a_coord;
varying vec2 v_coord;
void main(){
v_coord=a_coord;
gl_Position=a_pos;
}`
//片元着色器
const fragSource=`
// 所有float类型数据的精度是lowp
precision mediump float;
varying vec2 v_coord;
uniform vec2 st;
uniform float u_time;
uniform sampler2D u_sam;
uniform vec2 u_mouse;
// by srtuss, 2013

// rotate position around axis
vec2 rotate(vec2 p, float a)
{
	return vec2(p.x * cos(a) - p.y * sin(a), p.x * sin(a) + p.y * cos(a));
}

// 1D random numbers
float rand(float n)
{
    return fract(sin(n) * 43758.5453123);
}

// 2D random numbers
vec2 rand2(in vec2 p)
{
	return fract(vec2(sin(p.x * 591.32 + p.y * 154.077), cos(p.x * 391.32 + p.y * 49.077)));
}

// 1D noise
float noise1(float p)
{
	float fl = floor(p);
	float fc = fract(p);
	return mix(rand(fl), rand(fl + 1.0), fc);
}

// voronoi distance noise, based on iq's articles
float voronoi(in vec2 x)
{
	vec2 p = floor(x);
	vec2 f = fract(x);
	
	vec2 res = vec2(8.0);
	for(int j = -1; j <= 1; j ++)
	{
		for(int i = -1; i <= 1; i ++)
		{
			vec2 b = vec2(i, j);
			vec2 r = vec2(b) - f + rand2(p + b);
			
			// chebyshev distance, one of many ways to do this
			float d = max(abs(r.x), abs(r.y));
			
			if(d < res.x)
			{
				res.y = res.x;
				res.x = d;
			}
			else if(d < res.y)
			{
				res.y = d;
			}
		}
	}
	return res.y - res.x;
}

void main() {
   float flicker = noise1(u_time * 2.0) * 0.8 + 0.4;

    vec2 uv = gl_FragCoord.xy / st.xy;
	  uv = (uv - 0.5) * 2.0;
	  vec2 suv = uv;
	  uv.x *= st.x / st.y;
	
	
	  float v = 0.0;
	
	//  that looks highly interesting:
	// v = 1.0 - length(uv) * 1.3;
	
	
	// a bit of camera movement
	uv *= 0.6 + sin(u_time * 0.1) * 0.4;
	uv = rotate(uv, sin(u_time * 0.3) * 1.0);
	uv += u_time * 0.4;
	
	
	// add some noise octaves
	float a = 0.6, f = 1.0;
	
	for(int i = 0; i < 3; i ++) // 4 octaves also look nice, its getting a bit slow though
	{	
		float v1 = voronoi(uv * f + 5.0);
		float v2 = 0.0;
		
   	// make the moving electrons-effect for higher octaves
		if(i > 0)
		{
			// of course everything based on voronoi
			v2 = voronoi(uv * f * 0.5 + 50.0 + u_time);
			
			float va = 0.0, vb = 0.0;
			va = 1.0 - smoothstep(0.0, 0.1, v1);
			vb = 1.0 - smoothstep(0.0, 0.08, v2);
			v += a * pow(va * (0.5 + vb), 2.0);
		}
		
	//  make sharp edges
		v1 = 1.0 - smoothstep(0.0, 0.3, v1);
		
	// 	noise is used as intensity map
	 	v2 = a * (noise1(v1 * 5.5 + 0.1));
		
	// 	 octave 0's intensity changes a bit
		if(i == 0)
			v += v2 * flicker;
		else
			v += v2;
		
		f *= 3.0;
		a *= 0.7;
	 }

	// slight vignetting
	v *= exp(-0.6 * length(suv)) * 1.2;

	
	// // old blueish color set
	vec3 cexp = vec3(6.0, 4.0, 2.0);
	
	vec3 col = vec3(pow(v, cexp.x), pow(v, cexp.y), pow(v, cexp.z)) * 2.0;
	
	vec4 fragColor = vec4(col, 1.0);
  gl_FragColor=fragColor;

}
`
//初始化着色器
const program=initShader(gl,vertexSource,fragSource)
//加载纹理
const data=new Float32Array([
    1.0,1.0,1.0,  1.0,1.0,
    -1.0,1.0,1.0, 0.0,1.0,
    -1.0,-1.0,.5,0.0,0.0,
    1.0,1.0,1.0,  1.0,1.0,
    -1.0,-1.0,1.0,0.0,0.0,
    1.0,-1.0,.5, 1.0,0.0   //面1
])
console.log(data.BYTES_PER_ELEMENT);
const pos=gl.getAttribLocation(program,'a_pos')
const uv=gl.getAttribLocation(program,'a_coord')
const sam=gl.getUniformLocation(program,'u_sam')
const buffer=gl.createBuffer()
gl.bindBuffer(gl.ARRAY_BUFFER,buffer)
gl.bufferData(gl.ARRAY_BUFFER,data,gl.STATIC_DRAW)
gl.vertexAttribPointer(pos,3,gl.FLOAT,false,4*5,0)
gl.enableVertexAttribArray(pos)
gl.vertexAttribPointer(uv,2,gl.FLOAT,false,4*5,4*3)
gl.enableVertexAttribArray(uv)
//创建纹理图片
const img=new Image()
img.src='/../webGL资源/科比.jpg'
img.onload=()=>{
const texture=gl.createTexture()
gl.activeTexture(gl.TEXTURE0)
gl.bindTexture(gl.TEXTURE_2D,texture)
gl.pixelStorei(gl.UNPACK_FLIP_Y_WEBGL, true);
//设置纹理贴图填充方式(纹理贴图像素尺寸大于顶点绘制区域像素尺寸)
gl.texParameteri(gl.TEXTURE_2D, gl.TEXTURE_MIN_FILTER, gl.LINEAR);
//设置纹理贴图填充方式(纹理贴图像素尺寸小于顶点绘制区域像素尺寸)
gl.texParameteri(gl.TEXTURE_2D, gl.TEXTURE_MAG_FILTER, gl.LINEAR);
//设置纹素格式，jpg格式对应gl.RGB
gl.texImage2D(gl.TEXTURE_2D, 0, gl.RGB, gl.RGB, gl.UNSIGNED_BYTE, img);
gl.uniform1i(sam, 0);//纹理缓冲区单元TEXTURE0中的颜色数据传入片元着色器
// gl.getProgramInfoLog(program);
//开启深度测试
gl.enable(gl.DEPTH_TEST)
gl.drawArrays(gl.TRIANGLES,0,6)
}
//把画布坐标传给他
const xy=gl.getUniformLocation(gl.program,'st')
gl.uniform2f(xy,window.innerWidth,window.innerHeight)
//鼠标位置
webgl.value.addEventListener('mousemove',(e)=>{
const X=e.offsetX
const Y=-e.offsetY+670
//把X,Y坐标传给着色器
const mouse=gl.getUniformLocation(gl.program,'u_mouse')
gl.uniform2f(mouse,X,Y)

})
//传入时间
const time=gl.getUniformLocation(gl.program,'u_time')
let Time=0;
function loop(){
    Time+=0.02;
    gl.uniform1f(time,Time)
    requestAnimationFrame(loop)
    gl.drawArrays(gl.TRIANGLES,0,6)
}
loop()
})
function initShader(gl,vertexSource,fragSource){
const program=gl.createProgram()
const vsShader=gl.createShader(gl.VERTEX_SHADER)
const fsShader=gl.createShader(gl.FRAGMENT_SHADER)
gl.shaderSource(vsShader,vertexSource)
gl.shaderSource(fsShader,fragSource)
gl.compileShader(vsShader)
gl.compileShader(fsShader)
gl.attachShader(program,vsShader)
gl.attachShader(program,fsShader)
gl.linkProgram(program)
gl.useProgram(program)
gl.program=program
return program
}

</script>

<style scoped>
p{
  color: rgb(255, 255, 255);
  font-family:'cursive';
   text-shadow:
    1px 1px 2px black,
    0 0 1em blue,
    0 0 0.2em blue;
  font:
    1.2em Georgia,
    "Bitstream Charter",
    "URW Bookman L",
    "Century Schoolbook L",
    serif;
}
#text{
  margin-left: 20px;
  color: rgb(0, 255, 204);
  font-family:'cursive';
   text-shadow:
    1px 1px 2px black,
    0 0 2em rgb(255, 255, 255),
    0 0 2.2em rgb(86, 245, 0);
  font:
    1.2em Georgia,
    "Bitstream Charter",
    "URW Bookman L",
    "Century Schoolbook L",
    serif;

  box-shadow: 0px 5px 10px  rgb(4, 218, 218) ,0px -5px 10px  rgb(7, 235, 220); 
opacity: 0.8;
margin-top: 10px;
border-radius: 10px;

}

#about{
  margin-left: 20px;
    color: rgb(91, 253, 4);
    font-family:'cursive';
   text-shadow:
    1px 1px 2px black,
    0 0 2.1em rgb(236, 22, 22),
    0 0 1.2em rgb(255, 255, 255);
  font:
    2.0em Georgia,
    "Bitstream Charter",
    "URW Bookman L",
    "Century Schoolbook L",
    serif;
}
#textP{
    color: rgb(0, 251, 255);

text-shadow:
    1px 1px 2px black,
    0 0 2em rgb(255, 255, 255),
    0 0 2.2em rgb(86, 245, 0);
 
font: bold small-caps italic 1.0em 'Roboto', Courier, monospace;
 
  box-shadow: 0px 5px 10px  rgba(2, 95, 255, 0.708) ,0px -5px 10px  rgba(2, 95, 255, 0.708); 
opacity: 0.9;
margin-top: 10px;
border-radius: 10px;
}
</style>