# three-js-hello-world-cube
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
