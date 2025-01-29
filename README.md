# C/C++ open-source libraries with minimal dependencies

Generally, the following is a list of small, easy-to-integrate, portable libraries
which are usable from C and/or C++, and should be able to be compiled on both
32-bit and 64-bit platforms. There is preference for libraries that are C, public domain and single-file.
However, we have not personally verified that any specific library is as advertised, or is quality software.

### New libraries and corrections

We accept submissions for new libraries and corrections if information for a library below is wrong.
Consider either opening a Pull Request, a new Issue or drop a message in our discord channel: https://discord.gg/2fZVEym
The server is meant to be a pleasant space to chat about C, C++, Libs authoring and Game development specifically.

### Rules

- Libraries must be usable from C or C++, ideally both.
- Libraries must include the licensing terms in the header and source files.
- Libraries should be usable from more than one platform (ideally, all major desktops and/or all major mobile).
- Libraries should compile and work on both 32-bit and 64-bit platforms.
- Libraries should use at most two files (one header, one source): more than two files are mostly forbidden.

Exceptions will be allowed for good reasons.

### Other lists

Also you might be interested in other related, but different lists:

- [**STB**](https://github.com/nothings/stb): the mighty collection of gamedev utils.
- [clib](https://github.com/clibs/clib/wiki/Packages): list of (mostly) small single C functions (licenses not listed)
- [CCAN](https://ccodearchive.net/list.html): package of lots of shareable C functions (mixed licenses)
- And some more: 
[**andrewwillmott**](https://github.com/andrewwillmott?tab=repositories&q=&type=source&language=c&sort=),
[b-library (C,C++)](https://github.com/blat-blatnik/B-Library),
[blastbay](https://github.com/blastbay?tab=repositories&q=&type=source&language=c&sort=),
[chobo-shl (C++)](https://github.com/Chobolabs/chobo-shl),
[clibs](https://github.com/ennorehling/clibs), 
[containers (C++)](https://github.com/JCash/containers),
[cpp-poc (C++)](https://github.com/xdbr/cpp-poc),
[**cute_headers** (C,C++)](https://github.com/RandyGaul/cute_headers), 
[data-structures-c](https://github.com/bartobri/data-structures-c),
[**dr_libs**](https://github.com/mackron/dr_libs), 
[dyeo.h](https://github.com/dyeo/dyeo.h), 
[emilib (C++)](https://github.com/emilk/emilib),
[final_game_tech (C,C++)](https://github.com/f1nalspace/final_game_tech), 
[ftg_toolbox_public](https://github.com/frogtoss/ftg_toolbox_public),
[**gb**](https://github.com/gingerBill/gb), 
[gl-helpers (C,C++)](https://github.com/Flix01/Header-Only-GL-Helpers),
[ijhandlealloc](https://github.com/incrediblejr/ijhandlealloc),
[jar](https://github.com/kd7tck/jar), 
[**jo**](https://jonolick.com/code.html),
[kj](https://github.com/AfroDave/kj),
[**klib**](https://github.com/attractivechaos/klib),
[**kokke**](https://github.com/kokke?tab=repositories&q=&type=source&language=c&sort=),
[libjrc](https://github.com/SmileTheory/libjrc),
[**libs**](https://github.com/mattiasgustavsson/libs), 
[libs](https://github.com/bullno1/libs),
[live_edit](https://github.com/azmr/live_edit),
[maratis](https://github.com/anael-seghezzi/Maratis-Tiny-C-library), 
[**minilibs**](https://github.com/ccxvii/minilibs), 
[miscsrc](https://github.com/wernsey/miscsrc),
[**mmx**](https://github.com/vurtun/mmx), 
[**nflibs**](https://github.com/niklasfrykholm/nflibs),
[noc](https://github.com/guillaumechereau/noc), 
[ok-**fm**](https://github.com/brackeen/ok-file-formats),
[ok-**lib**](https://github.com/brackeen/ok-lib),
[**par**](https://github.com/prideout/par), 
[pico_headers](https://github.com/empyreanx/pico_headers), 
[portable-snippets](https://github.com/nemequ/portable-snippets),
[px (C++)](https://github.com/pplux/px), 
[rjm](https://github.com/rmitton/rjm), 
[**rxi**](https://github.com/rxi?tab=repositories&q=&type=source&language=c&sort=),
[shadertoolkit](https://github.com/jarikomppa/shadertoolkit),
[single-header-file-c-libs](https://github.com/arkanis/single-header-file-c-libs),
[**skeeto**](https://github.com/skeeto?tab=repositories&q=&type=source&language=c&sort=),
[slibs](https://github.com/yui0/slibs),
[snippets](https://github.com/blat-blatnik/Snippets),
[snippets](https://github.com/DanielGibson/Snippets), 
[**sokol**](https://github.com/floooh/sokol), 
[statvs (C++)](https://github.com/r-lyeh-archived/statvs),
[sts](https://github.com/kieselsteini/sts), 
[**sweet** (C++)](https://github.com/burner/sweet.hpp), 
[tinybits (C,C++)](https://github.com/r-lyeh/tinybits), 
[**tm**](https://github.com/to-miz/tm),
[yocto-gl (C++)](https://github.com/xelatihy/yocto-gl), 
[zeroTolerance](https://github.com/jharler/ZeroTolerance),
[zheaders](https://github.com/Zguy/ZHeaders),
[**zpl**](https://github.com/zpl-c/zpl),

### Library listing

| tag  | library                                                              | license          | &nbsp;&nbsp;&nbsp;API&nbsp;&nbsp;&nbsp; |files| description
| ---- | -------------------------------------------------------------------- |:----------------:|:---:|:---:| -----------
2d     | [si_normalmap](https://github.com/Sir-Irk/si_normalmap)              | **PD**           |**C**|**1**| Image to Normal Map generator
3d     | [lightmapper](https://github.com/ands/lightmapper#lightmapper)       | **PD**           |**C/C++**|**1**| Use your OpenGL renderer to offline bake lightmaps
3d     | [seamoptimizer](https://github.com/ands/seamoptimizer)               | **PD**           |**C/C++**|**1**| Modify lightmap data to hide seams
3d     | [small3dlib](https://gitlab.com/drummyfish/small3dlib)        | **CC0** + patent waiver |**C/C++**|**1**| Fast and portable software renderer
3d     | [stb_voxel_render](https://github.com/nothings/stb/blob/main/stb_voxel_render.h) |**PD**|**C/C++**|**1**| Minecraft-esque voxel rendering "engine" with many more features
3d     | [Vertex Cache Optimizer](https://github.com/Sigkill79/sts)           | **PD**           |**C/C++**|**1**| Vertex cache optimization of meshes
audio  | [atomix](https://github.com/BareRose/atomix)                         | **PD**           |**C**|**1**| Wait-free atomic sound mixer
audio  | [miniaudio](https://github.com/dr-soft/miniaudio)                    | **PD**           |**C/C++**|**1**| Audio playback and capture library
audio  | [minimp3](https://github.com/lieff/minimp3)                          | **CC0**          |**C**|**1**| Minimalistic MP3 decoder with sse/neon support
audio  | [stb_hexwave](https://github.com/nothings/stb/blob/main/stb_hexwave.h)|           **PD**|**C/C++**|**1**| Audio waveform synthesizer
audio  | [stb_vorbis](https://github.com/nothings/stb/blob/main/stb_vorbis.c)  |           **PD**|**C/C++**|**1**| Decode ogg vorbis files from file/memory to float/16-bit signed output
bench  | [ubench.h](https://github.com/sheredom/ubench.h)                     | **PD**           |**C/C++**|**1**| Microbenchmarking 
c      | [minicoro](https://github.com/edubart/minicoro/)                     | **PD**/**0MIT**  |**C/C++**|**1**| Stackful cross-platform coroutine library
c      | [stb_sprintf](https://github.com/nothings/stb/blob/main/stb_sprintf.h) |          **PD**|**C/C++**|**1**| Fast sprintf, snprintf for C/C++
crypt  | [random3](https://github.com/MichelPaulissen/random3)                | **PD**           |**C/C++**|**1**| Crypt-random generator
dev    | [EasyTab](https://github.com/ApoorvaJ/EasyTab)                       | **PD**           |**C/C++**|**1**| Multi-platform tablet input
ds     | [aArray](https://tse.gratis/aArray/)                                 | **PD**           |**C**|**1**| Arrays/strings: generic, safe
ds     | [cds_algo](https://github.com/cdwfs/algo)                            | **PD**           |**C/C++**|**1**| Collection of data structures (queue, stack, graph, heap...)
ds     | [DG_dynarr.h](https://github.com/DanielGibson/Snippets/)             | **PD**           |**C/C++**|**1**| Typesafe dynamic arrays (like std::vector) for plain C
ds     | [dynarr](https://github.com/BareRose/dynarr)                         | **PD**           |**C**|**1**| Dynamic array container
ds     | [jrsl](https://github.com/Garfield1002/jrsl)                         | **PD**           |**C/C++**|**1**| Skip Lists
ds     | [stb_ds](https://github.com/nothings/stb/blob/main/stb_ds.h) |                    **PD**|**C/C++**|**1**| Typesafe dynamic array and hash tables for C, will compile in C++
engine | [FWK1](https://github.com/fwk3d/v1/blob/master/2024/2024.10/engine/joint.h) | **PD**    | C |**1**| 3D game framework in C
engine | [kit](https://github.com/rxi/kit)                                    | **PD**           | C |**1**| Tiny library for making small games with big pixels
font   | [stb_easy_font](https://github.com/nothings/stb/blob/main/stb_easy_font.h) |      **PD**|**C/C++**|**1**| Quick-and-dirty easy-to-deploy bitmap font for printing frame rate, etc
font   | [stb_truetype](https://github.com/nothings/stb/blob/main/stb_truetype.h) |        **PD**|**C/C++**|**1**| Parse, decode, and rasterize characters from truetype fonts
game   | [raycastlib.h](https://gitlab.com/drummyfish/raycastlib)             | **CC0** + patent waiver  |**C/C++**|**1**| Advanced raycasting rendering library, pure C99 with no dependencies, only 32bit int math
game   | [stb_connected_components](https://github.com/nothings/stb/blob/main/stb_connected_components.h) | **PD**|**C/C++**|**1**| Incrementally compute reachability on grids
game   | [stb_herringbone_wang_tile](https://github.com/nothings/stb/blob/main/stb_herringbone_wang_tile.h) | **PD**|**C/C++**|**1**| Herringbone Wang tile map generator
game   | [stb_tilemap_editor](https://github.com/nothings/stb/blob/main/stb_tilemap_editor.h) |**PD**|**C/C++**|**1**| Embeddable tilemap editor
hash   | [lonesha256](https://github.com/BareRose/lonesha256)                 | **PD**           |**C**|**1**| SHA256 implementation
image  | [cro_mipmap.h](https://github.com/thebeast33/cro_lib)                | **PD**           |**C/C++**|**1**| Average, min, max mipmap generators
image  | [stb_image](https://github.com/nothings/stb/blob/main/stb_image.h) |              **PD**|**C/C++**|**1**| Image loading/decoding from file/memory: JPG, PNG, TGA, BMP, PSD, GIF, HDR, PIC
image  | [stb_image_resize](https://github.com/nothings/stb/blob/main/stb_image_resize2.h)|**PD**|**C/C++**|**1**| Resize images larger/smaller with good quality
image  | [stb_image_write](https://github.com/nothings/stb/blob/main/stb_image_write.h) |  **PD**|**C/C++**|**1**| Image writing to disk: PNG, TGA, BMP
image  | [stb_perlin](https://github.com/nothings/stb/blob/main/stb_perlin.h) |            **PD**|**C/C++**|**1**| Perlin's revised simplex noise w/ different seeds
image  | [stb_rect_pack](https://github.com/nothings/stb/blob/main/stb_rect_pack.h) |      **PD**|**C/C++**|**1**| Simple 2D rectangle packer with decent quality
image  | GIF [gif_load](https://github.com/hidefromkgb/gif_load)              | **PD**           |**C/C++**|**1**| (animated) GIF reader
image  | JPG [tiny_jpeg.h](https://github.com/serge-rgb/TinyJPEG/)            | **PD**           |**C/C++**|**1**| JPEG encoder
image  | WEBP [jebp](https://github.com/matanui159/jebp)                      | **0MIT**         |**C/C++**|**1**| Single header WebP decoder
json   | [json.h](https://github.com/sheredom/json.h)                         | **PD**           |**C/C++**|**1**| JSON parser
math   | [cds_spline](https://github.com/cdwfs/cds_spline/blob/master/cds_spline.h)|**PD**       |**C/C++**|**1**| Spline utils
math   | [df](https://github.com/983/df)                                      | **PD**           |**C/C++**|**1**| Find voronoi region in linear time of size of lattice
math   | [dvector](https://github.com/BareRose/dvector)                       | **PD**           |**C**|**1**| 2D/3D vector/quaternion/matrix math library
math   | [linmath.h](https://github.com/datenwolf/linmath.h)                  | **WTFPLv2**      |**C**|**1**| Vector library
math   | [nv_voronoi.h](https://www.icculus.org/~mordred/nvlib/)              | **PD**           |**C/C++**|**1**| Find voronoi regions on lattice w/ integer inputs
math   | [prns.h](https://marc-b-reynolds.github.io/shf/2016/04/19/prns.html) | **PD**           |**C/C++**|**1**| Seekable pseudo-random number sequences
math   | [rfft.h](https://github.com/grego/rfft.h)                            | **PD**           |**C/C++**|**1**| Fast Fourier Tranform for arbitrary array sizes
math   | [sobol.h](https://github.com/Marc-B-Reynolds/Stand-alone-junk/)      | **PD**           |**C/C++**|**1**| Sobol & stratified sampling sequences
math   | [Statistics-Tool-Box](https://github.com/gerbenvoshol/Statistics-Tool-Box) | **PD**     |**C/C++**|**1**| Statistical functions
math   | [stb_divide](https://github.com/nothings/stb/blob/main/stb_divide.h) |            **PD**|**C/C++**|**1**| More useful 32-bit modulus
math   | [vmath](https://github.com/monolifed/vmath)                          | **PD**           |**C**|**1**| Vector/matrix library
mem    | [buddy_alloc](https://github.com/spaskalev/buddy_alloc)              | **BSD0**         |**C**|**1**| Buddy memory allocator
mem    | [stb_leakcheck](https://github.com/nothings/stb/blob/main/stb_leakcheck.h) |      **PD**|**C/C++**|**1**| Quick-and-dirty malloc/free leak-checking
mem    | [wb_alloc](https://github.com/WilliamBundy/wb_alloc)                 | **PD**           |**C/C++**|**1**| Custom allocators in a single-header
misc   | [CLM_LIBS](https://github.com/CarlosLunaMota/CLM_LIBS)               | **PD**           |**C**|**1**| Diverse utilities
misc   | [Hedley](https://nemequ.github.io/hedley/)                           | **PD**           |**C/C++**|**1**| Compiler portability, optimization, static analysis, etc.
misc   | [process.h](https://github.com/sheredom/process.h)                   | **PD**           |**C/C++**|**1**| Process control API
misc   | [sili-toolchain](https://github.com/EimaMei/sili-toolchain)          | **PD**           |**C/C++**|**1**| C toolchain for modern C programming, strings, arrays, files, threading, ect
misc   | [stb_include](https://github.com/nothings/stb/blob/main/stb_include.h) |          **PD**|**C/C++**|**1**| Implement recursive #include support, particularly for GLSL
net    | [swrap](https://github.com/BareRose/swrap)                           | **PD**           |**C**|**1**| TCP and UDP socket wrapper
net    | [zed_net](https://github.com/Smilex/zed_net)                         | **PD**           |**C/C++**|**1**| Cross-platform socket wrapper
pack   | [nibrans](https://github.com/BareRose/nibrans)                       | **PD**           |**C**|**1**| Adaptive rANS library
pack   | [stb_dxt](https://github.com/nothings/stb/blob/main/stb_dxt.h) |                  **PD**|**C/C++**|**1**| Real-time DXT compressor
parse  | [stb_c_lexer](https://github.com/nothings/stb/blob/main/stb_c_lexer.h) |          **PD**|**C/C++**|**1**| Simplify writing parsers for C-like languages
prng   | [ranxoshi256](https://github.com/BareRose/ranxoshi256)               | **PD**           |**C**|**1**| Xoshiro256 algorithm
regex  | [Remimu](https://github.com/wareya/Remimu)                           | **CC0**          |**C/C++**|**1**| Regex engine
script | [xpl](https://github.com/paladin-t/xpl)                              | **WTFPLv2**      |**C**|**1**| X Programming Language
serial | [Serialization helper](https://gist.github.com/TheServer201/9ae5322cd52f76c7d36af15d3b366762) | **WTFPLv2** |**C**|**1**| Serialization helper
string | [gb_string.h](https://github.com/gingerBill/gb)                      | **PD**           |**C/C++**|**1**| Dynamic strings
string | [utf8](https://github.com/sheredom/utf8.h)                           | **PD**           |**C/C++**|**1**| UTF-8 string library
sys    | [doops](https://github.com/eduardsui/doops)                          | **PD**           |**C**|**1**| Event loop library
sys    | [endianness.h](https://github.com/rofl0r/endianness.h)               | **PD**           |**C**|**1**| Endianness conversion and detection  
thread | [cds_sync](https://github.com/cdwfs/cds_sync)                        | **PD**           |**C/C++**|**1**| Collection of synchronization primitives
ui     | [libcmdf](https://github.com/ronen25/libcmdf)                        | **PD**           |**C**|**1**| A small library for writing CLI applications
ui     | [nuklear](https://github.com/Immediate-Mode-UI/Nuklear)              | **PD**           |**C/C++**|**1**| Minimal GUI toolkit
ui     | [stb_textedit](https://github.com/nothings/stb/blob/main/stb_textedit.h) |        **PD**|**C/C++**|**1**| Guts of a text editor for games etc implementing them from scratch
unit   | [labrat](https://github.com/squarewave/labrat)                       | **PD**           |**C/C++**|**1**| Unit testing
unit   | [Rexo](https://github.com/christophercrouzet/rexo)                   | **PD**           |**C/C++**|**1**| Framework for C89/C++ featuring automatic registration of tests and a polished API
unit   | [utest.h](https://github.com/sheredom/utest.h)                       | **PD**           |**C/C++**|**1**| Unit testing
unit   | [walter](https://github.com/ir33k/walter)                            | **PD**           |**C**|**1**| Unit testing
vector | [ccVector.h](https://github.com/jobtalle/ccVector)                   | **PD**           |**C/C++**|**1**| Vector, quaternion and matrix math
vector | [Handmade Math](https://github.com/StrangeZak/Handmade-Math)         | **PD**           |**C/C++**|**1**| Vector math
video  | [jo_mpeg](https://www.jonolick.com/home/mpeg-video-writer) / [(converted to C)](https://blog.frost.kiwi/jo-mpeg-in-c) | **PD** |**C/C++**|**1**| MPEG file writer
image  | [jo_sift](https://www.jonolick.com/home/scale-invariant-feature-transform-sift-single-file-library) | **PD** |**C/C++**|**1**| Image feature detection and matching

### Secondary listing

The listing below meets some but not all the requirements aforementioned.

| tag  | library                                                              | license          | &nbsp;&nbsp;&nbsp;API&nbsp;&nbsp;&nbsp; |files| description
| ---- | -------------------------------------------------------------------- |:----------------:|:---:|:---:| -----------
2d     | [blendish](https://hg.sr.ht/~duangle/oui-blendish)                   | MIT              |**C/C++**|**1**| Blender-style widget rendering using NanoVG
2d     | [C-Turtle](https://github.com/walkerje/C-Turtle)                     | MIT              | C++ |**1**| Port of Python's Turtle to C++
2d     | [cgl](https://github.com/Jaysmito101/cgl)                            | MIT              |**C**|  2  | C Game Library
2d     | [Cimg](https://cimg.eu/)                                             | CeCILL/CeCILL-C  | C++ |**1**| Image processing toolkit (60K LoC)
2d     | [colourblind](https://github.com/azmr/colourblind)                   | ISC              |**C/C++**|**1**| Simulating colourblindness
2d     | [daisy](https://github.com/sse2/daisy)                               | MIT              | C++ |**1**| 2D Graphics and text
2d     | [Immediate2D](https://github.com/npiegdon/immediate2d)               | **PD**           | C++ |  2  | Zero-configuration, immediate-mode 2D graphics for Windows
2d     | [m_image.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_image.h) | ZLIB |**C/C++**|**1**| Image processing routines
2d     | [RFont](https://github.com/ColleagueRiley/RFont)                     | ZLIB             |**C/C++**|**1**| Simple-to-use lightweight single header modular font rendering library
2d     | [RGL](https://github.com/ColleagueRiley/RGL)                         | ZLIB             |**C/C++**|**1**| Simple ultra-lightweight OpenGL version abstraction based on RLGL (pipeline system)
2d     | [scalable-font2](https://gitlab.com/bztsrc/scalable-font2)           | MIT              |**C**|**1**| Scalable Font renderer + specification
2d     | [tigr](https://bitbucket.org/rmitton/tigr/src)                       | **PD**           |**C/C++**|  2  | Quick-n-dirty window text/graphics for Windows and macOS
2d     | [wfc](https://github.com/krychu/wfc)                                 | MIT              |**C**|**1**| Generate image locally similar to the input image using WFC algorithm
3d     | [debug-draw](https://github.com/glampert/debug-draw)                 | **PD**           | C++ |**1**| API-agnostic immediate-mode debug rendering
3d     | [mikktspace](https://developer.blender.org/diffusion/B/browse/master/intern/mikktspace)| zlib|**C/C++**| 2  | Compute tangent space for normal mapping
3d     | [model3d](https://gitlab.com/bztsrc/model3d)                         | MIT              |**C**|**1**| 3D model format specification
3d     | [Simple OpenGL Loader](https://github.com/tsherif/simple-opengl-loader)| MIT            |**C/C++**|**1**| Extensible, cross-platform OpenGL loader
3d     | [Swarmz](https://github.com/Cultrarius/Swarmz)                       | **PD**           | C++ |**1**| Swarming/flocking algorithm
3d     | [tinygizmo](https://github.com/ddiakopoulos/tinygizmo)               | **PD**           | C++ |  2  | Gizmo objects for interactively editing 3d transformations
3d     | [Vulkan Memory Allocator](https://github.com/GPUOpen-LibrariesAndSDKs/VulkanMemoryAllocator)|MIT|**C/C++**|**1**| Memory allocator for Vulkan
ai     | [Genann](https://github.com/codeplea/genann)                         | zlib             |**C/C++**|  2  | Simple neural networks (ANN)
ai     | [KANN](https://github.com/attractivechaos/kann)                      | MIT              |**C/C++**|  2  | Automatic differentiation (2 files)
app    | [RGFW](https://github.com/ColleagueRiley/RGFW)                       | ZLIB             |**C/C++**|**1**| A multi-platform single-header user-friendly GUI framework as an alternative to GLFW 
argv   | [Argh!](https://github.com/adishavit/argh)                           | BSD              | C++ |**1**| Command-line argument parsing
argv   | [Clara](https://github.com/catchorg/Clara)                           | Boost            | C++ |**1**| Composable, command line parser for C++ 11 and beyond
argv   | [CLI11](https://github.com/CLIUtils/CLI11)                           | BSD              | C++ |**1**| Feature-rich CLI parsing in modern C++11
argv   | [cmdline](https://github.com/tanakh/cmdline)                         | BSD              | C++ |**1**| Command-line argument parsing
argv   | [flags](https://github.com/sailormoon/flags)                         | **PD**           | C++ |**1**| Command-line argument parsing
argv   | [kgflags](https://github.com/kgabis/kgflags)                         | MIT              |**C/C++**|**1**| Command-line argument parsing
argv   | [linkom](https://github.com/hernandp/linkom)                         | MIT              |**C/C++**|**1**| Command-line argument parsing w/ DOS-style options
argv   | [optionparser](https://optionparser.sourceforge.net/)                | MIT              | C++ |**1**| Command-line argument parsing
argv   | [parg](https://github.com/jibsen/parg)                               | **PD**           |**C**|  2  | Command-line argument parsing
argv   | [ProgramOptions.hxx](https://github.com/Fytch/ProgramOptions.hxx)    | MIT              | C++ |**1**| Command-line argument parsing
audio  | [aw_ima.h](https://github.com/afterwise/aw-ima/blob/master/aw-ima.h) | MIT              |**C/C++**|**1**| IMA-ADPCM audio decoder
audio  | [btac1c](https://github.com/cr88192/bgbtech_misc/blob/master/mini/btac1c_mini0.h)| MIT  |**C/C++**|**1**| MS-IMA_ADPCM variant
audio  | [chibi-xmplay](https://github.com/reduz/chibi-xmplay)                | BSD3             |**C**|  2  | XM module playback library
audio  | [Geneva](https://github.com/KrzysztofSzewczyk/Geneva)                | MIT              |**C/C++**|**1**| Library generating 8-bit waveforms of various kinds
audio  | [mojoAL](https://github.com/icculus/mojoAL)                          | ZLIB             |**C**|**1**| Full OpenAL 1.1 implementation
audio  | [nanoalsa](https://gitlab.com/bztsrc/nanoalsa)                       | MIT              |**C**|**1**| Tiny PCM playback under Linux
audio  | [pocketmod](https://github.com/rombankzero/pocketmod)                | MIT              |**C/C++**|**1**| ProTracker MOD file renderer
audio  | [TinySoundFont](https://github.com/schellingb/TinySoundFont)         | MIT              |**C/C++**|**1**| SoundFont2 loader & synthesizer
bench  | [picobench](https://github.com/iboB/picobench)                       | MIT              | C++ |**1**| Microbenchmarking
c      | [errnoname](https://github.com/mentalisttraceur/errnoname)           | **BSD0**         |**C**|  2  | Extended errno messages
cpp    | [filesystem](https://github.com/gulrak/filesystem)                   | MIT              | C++ |**1**| Implementation of std::filesystem
cpp    | [outcome](https://github.com/ned14/outcome/tree/develop/single-header) | Apache2/Boost  | C++ |**1**| Outcome and result C++ containers
crypt  | [ggentropy](https://github.com/mikejsavage/ggentropy)                | ISC              | C++ |  2  | Cross platform entropy library
crypt  | [Monocypher](https://monocypher.org)                                 | **PD**           |**C**|  2  | High-quality small cryptography library
crypt  | [TweetNaCl](https://tweetnacl.cr.yp.to/software.html)                | **PD**           |**C**|  2  | High-quality tiny cryptography library
csv    | [CSVstream](https://github.com/awdeorio/csvstream/)                  | MIT              | C++ |**1**| CSV parser
csv    | [Fast C++ CSV Parser](https://github.com/ben-strasser/fast-cpp-csv-parser) | BSD        | C++ |**1**| CSV parser
csv    | [Rapidcsv](https://github.com/d99kris/rapidcsv/)                     | BSD              | C++ |**1**| CSV parser
csv    | [Vince's CSV Parser](https://github.com/vincentlaucsb/csv-parser)    | MIT              | C++ |**1**| CSV parser and serializer
date   | [date](https://github.com/HowardHinnant/date)                        | MIT              | C++ |**1**| Date and time libraries
debug  | [dbgtools](https://github.com/wc-duck/dbgtools)                      | zlib             |**C/C++**|  2  | Cross-platform debug util libraries
debug  | [debug-assert](https://github.com/foonathan/debug_assert)            | zlib             | C++ |**1**| Modular assertion macro
debug  | [debugbreak](https://github.com/scottt/debugbreak)                   | BSD              |**C/C++**|**1**| Programmatic debug break
debug  | [loguru](https://github.com/emilk/loguru)                            | **PD**           | C++ |**1**| Flexible logging
debug  | [pempek_assert.cpp](https://github.com/gpakosz/Assert)               | **WTFPLv2**      | C++ |  2  | Flexible assertions
dev    | [libue](https://github.com/houqp/libue)                              | MIT              |**C/C++**|**1**| Helper library for Linux device hot-plug event
ds     | [avl](https://github.com/etherealvisage/avl)                         | **PD**           |**C/C++**|  2  | AVL tree
ds     | [DynaVar](https://github.com/ArjArav98/DynaVar)                      | GPL-3.0          | C++ |  1  | Object which can store any type of primitive data type
ds     | [fifo_declare.h](https://github.com/buserror/simavr/blob/master/simavr/sim/fifo_declare.h) | LGPL2 |**C/C++**|**1**| Thread/core safe FIFO
ds     | [itlib](https://github.com/iboB/itlib)                               | MIT              | C++ |**1**| Several C++11 standard-contaner-like libraries and helpers
ds     | [jhr_skip_list](https://github.com/Garfield1002/jhr_skip_list)       | **PD**           | C++ |**1**| Skip Lists
ds     | [klib](https://attractivechaos.github.io/klib/)                      | MIT              |**C/C++**|  2  | Many 2-file libs: hash, sort, b-tree, etc
ds     | [libintrusive](https://github.com/graphitemaster/libintrusive)       | **PD**           |**C**|  2  | Intrusive data structures
ds     | [libpqueue](https://github.com/vy/libpqueue)                         | BSD              |**C/C++**|  2  | Priority queue (heap)
ds     | [LinkedList](https://github.com/ivanseidel/LinkedList)               | MIT              |**C/C++**|  2  | Linked list C++ 
ds     | [mempool](https://github.com/hardikp/cpp-mempool)                    | MIT              | C++ |**1**| Efficient minimal memory pool implementation for C++
ds     | [PackedArray](https://github.com/gpakosz/PackedArray)                | **WTFPLv2**      |**C**|  2  | Memory-efficient array of elements with non-pow2 bitcount
ds     | [selist](https://github.com/ennorehling/clibs)                       | ISC              |**C/C++**|  2  | Space-efficient linked-list
ds     | [simclist](https://mij.oltrelinux.com/devel/simclist)                | BSD              |**C/C++**|  2  | Linked-list
ds     | [uthash](https://github.com/troydhanson/uthash)                      | BSD              |**C/C++**|  2  | Several 1-header, 1-license-file libs: generic hash, list, etc
engine | [olcPixelGameEngine](https://github.com/OneLoneCoder/olcPixelGameEngine) | BSD3         | C++ |**1**| Game engine
engine | [Punity](https://github.com/martincohen/Punity)                      | MIT              | C |**1**| A tiny game engine in C
file   | [dirent](https://github.com/tronkko/dirent)                          | MIT              |**C/C++**|**1**| Dirent for Windows: retrieve file & dir info
file   | [miniphysfs](https://github.com/edubart/miniphysfs)                  | ZLIB             |**C/C++**|**1**| Single-file port of PhysFS, a fs/zip abstraction
file   | [tfile](https://github.com/rec/tfile)                                | MIT              |C++|**1**| FILE* wrapper does read-write-append-seek-close (Win/Mac/Unix)
file   | [TinyDir](https://github.com/cxong/tinydir)                          | BSD              |**C**|**1**| Cross-platform directory reading (Win/POSIX/MinGW)
file   | [whereami](https://github.com/gpakosz/whereami)                      | **WTFPLv2**      |**C/C++**|  2  | Get path/filename of executable or module
font   | [blit-fonts](https://github.com/azmr/blit-fonts)                     | ISC              |**C/C++**|**1**| Bitmap font blitters
font   | [ssfn.h](https://gitlab.com/bztsrc/scalable-font)                    | MIT              |**C/C++**|**1**| Scalable/bitmap/pixmap font renderer
hash   | [hash.c](https://github.com/zzo38/freeheromesh/blob/trunk/hash.c)    | **PD**           |**C**|  2  | SHA1/SHA3/MD5 hashes
hash   | [PicoSHA2](https://github.com/okdshin/PicoSHA2)                      | MIT              | C++ |**1**| SHA256 implementation
hash   | [xxHash](https://github.com/Cyan4973/xxHash)                         | BSD              |**C/C++**|  2  | Fast hash function
image  | [bitmap](https://github.com/ArashPartow/bitmap)                      | MIT              | C++ |**1**| Bitmap decoder and utilities
image  | [framepacker](https://github.com/paladin-t/framepacker)              | MIT              | C++ |**1**| Texture bin packing algorithm
image  | [tiffloader](https://github.com/MalcolmMcLean/tiffloader)            | **PD**           |**C**|  2  | TIFF image loader
image  | EXR [miniexr](https://github.com/aras-p/miniexr)                     | **PD**           | C++ |  2  | OpenEXR writer, needs header file
image  | EXR [tinyexr](https://github.com/syoyo/tinyexr)                      | BSD              |**C/C++**|**1**| EXR image read/write, uses miniz internally
image  | GIF [gif.h](https://github.com/ginsweater/gif-h)                     | **PD**           | C++ |**1**| Animated GIF writer (can only include once)
image  | GIF [jo_gif.cpp](https://www.jonolick.com/home/gif-writer)           | **PD**           | C++ |**1**| Animated GIF writer (CPP file can also be used as H file)
image  | JPG [jpeg-compressor](https://github.com/richgel999/jpeg-compressor) | **PD**           | C++ |  2  | 2-file JPEG compress, 2-file JPEG decompress
image  | JPG [NanoJPEG](https://keyj.emphy.de/nanojpeg/)                      | MIT              |**C/C++**|**1**| JPEG decoder
image  | JPG EXIF [easyexif](https://github.com/mayanklahiri/easyexif)        | BSD2             | C++ |  2  | EXIF metadata extractor for JPEG images
image  | JPG EXIF [TinyEXIF](https://github.com/cdcseacave/TinyEXIF)          | BSD              | C++ |  2  | Parse EXIF data from JPEG (XMP w/ TinyXML2 lib)
image  | PDF [PDFgen](https://github.com/AndreRenaud/PDFGen)                  | **PD**           |**C**|  2  | PDF writer |
image  | PNG [lodepng](https://lodev.org/lodepng/)                            | zlib             |**C/C++**|  2  | PNG encoder/decoder
image  | PNG [picopng.cpp](https://lodev.org/lodepng/picopng.cpp)             | zlib             | C++ |  2  | Tiny PNG loader
image  | PNG [TinyPngOutput](https://www.nayuki.io/page/tiny-png-output)      | LGPLv3           |**C/C++**|  2  | PNG writer |
image  | PNM [PNM](https://github.com/dmilos/PNM)                             | Apache2          | C++ |  1  | PBM, PGM and PPM reader and writer |
image  | SVG [nanoSVG](https://github.com/memononen/nanosvg)                  | ZLIB             |**C/C++**|**1**| 1-file SVG parser; 1-file SVG rasterizer
ini    | [inih](https://github.com/benhoyt/inih)                              | BSD              |**C/C++**|  2  | .ini file parser
json   | [ajson](https://github.com/lordoffox/ajson)                          | Boost            | C++ |**1**| JSON serialize & deserialize w/ STL support
json   | [cJSON](https://github.com/DaveGamble/cJSON)                         | MIT              |**C/C++**|**1**| JSON parser
json   | [cJSON](https://sourceforge.net/projects/cjson/)                     | MIT              |**C/C++**|**1**| JSON parser
json   | [jsmn](https://github.com/zserge/jsmn)                               | MIT              |**C**|**1**| Minimalistic JSON parser
json   | [json-build](https://github.com/lcsmuller/json-build)                | MIT              |**C/C++**|**1**| JSON serializer
json   | [json.hpp](https://github.com/nlohmann/json)                         | MIT              | C++ |**1**| JSON parse, serialize, deserialize
json   | [jsonc](https://gitlab.com/bztsrc/jsonc)                             | MIT              |**C/C++**|**1**| Extremely fast and extremely small (~60 SLoC) JSON parser
json   | [jzon.h](https://github.com/Zguy/Jzon)                               | MIT              | C++ |  2  | JSON parser
json   | [parson](https://github.com/kgabis/parson)                           | MIT              |**C/C++**|  2  | JSON parser and serializer
json   | [PicoJSON](https://github.com/kazuho/picojson)                       | BSD              | C++ |**1**| JSON parse/serializer
json   | [sjson](https://github.com/septag/sjson)                             | BSD2             |**C**|**1**| JSON encode/decoder
logic  | [FFSM2](https://github.com/andrew-gresyk/FFSM2/blob/master/include/ffsm2/machine.hpp) | MIT | C++ |**1**| Flat FSM
logic  | [HFSM2](https://github.com/andrew-gresyk/HFSM2/blob/master/include/hfsm2/machine.hpp) | MIT | C++ |**1**| Hierarchical FSM
math   | [amoeba](https://github.com/starwing/amoeba)                         | MIT              |**C/C++**|**1**| Constraint solver (Cassowary) w/Lua binding
math   | [ceval-single-header](https://github.com/e-t-sudo/ceval-single-header)| MIT             |**C/C++**|**1**| A single-header library for parsing and evaluation of arithmetic expressions
math   | [Clipper](https://www.angusj.com/delphi/clipper.php)                 | Boost            | C++ |  2  | Line & polygon clipping & offsetting
math   | [Delaunay](https://github.com/BrunoLevy/geogram.psm.Delaunay)        | BSD3             | C++ |  2  | 2D and 3D Delaunay triangulation
math   | [ExprTk](https://www.partow.net/programming/exprtk/index.html)       | MIT              | C++ |**1**| Runtime mathematical expression parser and evaluation engine.
math   | [fft](https://github.com/wareya/fft)                                 | **PD**           | C++ |**1**| Fast Fourier Transform |
math   | [HMM Toolkit](https://github.com/gerbenvoshol/Hidden-Markov-Model-Toolkit) | GPL2       |**C/C++**|**1**| Discrete and continuous Hidden Markov Models (DHMM, CHMM)
math   | [jc_voronoi](https://github.com/JCash/voronoi)                       | MIT              |**C/C++**|**1**| Find voronoi regions on float/double data
math   | [m_math.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_math.h) | ZLIB |**C/C++**|**1**| Math with C/OpenCL portability
math   | [nanoflann](https://github.com/jlblancoc/nanoflann)                  | BSD              | C++ |**1**| Build KD trees for point clouds
math   | [omm](https://github.com/Hectarea1996/omm)                           | MIT              | C++ |**1**| Template open multi-methods
math   | [OpenNL](https://github.com/BrunoLevy/geogram.psm.OpenNL)            | BSD3             | C++ |  2  | Linear and eigen solvers
math   | [par_msquares](https://prideout.net/marching-squares)                | MIT              |**C/C++**|**1**| Convert (binarized) image to triangles
math   | [par_shapes](https://prideout.net/shapes)                            | MIT              |**C/C++**|**1**| Generate various 3d geometric shapes
math   | [par_streamlines](https://prideout.net/blog/par_streamlines)         | MIT              |**C/C++**|**1**| Tessellate wide lines and curves with shading attributes
math   | [PoissonGenerator.h](https://github.com/corporateshark/poisson-disk-generator) | MIT    | C++ |**1**| Poisson disk points generator (disk or rect)
math   | [PolyPartition](https://github.com/ivanfratric/polypartition)        | MIT              | C++ |  2  | Polygon triangulation, partitioning
math   | [precision](https://github.com/possibly-wrong/precision)             | **PD**           | C++ | 3 | Arbitrary-precision integer and rational arithmetic
math   | [sdf.h](https://github.com/memononen/SDF)                            | MIT              |**C/C++**|**1**| Compute signed-distance field from antialiased image
math   | [ShaderFastLibs](https://github.com/michaldrobot/ShaderFastLibs)     | MIT              | C++ |**1**| (also HLSL) Approximate transcendental functions optimized for shaders (esp. GCN)
math   | [simple_linear_regression](https://github.com/torkeldanielsson/simple_linear_regression) | MIT |**C/C++**|**1**| Simple linear regression
math   | [simrank.hpp](https://github.com/roukaour/simrank)                   | MIT              | C++ |  2  | SimRank graph similarity algorithm
math   | [SummedAreaTable](https://github.com/corporateshark/Summed-Area-Table.git) | MIT        | C++ |**1**| Summed-Area Table generation and sum/avg queries
math   | [TinyExpr](https://github.com/codeplea/tinyexpr)                     | zlib             |**C**|  2  | Evaluation of math expressions from strings
math   | [Tomas Akenine-Moller snippets](https://tinyurl.com/ht79ndj)         | **PD**           |**C/C++**|  2  | Various 3D intersection calculations, not lib-ified
math   | [Voxelizer](https://github.com/karimnaaji/voxelizer)                 | MIT              |**C/C++**|**1**| Convert triangle mesh to voxel triangle mesh
math   | [xatlas](https://github.com/jpcy/xatlas)                             | MIT              | C++ |  2  | Mesh parameterization
mesh   | [cgltf](https://github.com/jkuhlmann/cgltf)                          | MIT              |**C**|**1**| GlTF 2.0 file loader
mesh   | [fast_obj.h](https://github.com/thisistherk/fast_obj)                | MIT              |**C**|**1**| Wavefront OBJ file loader
mesh   | [m3d.h](https://bztsrc.gitlab.io/model3d)                            | MIT              |**C/C++**|**1**| Model 3D importer/exporter (with Blender, Goxel, WebGL JS and assimp integration) |
mesh   | [objzero](https://github.com/jpcy/objzero)                           | MIT              |**C**|  2  | Wavefront OBJ file loader
mesh   | [qll_q3.h](https://github.com/dav64/qll)                             | **WTFPLv2**      | C++ |**1**| Quake3 BSP loader
mesh   | [tinyobjloader-c](https://github.com/syoyo/tinyobjloader-c)          | MIT              |**C**|**1**| Wavefront OBJ file loader
mesh   | [tinyobjloader](https://github.com/syoyo/tinyobjloader)              | MIT              | C++ |**1**| Wavefront OBJ file loader
mesh   | [tinyply](https://github.com/ddiakopoulos/tinyply)                   | **PD**           | C++ |  2  | PLY mesh file loader
mesh   | [tk_objfile](https://github.com/joeld42/tk_objfile)                  | MIT              |**C/C++**|**1**| OBJ file loader
misc   | [ASAP](https://github.com/mobius3/asap)                              | MIT              | C++ |**1**| Library for parsing, printing, iterating and operating on dates.
misc   | [Color-Toolkit](https://github.com/gerbenvoshol/Color-Toolkit)       | GPL2             |**C/C++**|**1**| Color conversion utils (RGB, XYZ, Lab, CIE76, CIE94 and CIEDE200)
misc   | [cpp-generators](https://github.com/c-smile/cpp-generators)          | BSD              | C++ |**1**| Generators in C++
misc   | [ebnn.h](https://github.com/kunglab/ebnn/blob/master/c/ebnn.h)       | MIT              |**C**|**1**| BNN (Binarized Neural Networks)
misc   | [h.h](https://github.com/robertsdotpm/h.h)                           | GPL3             |**C/C++**|**1**| Diverse utilities
misc   | [MakeID.h](https://www.humus.name/3D/MakeID.h)                       | **PD**           | C++ |**1**| Allocate/deallocate small integer IDs efficiently
misc   | [mmu](https://github.com/CN-xLeaves/mmu)                             | MIT              |**C**|  2  | Memory management and data structure toolset
misc   | [openGA](https://github.com/Arash-codedev/openGA)                    | MPL-2.0          | C++ |**1**| A C++ Generic Algorithm solver library
misc   | [PlusCallback](https://github.com/codeplea/pluscallback)             | zlib             | C++ |**1**| Function/method callbacks
misc   | [QR-Code-generator](https://github.com/nayuki/QR-Code-generator)     | MIT              |**C**|  2  | QR Code generator
misc   | [qsort](https://github.com/svpv/qsort)                               | MIT              |**C**|**1**| Qsort algorithm as a C macro
misc   | [scogem.c](https://github.com/zzo38/scorpion/blob/trunk/scogem.c)    | **PD**           |**C**|  2  | URL parser
misc   | [smallxrm.c](https://github.com/zzo38/freeheromesh/blob/trunk/smallxrm.c) | **PD**      |**C**|  2  | Implementation of X resource manager
misc   | [stmr](https://github.com/wooorm/stmr.c)                             | MIT              |**C**|  2  | Extract English word stems
misc   | [x.h](https://github.com/Neur1n/x.h)                                 | Mulan2           |**C/C++**|**1**| Cross-platform C/C++ utilities
nav    | [m_path_finding.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_path_finding.h) | ZLIB |**C/C++**|**1**| Floodfill-based path finding
nav    | [micropather](https://www.grinninglizard.com/MicroPather/)           | zlib             | C++ |  2  | Pathfinding with A\*
net    | [civetweb](https://github.com/civetweb/civetweb)                     | MIT              |**C/C++**|  2  | HTTP server, fork of Mongoose
net    | [cpp-httplib](https://github.com/yhirose/cpp-httplib)                | MIT              |**C/C++**|**1**| Cross-platform HTTP server/client
net    | [enet](https://github.com/zpl-c/enet)                                | MIT              |**C/C++**|**1**| Reliable UDP networking library
net    | [EWS](https://github.com/hellerf/EmbeddableWebServer)                | BSD              |**C/C++**|**1**| HTTP server
net    | [happyhttp](https://github.com/mingodad/HappyHTTP)                   | zlib             | C++ |  2  | HTTP client requests
net    | [libcluon](https://github.com/chrberger/libcluon)                    | MPL-2.0          | C++ |**1**| Cross-platform socket wrapper and data marshalling with native implementations for [Protobuf](https://developers.google.com/protocol-buffers/), [LCM](https://lcm-proj.github.io/type_specification.html)/[ZCM](https://zerocm.github.io/zcm/), JSON, and [MsgPack](https://msgpack.org) serialization/deserialization
net    | [librg](https://github.com/zpl-c/librg)                              | BSD3             |**C/C++**|**1**| World/entity synchronization multiplayer library
net    | [LUrlParser](https://github.com/corporateshark/LUrlParser)           | MIT              | C++ |  2  | Lightweight URL & URI parser RFC 1738, RFC 3986
net    | [mongoose](https://github.com/cesanta/mongoose)                      | GPLv2            |**C/C++**|  2  | HTTP server
net    | [netq](https://gitlab.com/bztsrc/netq)                               | MIT              |**C**|**1**| Reliable datagram library
net    | [par_easycurl.h](https://github.com/prideout/par)                    | MIT              |**C/C++**|**1**| CURL wrapper
net    | [simpletls.c](https://github.com/zzo38/scorpion/blob/trunk/simpletls.c) | **PD**        |**C**|  2  | Function to create a socket and connect to a remote server with TLS
net    | [tiniest-analytics](https://github.com/Pintea/tiniest-analytics)     | MIT              | C++ |  2  | Cross-platform analytics for games (using Google Analytics <4)
net    | [tiny-MQTT-c](https://github.com/kokke/tiny-MQTT-c)                  | **PD**           |**C**| 2(4)                   | Small implementation of (some of) the MQTT protocol in C
net    | [tlse](https://github.com/eduardsui/tlse)                            | **PD/BSD2**      |**C**|  2  | TLS v1.0, 1.2, 1.3 and DTLS 1.0, 1.2 implementations
net    | [webster](https://github.com/brunexgeek/webster)                     | Apache2          | C++ |  2  | Standalone HTTP server/client
net    | [yocto](https://github.com/tom-seddon/yhs)                           | **PD**           |**C/C++**|  2  | Non-production-use HTTP server
net    | [znet](https://github.com/starwing/znet)                             | MIT              |**C/C++**|**1**| Cross-platform networking w/ Lua binding
pack   | [dmc_unrar](https://github.com/DrMcCoy/dmc_unrar)                    | GPLv2+           |**C/C++**|**1**| RAR file decompression
pack   | [fastlz](https://code.google.com/archive/p/fastlz/source/default/source) | MIT          |**C/C++**|  2  | Fast but larger LZ compression
pack   | [lz4](https://github.com/lz4/lz4)                                    | BSD              |**C/C++**|  2  | Fast but larger LZ compression
pack   | [microtar](https://github.com/rxi/microtar)                          | MIT              |**C/C++**|  2  | Lightweight tar library
pack   | [miniz.c](https://github.com/richgel999/miniz)                       | MIT              |**C/C++**|**1**| Compression, decompression, ZIP file, PNG writing
pack   | [pithy](https://github.com/johnezang/pithy)                          | BSD              |**C/C++**|  2  | Fast but larger LZ compression
pack   | [rle](https://gitlab.com/bztsrc/rle)                                 | MIT              |**C**|**1**| Run-length en/decoder
parse  | [cmp](https://github.com/camgunz/cmp)                                | MIT              |**C/C++**|  2  | MessagePack parser and serializer
parse  | [cpp-peglib](https://github.com/yhirose/cpp-peglib)                  | MIT              |**C/C++**|**1**| PEG (Parsing Expression Grammars) library
parse  | [html-parse.c](https://git.savannah.gnu.org/cgit/wget.git/tree/src/html-parse.c)  | GPL |**C**|  2  | HTML parser (wget)
parse  | [SLRE](https://github.com/cesanta/slre)                              | GPLv2            |**C/C++**|**1**| Regular expression matcher
parse  | [tok](https://gitlab.com/bztsrc/tok)                                 | MIT              |**C**|**1**| Configurable tokenizer
parse  | [tomlplusplus](https://github.com/marzer/tomlplusplus)               | MIT              | C++ |**1**| TOML parser and serializer 
parse  | [udisasm](https://gitlab.com/bztsrc/udisasm)                         | MIT              |**C/C++**|**1**| Extremely small disassembler for ARMv8.2 AArch64 (~65k) |
parse  | [Unformat](https://github.com/adamyaxley/Unformat)                   | **PD**           | C++ |**1**| Parses formatted strings (reverse of std::format)
prng   | [random](https://github.com/effolkronium/random)                     | MIT              | C++ |**1**| Convenient API for random
prng   | [SimplexNoise](https://github.com/simongeilfus/SimplexNoise)         | BSD2             | C++ |**1**| Collection of noise generators
profile| [MicroProfile](https://github.com/jonasmr/microprofile)              | **PD**           | C++ | 2-4 | CPU (and GPU?) profiler, 1-3 header files, uses miniz internally
profile| [prof](https://github.com/cyrus-and/prof)                            | MIT              |**C/C++**|**1**| Profiler for Linux
profile| [Remotery](https://github.com/Celtoys/Remotery)                      | Apache2          |**C/C++**|  2  | CPU/GPU profiler Win/Mac/Linux, using web browser for viewer
raster | [canvas_ity](https://github.com/a-e-k/canvas_ity)                    | ISC              | C++ |**1**| 2D rasterizer
script | [Duktape](https://duktape.org/)                                      | MIT              |**C**|  2  | Embeddable JavaScript engine
script | [LIL](https://runtimeterror.com/tech/lil/)                           | zlib             |**C/C++**|  2  | Interpreter for a Tcl-like scripting language
script | [lualite](https://github.com/user1095108/lualite)                    | MIT              | C++ |**1**| Generate Lua bindings in C++
script | [minilua](https://github.com/edubart/minilua)                        | MIT              |**C/C++**|**1**| Single-file port of Lua scripting language
script | [MY-BASIC](https://github.com/paladin-t/my_basic/)                   | MIT              |**C**|  2  | Interpreter for a BASIC dialect scripting language
script | [Picol](https://chiselapp.com/user/dbohdan/repository/picol/)        | BSD              |**C/C++**|**1**| Interpreter for a Tcl-like scripting language
script | [s7](https://ccrma.stanford.edu/software/snd/snd/s7.html)            | BSD              |**C/C++**|  2  | Interpreter for a subset of Scheme (R5RS/R7RS)
serial | [archive](https://github.com/voidah/archive)                         |**PD**            | C++ |**1**| Binary serialize & deserlize w/ STL support
serial | [blob_tree](https://github.com/dicroce/blob_tree)                    | MIT              | C++ |**1**| Binary tree serializer
serial | [cista](https://github.com/felixguendling/cista)                     |MIT               | C++ |**1**| Cross-platform high performance zero copy C++17 serialization/deserialization
serial | [libcluon](https://github.com/chrberger/libcluon)                    | MPL-2.0          | C++ |**1**| Cross-platform data serialization/deserialization with native implementations for [Protobuf](https://developers.google.com/protocol-buffers/), [LCM](https://lcm-proj.github.io/type_specification.html)/[ZCM](https://zerocm.github.io/zcm/), JSON, and [MsgPack](https://msgpack.org)
serial | [qserial](https://github.com/earonesty/qserial)                      | BSD3             | C++ |**1**| Schema-driven serialization library
serial | [visit_struct](https://github.com/cbeck88/visit_struct)              | Boost            | C++ |  2  | Struct-field reflection
string | [csplit](https://github.com/jwlodek/csplit)                          | MIT              |**C/C++**|**1**| String splitting and processing single-header library
string | [dfa](https://bjoern.hoehrmann.de/utf-8/decoder/dfa/)                | MIT              |**C/C++**|  2  | Fast UTF-8 decoder (need a header file)
string | [ggformat](https://github.com/mikejsavage/ggformat)                  | ISC              | C++ |  2  | Printf replacement
string | [inja.hpp](https://github.com/pantor/inja)                           | MIT              | C++ |**1**| Template engine
string | [levenshtein](https://github.com/wooorm/levenshtein.c)               | MIT              |**C/C++**|  2  | Compute edit distance between two strings
string | [Obfuscate](https://github.com/adamyaxley/Obfuscate)                 | **PD**           | C++ |**1**| Guaranteed compile-time string literal obfuscation library for C++14
string | [Str.h](https://github.com/ocornut/Str)                              | **PD**           | C++ |**1**| Simple C++ string type with an optional local buffer
string | [str](https://github.com/maxim2266/str)                              | BSD              |**C**|  2  | Yet another string library for C language
string | [str_view.hpp](https://github.com/sawickiap/str_view)                | MIT              | C++ |**1**| Null-termination-aware string-view class
string | [tinyformat](https://github.com/c42f/tinyformat)                     | Boost            | C++ |**1**| Typesafe printf
svg    | [SimpleSVG](https://github.com/adishavit/simple-svg)                 | BSD3             | C++ |**1**| Easy to use SVG library
sys    | [cpuid](https://github.com/anzz1/cpuid)                              | ??               |**C/C++**|**1**| Cross-platform cpuid intrinsic
sys    | [iathook](https://github.com/anzz1/iathook)                          | ??               |**C/C++**|**1**| Import address table hooking library (x86/x64,w32)
sys    | [JArgsParser](https://github.com/ZhengqiaoWang/JArgsParser)          | MIT              | C++ |**1**| Arguments parser
sys    | [openmodal](https://gitlab.com/bztsrc/openmodal)                     | MIT              |**C**|**1**| Native file modals
sys    | [rang](https://github.com/agauniyal/rang)                            | **PD**           | C++ |**1**| Cross-platform colored console text
sys    | [xproc](https://github.com/time-killer-games/xproc)                  | MIT              | C++ |  2  | Foreign Process Information
thread | [bikeshed.h](https://github.com/DanEngelbrecht/bikeshed)             | MIT              |**C/C++**|**1**| Cross-platform lock free fixed memory hierarchical work scheduler
thread | [cds_job](https://github.com/cdwfs/cds_job)                          | **PD**           | C++ |**1**| Lock-free job queue
thread | [TinyCThread](https://tinycthread.github.io/)                        | zlib             |**C/C++**|  2  | Cross-platform implementation of the C11 Threads API
thread | [TinyThread++](https://tinythreadpp.bitsnbites.eu/)                  | zlib             | C++ |  2  | Cross-platform implementation of the C++11 Threads API
ui     | [Clay](https://github.com/nicbarker/clay)                            | ZLIB             |**C/C++**|**1**| High performance 2D UI layout library
ui     | [dear imgui](https://github.com/ocornut/imgui)                       | MIT              | C++ |  9  | An immediate-mode GUI formerly named "ImGui"; [3rd-party C wrapper](https://github.com/Extrawurst/cimgui)
ui     | [linenoise](https://github.com/antirez/linenoise)                    | BSD              |**C/C++**|  2  | Terminal readline w/ history etc
ui     | [tinyfiledialogs](https://sourceforge.net/projects/tinyfiledialogs/) | ZLIB             |**C/C++**|  2  | Modal dialogs inc. file open/save (Win/Mac/Linux)
ui     | [wcwidth9](https://github.com/joshuarubin/wcwidth9)                  | Apache2          |**C**|**1**| Platform independent wcwidth with full unicode 9 support
ui     | [webview](https://github.com/zserge/webview)                         | MIT              |**C/C++**|**1**| Cross-platform webview library
unit   | [catch2](https://github.com/catchorg/Catch2/)                        | Boost            | C++ |**1**| Unit testing
unit   | [catch](https://github.com/philsquared/Catch)                        | Boost            | C++ |**1**| Unit testing
unit   | [clove-unit](https://github.com/fdefelici/clove-unit)                | MIT              |**C**|**1**| Unit testing
unit   | [doctest](https://github.com/onqtam/doctest)                         | MIT              | C++ |**1**| Unit testing
unit   | [fctx](https://github.com/imb/fctx)                                  | BSD              |**C/C++**|**1**| Unit testing
unit   | [greatest](https://github.com/silentbicycle/greatest)                | ISC              |**C**|**1**| Unit testing
unit   | [hippomocks](https://github.com/dascandy/hippomocks)                 | LGPL             | C++ |**1**| Unit testing
unit   | [minctest](https://github.com/codeplea/minctest)                     | ZLIB             |**C**|**1**| Unit testing
unit   | [munit](https://github.com/nemequ/munit)                             | MIT              |**C**|**1**| Unit testing
unit   | [picotest](https://github.com/colinbarry/picotest)                   | MIT              |**C/C++**|**1**| Unit testing
unit   | [SPUT](https://www.lingua-systems.com/unit-testing/)                 | BSD              |**C/C++**|**1**| Unit testing
unit   | [trompeloeil](https://github.com/rollbear/trompeloeil)               | Boost            | C++ |**1**| Unit testing
unit   | [utest](https://github.com/evolutional/utest)                        | MIT              |**C/C++**|**1**| Unit testing
uuid   | [uuid4](https://github.com/gpakosz/uuid4)                            | MIT/**WTFPLv2**  |**C/C++**|  2  | UUID v4 generator
uuid   | [uuid_h](https://github.com/wc-duck/uuid_h)                          | ZLIB             |**C/C++**|**1**| UUID generator
vector | [algebra3.h](https://www.animats.com/source/graphics/algebra3.h)     | **PD**           | C++ |**1**| Vector utilities for 2, 3, and 4 element vectors, all inline
vector | [hypatia](https://github.com/dagostinelli/hypatia)                   | MIT              |**C**|**1**| Vector/matrix/quaternion math
vector | [linalg.h](https://github.com/sgorsten/linalg)                       | **PD**           | C++ |**1**| Vector/matrix/quaternion math
vector | [linalg](https://github.com/ilyak/linalg)                            | ISC              |**C/C++**|**1**| Vector/matrix/quaternion math
video  | [pl_mpeg](https://github.com/phoboslab/pl_mpeg)                      | MIT              |**C**|**1**| MPEG1 video and audio decoder
xml    | [pugixml](https://pugixml.org/)                                      | MIT              | C++ |  2  | Light-weight C++ XML processing library
xml    | [tinyxml2](https://github.com/leethomason/tinyxml2)                  | zlib             | C++ |  2  | Simple, small, efficient, C++ XML parser
xml    | [yxml](https://dev.yorhel.nl/yxml)                                   | MIT              |**C**|  2  | Small, fast and correct XML parser
yaml   | [mini-yaml](https://github.com/jimmiebergmann/mini-yaml)             | MIT              | C++ |  2  | YAML parser and serializer

<!-- todo

https://github.com/avivbeeri/abc - check branches
https://github.com/stevenlr/Flint - waiting for a 2nd header
https://github.com/azmr/sweet - NO license

https://github.com/983/df
https://github.com/983/fft
https://github.com/andrewwillmott/colour-blind-luts
https://github.com/bqqbarbhg/bq_websocket
https://github.com/jarikomppa/ipc
https://github.com/joric/joirc
https://github.com/schellingb/c-data-structures
https://github.com/ufbx/ufbx
https://github.com/wangyi-fudan/wyhash
https://github.com/wangyi-fudan/wyHLL
https://github.com/willemt/raft_amalgamation
https://github.com/willemt/splay-tree
https://github.com/willemt/yabtorrent
https://github.com/xtopher-xyz/xrns-player

-->

## *List FAQ*

### Can I link directly to this list?

Yes. For historical reasons, [this is the preferred link.](https://github.com/nothings/single_file_libs)

### Why isn't library XXX which is made of 3 or more files on this list?

We draw the line arbitrarily at 2 files at most. Some of these libraries are still easy to drop into
your project and build, so you might still be ok with them. But since people come to stb for single-file
public domain libraries, we feel that starts to get too far from what we do here.

### Why isn't library XXX which is at most two files and has minimal other dependencies on this list?

Probably because we don't know about it, feel free to submit a pull request or issue (it can be your
own library or somebody else's). But we might not include it for various other reasons, including
subtleties of what is 'minimal other dependencies' and subtleties about what is 'lightweight'.

### What are the differences between C, C++ and C/C++ in the API column?

For the API column, "C" means C only, "C++" means C++ only, and "C/C++" means C/C++ usable
from either; some files may require *building* as C or C++ but still qualify as "C/C++" as
long as the header file uses `extern "C"` to make it work. (In some cases, a header-file-only
library may compile as both C or C++, but produce an implementation that can only be called from
one or the other, because of a lack of use of `extern "C"`; in this case the table still qualifies it
as C/C++, as this is not an obstacle to most users.)

### Why are the LICENSING terms required in the header and source files?

Please note that every file that must be included in a user's project counts; a header and a source
file is 2 files, but a header file, source file, and LICENSE (if the license isn't in the
source file) is 3 files, and won't be accepted, because it's not 2 files. But actually
'LICENSE' is a problem for just dropping the library in a source tree anyway, since it's
not scoped to just the library, so library authors are encouraged to include the license in the
source file and not require a separate LICENSE.

### Why isn't SQLite's amalgamated build on this list?

Come on.
