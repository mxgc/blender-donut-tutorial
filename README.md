# Blender Tutorial

## L1
1. g,r,s    grab, rotate, scale; mid-btn snap to three major axes
2. mid-btn  orbiting; pan with shift-mid-btn
3. `key     show different views; view-selected
4. shift-d  duplicate

## L2
1. shit-a   add new object; f9
2. ctrl-a S apply the scale! It's very important. 
3. r-btn    shade smooth/flat
4. tab      edit mode
5. ctrl-tab modes
6. o        proportional editing
7. alt-s    move vertical to the face; move along normal

## L3
1. alt-z    toggle x-ray
2. shift-d  duplicate
3. p        separate    
4. l        select linked
5. mod      subsurf 
6. mod      solidify 
7. z        wireframe mode
8. mod      shift for small increments;
            ctrl for snap to increments

## L4
1. snap     snapping tool; 
            snap to face, project individual elements;
            snap to increments
2. use ref
3. mod      apply mod; usually best to put on top
            subsurf, the viewport level will be applied
4. h/alt-h  hide/unhide
5. e        extrude, add more mesh
6. alt-left click to select edge loop 
7. mod      shrink warp modifier

## L5
1. mod      apply mods
2. layout   sculpting layout
3. ctrl-tab switch mode
4. x        draw; hold ctrl to dig
5. g        grab
6. f        change radius
7. shift-f  change the strength 
8. shift-s  smooth; hold shift to temp activate smooth
9. i        inflate; for sculpting characters

## L6
1. camera   View properties: Lock Camera to View
2. alt-g    snap selected obj to the center of viewport
3. material BSDF
            base color
            roughness
            subsurface scattering
4. render   denoise; viewport start at sample 50

## L7
1. layout   shading; node editor; left to right
2. add      texture -> noise texture
3. ctrl-rb  sever connection
4. add      converter -> colorramp
5. addon    node wrangler to preview node ctrl-shift-left
6. add      texture coordinate
7. shading  bump (normals); change distance

## L8
1. mode     texture paint; x for selecting primary/secondary color
2. shading  image texture
3. shading  mix RGB

## L9
1. geo-node a modifier 
2. geo-node distribute points on faces; poisson disk
3. geo-node join geometry
4. geo-node instance on points
5. apply    scale; rotation
6. geo-node rotate euler; local
7. tau      2 pi
8. mode     weight paint; ctrl-tab
9. geo-node math

## L10
1. ctrl-r   loop cut in edit mode
2. center   point representing center of the mesh
3. geo-node collection info node
4. ctrl-l   link; link materials
5. shading  object info node; random 
6. shading  color ramp

## L11
1. ctrl-p   parenting; select child, then shift-select parent, then ctrl-p to make the child connect to parent
2. output   change resolution and format
3. camera   change focal length; high focal length leads to depth compression 
4. camera   composition guide; center
5. i        insert keyframe
6. playback frame dropping
7. mode     animation
8. editor   graph editor; ctrl-mid-click to zoom; home btn to show everything; ctrl-right-click to add new keyframe; adjust frame timing with bazier curve handles

## L12
1. geo-node point; distribute points on faces
2. geo-node geometry; set position node
3. geo-node random value
4. i        insert keyframe when hovering over any fileds in blender, for example, Offset in Set Position node 
5. i        works on ANY field; change color with animation, etc
6. geo-node value node; #frame for frame info; field turns purple indicating there's a driver there
7. geo-node combine xyz; separating out different components
8. ctrl-j   comment with a node selected; adding a frame
9. geo-node instance on points

## L13 lighting
1. light    primary purpose of lighting is to reveal form; shadow is your friend
2. position top left, top right
3. light    radius down -> sharper shadow
4. light    inverse square law
5. light    fill light to bring out more detail from opposite direction; less power, softer
6. light    world light, env light, all direction, can be set to zero
7. render   color management; look: high or medium high contrast
8. color    spyder x, color accurarcy and luminance
9. reder    color management; view transform: false color; whilte means lost information
10. light   rim light, used to separate the obj from background
11. light   three point lighting: key, fill and rim

## L14 compositing
1. post     compositing, layering, post processing
2. node     ctrl-shift-click on any node; viewer node; turn off backdrop 
3. render   film: check transparent to remove the black background
4. node     RGB color node; alpha over; gradient
5. node     matte
5. node     mix node
6. glare    blur; render pass - glossy direct
7. property layer property; passes; glossy direct, etc
8. node     color balance node; use Offset/Power/Slope
9. node     lens distortion; dispersion: chronamtic aberration; distort: lens barrel effect

## L15 render settings
1. render   sample count; get the least amount of noise in the least amount of time
2. render   denoiser; use optix for viewport; use openimagedenoise for final render
3. render   subsurface scattering is VERY costly
4. render   motion blur checkbox
5. camera   depth of field; change F stop to ~60 since camera is so close to the object
6. render   performance, persistent data
7. render   light paths; clamping to 0

## L16 finale
1. render   render into individual OpenEXR (prefered, half color depth is fine) or TIFF, then compile that into video
2. color    three colors or less?
3. output   properties; output
4. render   render tab (top), render animation
5. openexr  color space is not embeded
6. video    video sequence editor
7. video    add, image sequence
8. video    render, color management; filmic, high contrast, exposure (1.0, same as previous setting)
9. video    render tab, render animation

# 4 week curriculum 
https://www.blenderguru.com/podcasts/episode-4
https://www.youtube.com/watch?v=nqW01JzVQFQ

## week 1
1. complete: blender `beginning donut tutorial`
2. homework: create something similar by yourself (eg. cookie or a cupcake)

## week 2
1. lighting: watch `beginners guide to lighting`; practice: create 5 lighting variations for your donut render (trying many ideas)
2. photorealism: watch `how to make photorealistic materials in blender`, `principles bsdf in blender`
3. texturing: complete `the anvil tutorial`; homework: make something related an axe, a weapon etc. (something small and achievable within 2-3 days, replicate the photo 1:1)
4. composition: watch `understanding composition`; homework: use your lighting and composition knowledge to create 5 variations of your anvil (aspect ratios, etc)

## week 3
1. solo project: create something entirely new of your own choosing that's achievable within 2 days. (eg, axe, hammer, latern etc); replicate a photo 1 to 1 is very most important (comparision)
2. environment creation: watch: `render optimizations`; watch: `introduction to microdisplacements`; watch: `how to tile a texture properly`; watch: `importing FBX models into blender` (how to use photo scans)
3. solo project: create an environment of your own choosing (desert is easiest)

## week 4
1. research: visit artstation and explore the highest performing environement entries 
2. technical: watch: `how to import Mixamo Characters into Blender`; homework: add the acharacter to your enviornment
3. aesthetics: watch: `understanding color`; practical: try to improve color in your environment image; watch: `compositing effects in blender`; homework: add glare, barrel distortion, a vignette and sharpening to environement, color management, color grading
4. final project: using everything you've learned, create an environment with a character