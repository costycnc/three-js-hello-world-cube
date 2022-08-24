# three-js-hello-world-cube

Getting starded with three.js

First step to know three

I create https://github.com/costycnc/costycnc-three.js-3d-gcode to understand how working three.js ... so ...

The official source where from my experience i find all examples for advanced or begginer is www.threejs.org ... 

but need install kit on your computer and use a host server if you want run code in your computer locally ...

and  write in mode with includes library like this:

             		<!-- Import maps polyfill -->
		<!-- Remove this when import maps will be widely supported -->
		<script async src="https://unpkg.com/es-module-shims@1.3.6/dist/es-module-shims.js"></script>

		<script type="importmap">
			{
				"imports": {
					"three": "../build/three.module.js"
				}
			}
		</script>

		<script type="module">

			import * as THREE from 'three';

			let camera, scene, renderer;
			let mesh;

			init();
			animate();

as you see all library is located separately one by one in /build/three.module.js 

but in my case if download three.js is in your folder you can run examples without create a local server

like this:

           	<body>

		  <script src="three.js"></script>

		<script>
			
			const scene = new THREE.Scene();
			const camera = new THREE.PerspectiveCamera( 75, window.innerWidth / window.innerHeight, 0.1, 1000 );
			
so is more sample for begginers ... also ... i spend some times to understand differences by them ...

only that three.js contain only some library ... so if you need to add some function like orbitcontrols.js need to insert this script separately 

and not make confusion ... orbitcontrols.js from folder three.js-dev\examples\js\controls is not same as orbitcontrols.js that working with this type of here

so... to working in mode that is in this folder need to find library compatible.

orbitcontrols in this mode seem not be officialy and can not find this on official site threejs.org but only on private members like github like this ...

https://gist.github.com/mrflix/8351020

so i hope that you understand what did and not make confusion...

also all oficial lybraries of threejs can be converted but seem that exists few programmers that realise this until now ...

