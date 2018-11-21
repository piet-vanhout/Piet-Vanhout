<html xmlns="http://www.w3.org/1999/xhtml"><head>
<title>Aframe Environments</title>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<script src="https://aframe.io/releases/0.7.0/aframe.min.js"></script>
<script src="https://cdn.rawgit.com/feiss/aframe-environment-component/ad57b15d/dist/aframe-environment-component.min.js"></script>
<script src="https://unpkg.com/aframe-event-set-component@^4.0.0/dist/aframe-event-set-component.min.js"></script>

</head>
<body class="a-body ">

<!-- Opgave opdracht 
Vul dit Aframe bestand verder aan zoals in het voorbeeld (filmpje)
- foto (image) toevoegen
- sneeuwman afwerken (lichaam, hoofd met ogen en neus)
- Tekst "VR sneeuwman" in het midden zetten (zoals in het filmpje)
- hyperlink naar "wiki met sneeuwman"
- (vrijblijvend: texture rond box met hyperlink )
-->


<a-scene effects="bloom, fxaa" bloom="radius: 0.25" fxaa="" class="fullscreen" inspector="" keyboard-shortcuts="" screenshot="" vr-mode-ui="" fog="color:#899396;far:92"><canvas class="a-canvas" data-aframe-canvas="true" width="300" height="150"></canvas>
<a-assets> 
<img id="foto" src="sneeuwman.JPG">
<img id="brick_bump" src="https://aframe.io/sample-assets/assets/images/bricks/brick_bump.jpg" crossorigin="anonymous"><img id="brick_bump" src="https://aframe.io/sample-assets/assets/images/bricks/brick_bump.jpg" crossorigin="anonymous"><img id="sneeuwman" src="https://ucarecdn.com/f31e9161-2226-4fc5-8d23-819d89444f9f/" crossorigin="anonymous"></a-assets> 

<!-- Camera -->
<a-camera position="-4.055335739753037 1.6 -14.37515065839035" rotation="19.709748152500318 178.30446584471215 0" camera="" look-controls="" wasd-controls="" data-aframe-inspector-original-camera="">
<a-entity cursor="fuse:true;fuseTimeout:1000" position="0 0 -1" geometry="primitive:sphere;radius:0.005" material="color:#FF0000;shader:flat;opacity:0.5" raycaster="">
<a-animation attribute="scale" to="3 3 3" dur="1000" begin="cursor-fusing" fill="backwards" easing="linear">
</a-animation>
</a-entity>
</a-camera>


<!-- landschap -->
<a-entity id="env1" environment="skyType:atmosphere;skyColor:#0d0d0d;horizonColor:#404040;lightPosition:1.08 2.94 0.95;flatShading:true;groundYScale:4.81;groundTexture:checkerboard;groundColor:#252525;groundColor2:#111111;dressing:cubes;dressingColor:#9f9f9f;dressingScale:1.51;dressingVariance:5 20 5;grid:dots;shadow:true;preset:checkerboard"><a-entity position="0 50 0" light="intensity:0.549;groundColor:#252525;type:hemisphere;color:#CEE4F0"></a-entity><a-entity position="-1.804 3.452 1.452" light="intensity:0.549;castShadow:true;shadowCameraLeft:-10;shadowCameraBottom:-10;shadowCameraRight:10;shadowCameraTop:10" scale="1.19 1 1"></a-entity><a-entity rotation="-90 0 0" scale="1 1 4.81" shadow="cast:false" position="-1.63 0.064 0.497"></a-entity><a-entity></a-entity><a-sky radius="200" geometry="" theta-length="110" material="sunPosition:0.33 0.898 0.29;shader:skyshader"></a-sky><a-entity id="stars"></a-entity></a-entity>

<!-- foto -->


<!-- sneeuwman -->

<a-sphere id="oog" position="-3.815 5.366 -7.61" radius="1.25" color="white" material="color:#000000;transparent:true" shadow="" scale="-0.06000000000000009 0.04999999999999992 0.06000000000000004"></a-sphere><a-sphere id="oog" position="-5.41 5.332 -7.473" radius="1.25" color="white" material="color:#000000;transparent:true" shadow="" scale="-0.06000000000000009 0.04999999999999992 0.06000000000000004"></a-sphere><a-sphere id="bol-4" position="-4.563 2.964 -8.965" radius="1.25" color="white" shadow=""></a-sphere><a-sphere id="bol-3" position="-4.578 4.924 -8.781" radius="1.25" color="white" shadow=""></a-sphere><a-sphere id="onderste bol-2" position="-4.496 1.126 -8.792" radius="1.25" color="white" shadow=""></a-sphere>

<a-cone id="hoed" color="brown" radius-bottom="1" radius-top="0" position="-4.986 6.484 -9.239" rotation="-11 -3 15" material="color:#804000" geometry="" shadow=""></a-cone><a-cone id="neus" color="brown" radius-bottom="1" radius-top="0" position="-4.587 5.103 -7.384" rotation="90.38 -2.71 -6.91" material="color:#ff8040" shadow="" scale="0.45 1.03 0.27"></a-cone>



<!-- tekst -->
<a-entity id="tekst" data-brackets-id="272" text="color:#ff0080;value:VR sneeuwman;anchor:left;width:2" position="0.174 3.724 -2.309" scale="14.879999999999999 11.58 -4.38"></a-entity>


<!-- box link naar website --> 
<a-entity id="box met weblink" mixin="col1" geometry="" position="4 0.577 -7" material="shader:flat;side:double;color:#777777;src:[object HTMLImageElement]" event-set__enter="[object Object]" event-set__leave="[object Object]" onclick="location.href='https://www.google.be/search?q=sneeuwman'">
</a-entity>

<a-entity id="link" text="anchor:left;color:#00ff00;value:link;width:3.51" position="3.7 0.8 -6.48"></a-entity>
<a-entity id="wiki" text="anchor:left;color:#00ff00;value:Wiki;width:3.51" position="3.7 0.6 -6.48"></a-entity>
<a-entity id="Sneeuwman" text="anchor:left;color:#00ff00;value:Sneeuwman;width:3.51" position="3.5 0.4 -6.48">
</a-entity>




</a-scene>

<a href="blob:file:///668afa79-1c2f-490e-9395-e3b4f8c423b6" download="c-users-piet-vanhout-documents-sneeuwman-html" style="display: none;"></a><a href="blob:file:///05d5c61b-9d8a-4715-a13a-1eef8221de1b" download="c-users-piet-vanhout-documents-sneeuwman-html" style="display: none;"></a></body></html>
