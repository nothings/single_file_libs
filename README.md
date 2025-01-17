# Single-file public-domain/open source libraries with minimal dependencies

I am the author of a large number of [single-file C/C++ public domain libraries](https://github.com/nothings/stb).
I am not the only person who writes libraries like this, so below are other, similar libraries.

Generally, the following is a list of small, easy-to-integrate, portable libraries
which are usable from C and/or C++, and should be able to be compiled on both
32-bit and 64-bit platforms. However, I have not personally verified that any
specific lilbrary is as advertised, or is quality software.

### Rules

- Libraries must be usable from C or C++, ideally both
- Libraries should be usable from more than one platform (ideally, all major desktops and/or all major mobile)
- Libraries should compile and work on both 32-bit and 64-bit platforms
- Libraries should use at most two files (one header, one source)

Exceptions will be allowed for good reasons.

### Recent additions

Recent additions are marked with an asterisk in the left column.

### New libraries and corrections

See discussion after the list.

### JSON Parsing

There are a lot of JSON parsers listed here. For some analysis and performance
results, check out https://github.com/miloyip/nativejson-benchmark

### Other lists

Also you might be interested in other related, but different lists:

- [clib](https://github.com/clibs/clib/wiki/Packages): list of (mostly) small single C functions (licenses not listed)
- [CCAN](https://ccodearchive.net/list.html): package of lots of shareable C functions (mixed licenses)

### Library listing

**Public domain single-file libraries usable from C and C++ are in bold.** Other
libraries are either non-public domain, or two files, or not usable from both C and C++, or
all three. Libraries of more than two files are mostly forbidden.

For the API column, "C" means C only, "C++" means C++ only, and "C/C++" means C/C++ usable
from either; some files may require *building* as C or C++ but still qualify as "C/C++" as
long as the header file uses `extern "C"` to make it work. (In some cases, a header-file-only
library may compile as both C or C++, but produce an implementation that can only be called from
one or the other, because of a lack of use of `extern "C"`; in this case the table still qualifies it
as C/C++, as this is not an obstacle to most users.)

### Categories:

  - general purpose
    - [data structures](#data-structures)
    - [string processing](#strings)
    - [scripting](#scripting)
    - [hashing](#hashing)
  - mathematics
    - [vector math](#vectors)
    - [geometry math](#geometry-math)
    - [general math](#math)
  - parsing
    - [JSON](#json)
    - [YAML](#yaml)
    - [CSV](#csv)
    - [other serialization](#serialization)
    - [argv argument processing](#argv)
    - [other parsing](#parsing)
  - graphics
    - [textmode](#graphics-text)
    - [2D graphics](#graphics-2d)
    - [3D graphics](#graphics-3d)
    - [3D geometry file processing](#geometry-file)
    - [image loading, saving, & processing](#images)
  - audio/video/data compression
    - [compression](#compression)
    - [audio processing & files](#audio)
    - [video](#video)
  - [videogames](#videogames)
  - operating system features
    - [files and filenames](#files--filenames)
    - [multithreading](#multithreading)
    - [networking](#network)
    - [hardware interfacing](#hardware)
  - debugging, profiling, testing
    - [debugging](#debugging)
    - [profiling](#profiling)
    - [unit testing etc.](#unit-testing)
  - other
    - [AI](#ai)
    - [cryptography](#crypto)
    - [state machines](#state-machines)
    - [user interface](#user-interface)
    - [miscellaneous](#miscellaneous)

# AI
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
| [Genann](https://github.com/codeplea/genann)                          | zlib                 |C/C++|  2  | simple neural networks (ANN)
| [KANN](https://github.com/attractivechaos/kann)                       | MIT                  |C/C++|  2  | automatic differentiation (2 files)
| [micropather](http://www.grinninglizard.com/MicroPather/)             | zlib                 | C++ |  2  | pathfinding with A\*

# argv
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [Argh!](https://github.com/adishavit/argh)                           | BSD                  | C++ |**1**| command-line argument parsing
|  [Clara](https://github.com/catchorg/Clara)                           | Boost                | C++ |**1**| composable, command line parser for C++ 11 and beyond
|  [CLI11](https://github.com/CLIUtils/CLI11)                           | BSD                  | C++ |**1**| Feature-rich CLI parsing in modern C++11
|  [cmdline](https://github.com/tanakh/cmdline)                         | BSD                  | C++ |**1**| command-line argument parsing
|  [flags](https://github.com/sailormoon/flags)                         | **public domain**    | C++ |**1**| command-line argument parsing
|  [getops.hpp](https://github.com/burner/sweet.hpp/getopts.hpp)        | LGPL3                | C++ |**1**| command-line argument parsing for C++ 11 and beyond
|  [kgflags](https://github.com/kgabis/kgflags)                         | MIT                  |C/C++|**1**| command-line argument parsing
|  [linkom](https://github.com/hernandp/linkom)                         | MIT                  |C/C++|**1**| command-line argument parsing w/ DOS-style options
|  [optionparser](http://optionparser.sourceforge.net/)                 | MIT                  | C++ |**1**| command-line argument parsing
|  [parg](https://github.com/jibsen/parg)                               | **public domain**    |  C  |  2  | command-line argument parsing
|  [ProgramOptions.hxx](https://github.com/Fytch/ProgramOptions.hxx)    | MIT                  | C++ |**1**| command-line argument parsing

# audio
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [aw_ima.h](https://github.com/afterwise/aw-ima/blob/master/aw-ima.h) | MIT                  |C/C++|**1**| IMA-ADPCM audio decoder
|  [btac1c](https://github.com/cr88192/bgbtech_misc/blob/master/mini/btac1c_mini0.h)| MIT      |C/C++|**1**| MS-IMA_ADPCM variant
|**[dr_flac](https://github.com/mackron/dr_libs)**                      | **public domain**    |C/C++|**1**| FLAC audio decoder
|**[dr_wav](https://github.com/mackron/dr_libs)**                       | **public domain**    |C/C++|**1**| WAV audio loader
|  [Geneva](https://github.com/KrzysztofSzewczyk/Geneva)                | MIT                  |C/C++|**1**| Library generating 8-bit waveforms of various kinds
|  [minimp3](https://github.com/lieff/minimp3)                          | CC0                  |  C  |**1**| Minimalistic MP3 decoder with sse/neon support
|**[miniaudio](https://github.com/dr-soft/miniaudio)**                  | **public domain**    |C/C++|**1**| Audio playback and capture library
|  [pocketmod](https://github.com/rombankzero/pocketmod)                | MIT                  |C/C++|**1**| ProTracker MOD file renderer
|**[sts_mixer](https://github.com/kieselsteini/sts)**                   | **public domain**    |C/C++|**1**| simple stereo audio mixer
|  [tinysound](https://github.com/RandyGaul/tinyheaders)                | zlib                 |C/C++|**1**| direct sound audio mixer & WAV loader
|  [TinySoundFont](https://github.com/schellingb/TinySoundFont)         | MIT                  |C/C++|**1**| SoundFont2 loader & synthesizer

# compression
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [dmc_unrar](https://github.com/DrMcCoy/dmc_unrar)                    | GPLv2+               |C/C++|**1**| RAR file decompression
|  [fastlz](https://code.google.com/archive/p/fastlz/source/default/source) | MIT              |C/C++|  2  | fast but larger LZ compression
|  [lz4](https://github.com/lz4/lz4)                                    | BSD                  |C/C++|  2  | fast but larger LZ compression
|**[miniz.c](https://github.com/richgel999/miniz)**                     | MIT                  |C/C++|**1**| compression, decompression, ZIP file, PNG writing
|  [microtar](https://github.com/rxi/microtar)                          | MIT                  |C/C++|  2  | lightweight tar library
|  [pithy](https://github.com/johnezang/pithy)                          | BSD                  |C/C++|  2  | fast but larger LZ compression
|  [rle](https://gitlab.com/bztsrc/rle)                                 | MIT                  |C    |**1+1**| extremely simple run-length encoder/decoder |

# crypto
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [ggentropy](https://github.com/mikejsavage/ggentropy)                | ISC                  | C++ |  2  | cross platform entropy library
|  [Monocypher](https://monocypher.org)                                 | **public domain**    |  C  |  2  | high-quality small cryptography library
|  [TweetNaCl](http://tweetnacl.cr.yp.to/software.html)                 | **public domain**    |  C  |  2  | high-quality tiny cryptography library

# data structures
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|**[aArray](https://tse.gratis/aArray/)**                               | **public domain**    |  C  |**1**| Arrays/strings: generic, safe
|  [avl](https://github.com/etherealvisage/avl)                         | **public domain**    |C/C++|  2  | AVL tree
|  [bitset.hpp](https://github.com/burner/sweet.hpp/bitset.hpp)         | LGPL3                | C++ |**1**| Compile time sided bit set for C++11 and beyond
|  [c-bool-value](https://github.com/lduck11007/c-bool-value)           | **WTFPLv2**          |C/C++|  1  | Simple and easy boolean values in standard c
|**[DG_dynarr.h](https://github.com/DanielGibson/Snippets/)**           | **public domain**    |C/C++|**1**| typesafe dynamic arrays (like std::vector) for plain C
|  [DynaVar](https://github.com/ArjArav98/DynaVar)                      | GPL-3.0              | C++ |  1  | Object which can store any type of primitive data type
|  [fector.hpp](https://github.com/burner/sweet.hpp/fector.hpp)         | LGPL3                | C++ |**1**| A fixed size std::vector like structure
|  [itlib](https://github.com/iboB/itlib)                               | MIT                  | C++ |**1**| several C++11 standard-contaner-like libraries and helpers
|  [klib](http://attractivechaos.github.io/klib/)                       | MIT                  |C/C++|  2  | many 2-file libs: hash, sort, b-tree, etc
|  [LinkedList](https://github.com/ivanseidel/LinkedList)               | MIT                  |C/C++|  2  | Linked list C++ 
|  [libpqueue](https://github.com/vy/libpqueue)                         | BSD                  |C/C++|  2  | priority queue (heap)
|  [minilibs](https://github.com/ccxvii/minilibs)                       | **public domain**    |  C  |  2  | two-file binary tress (also regex, etc)
|  [PackedArray](https://github.com/gpakosz/PackedArray)                | **WTFPLv2**          |  C  |  2  | memory-efficient array of elements with non-pow2 bitcount
|  [simclist](http://mij.oltrelinux.com/devel/simclist)                 | BSD                  |C/C++|  2  | linked-list
|  [selist](https://github.com/ennorehling/clibs)                       | ISC                  |C/C++|  2  | space-efficient linked-list
|  [trie.hpp](https://github.com/burner/sweet.hpp/trie.hpp)             | LGPL3                | C++ |**1**| A trie (prefix tree) implementation for C++11
|  [mempool](https://github.com/hardikp/cpp-mempool)                    | MIT                  | C++ |**1**| Efficient minimal memory pool implementation for C++
|  [uthash](https://github.com/troydhanson/uthash)                      | BSD                  |C/C++|  2  | several 1-header, 1-license-file libs: generic hash, list, etc
|  [px_mem.h](https://github.com/pplux/px/blob/master/px_mem.h)         | MIT                  | C++ |  1  | Safe memory managemnt constructs for C++

# debugging
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [dbgtools](https://github.com/wc-duck/dbgtools)                      | zlib                 |C/C++|  2  | cross-platform debug util libraries
|  [debug-assert](https://github.com/foonathan/debug_assert)            | zlib                 | C++ |**1**| modular assertion macro
|  [debugbreak](https://github.com/scottt/debugbreak)                   | BSD                  |C/C++|**1**| programmatic debug break
|  [log.hpp](https://github.com/burner/sweet.hpp/log.hpp)               | LGPL3                | C++ |**1**| multi threaded simple C++11 and beyond logger
|  [loguru](https://github.com/emilk/loguru)                            | **public domain**    | C++ |**1**| flexible logging
|  [pempek_assert.cpp](https://github.com/gpakosz/Assert)               | **WTFPLv2**          | C++ |  2  | flexible assertions

# files & filenames
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|**[DG_misc.h](https://github.com/DanielGibson/Snippets/)**             | **public domain**    |C/C++|**1**| Daniel Gibson's stb.h-esque cross-platform helpers: path/file, strings
|  [dirent](https://github.com/tronkko/dirent)                          | MIT                  |C/C++|**1**| dirent for Windows: retrieve file & dir info
|  [tfile](https://github.com/rec/tfile)                                | MIT                  |C++|**1**| FILE* wrapper does read-write-append-seek-close (Win/Mac/Unix)
|  [TinyDir](https://github.com/cxong/tinydir)                          | BSD                  |  C  |**1**| cross-platform directory reading (Win/POSIX/MinGW)
|  [tinyfiles](https://github.com/RandyGaul/tinyheaders)                | zlib                 |C/C++|**1**| cross-platform directory reading (Win/Mac/Unix)
|  [whereami](https://github.com/gpakosz/whereami)                      | **WTFPLv2**          |C/C++|  2  | get path/filename of executable or module

# geometry file
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [cgltf](https://github.com/jkuhlmann/cgltf)                          | MIT                  |  C  |**1**| glTF 2.0 file loader
|  [fast_obj.h](https://github.com/thisistherk/fast_obj)                | MIT                  |  C  |**1**| wavefront OBJ file loader
|  [objzero](https://github.com/jpcy/objzero)                           | MIT                  |  C  |  2  | wavefront OBJ file loader
|  [tinyply](https://github.com/ddiakopoulos/tinyply)                   | **public domain**    | C++ |  2  | PLY mesh file loader
|  [tinyobjloader](https://github.com/syoyo/tinyobjloader)              | MIT                  | C++ |**1**| wavefront OBJ file loader
|  [tinyobjloader-c](https://github.com/syoyo/tinyobjloader-c)          | MIT                  |  C  |**1**| wavefront OBJ file loader
|  [tk_objfile](https://github.com/joeld42/tk_objfile)                  | MIT                  |C/C++|**1**| OBJ file loader
|  [yocto_obj.h](https://github.com/xelatihy/yocto-gl)                  | MIT                  |C/C++|**1**| wavefront OBJ file loader
|  [m3d.h](https://bztsrc.gitlab.io/model3d)                            | MIT                  |C/C++|**1**| Model 3D importer/exporter (with Blender, Goxel, WebGL JS and assimp integration) |
|  [qll_q3.h](https://github.com/dav64/qll)                             | **WTFPLv2**          | C++ |**1**| Quake3 BSP loader

# geometry math
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [Clipper](http://www.angusj.com/delphi/clipper.php)                  | Boost                | C++ |  2  | line & polygon clipping & offsetting
|**[df](https://github.com/983/df)**                                    | **public domain**    |C/C++|**1**| find voronoi region in linear time of size of lattice
|  [jc_voronoi](https://github.com/JCash/voronoi)                       | MIT                  |C/C++|**1**| find voronoi regions on float/double data
|  [nanoflann](https://github.com/jlblancoc/nanoflann)                  | BSD                  | C++ |**1**| build KD trees for point clouds
|**[nv_voronoi.h](http://www.icculus.org/~mordred/nvlib/)**             | **public domain**    |C/C++|**1**| find voronoi regions on lattice w/ integer inputs
|  [par_msquares](https://prideout.net/marching-squares)                | MIT                  |C/C++|**1**| convert (binarized) image to triangles
|  [par_shapes](https://prideout.net/shapes)                            | MIT                  |C/C++|**1**| generate various 3d geometric shapes
|  [par_streamlines](https://prideout.net/blog/par_streamlines)         | MIT                  |C/C++|**1**| tessellate wide lines and curves with shading attributes
|  [PolyPartition](https://github.com/ivanfratric/polypartition)        | MIT                  | C++ |  2  | polygon triangulation, partitioning
|**[rjm_mc.h](https://github.com/rmitton/rjm)**                         | **public domain**    |C/C++|**1**| marching cubes triangulator
|**[sobol.h](https://github.com/Marc-B-Reynolds/Stand-alone-junk/)**    | **public domain**    |C/C++|**1**| sobol & stratified sampling sequences
|  [sdf.h](https://github.com/memononen/SDF)                            | MIT                  |C/C++|**1**| compute signed-distance field from antialiased image
|  [Tomas Akenine-Moller snippets](http://tinyurl.com/ht79ndj)          | **public domain**    |C/C++|  2  | various 3D intersection calculations, not lib-ified
|  [Voxelizer](https://github.com/karimnaaji/voxelizer)                 | MIT                  |C/C++|**1**| convert triangle mesh to voxel triangle mesh
|  [xatlas](https://github.com/jpcy/xatlas)                             | MIT                  | C++ |  2  | mesh parameterization
|  [yocto_bvh.h](https://github.com/xelatihy/yocto-gl)                  | MIT                  |C/C++|**1**| ray-casting and closest-element queries of bounding-volume hierarchy
|  [yocto_shape.h](https://github.com/xelatihy/yocto-gl)                | MIT                  |C/C++|**1**| shape generation, tesselation, normals, etc.

# graphics (text)
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [rang](https://github.com/agauniyal/rang)                            | **public domain**    | C++ |**1**| cross-platform colored console text
|  [ssfn.h](https://gitlab.com/bztsrc/scalable-font)                    | MIT                  |C/C++|**1**| scalable/bitmap/pixmap font renderer |

# graphics (2d)
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [blendish](https://hg.sr.ht/~duangle/oui-blendish)                   | MIT                  |C/C++|  1  | blender-style widget rendering using NanoVG
|  [Cimg](http://cimg.eu/)                                              | CeCILL/CeCILL-C      | C++ |**1**| image processing toolkit (60K LoC)
|  [Immediate2D](https://github.com/npiegdon/immediate2d)               | **public domain**    | C++ |  2  | zero-configuration, immediate-mode 2D graphics for Windows
|  [noc_turtle](https://github.com/guillaumechereau/noc)                | MIT                  |C/C++|  2  | procedural graphics generator
|  [tigr](https://bitbucket.org/rmitton/tigr/src)                       | **public domain**    |C/C++|  2  | quick-n-dirty window text/graphics for Windows and macOS
|  [RGL](https://github.com/ColleagueRiley/RGL)                          | zlib                 |C/C++|  1  | Simple ultra-lightweight OpenGL version abstraction based on RLGL (pipeline system)
|  [RFont](https://github.com/ColleagueRiley/RFont)                        | zlib                 |C/C++|  1  | Simple-to-use lightweight single header modular font rendering library
|  [wfc](https://github.com/krychu/wfc)                                 | MIT                  |  C  |**1**| generate image locally similar to the input image using WFC algorithm

# graphics (3d)
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [debug-draw](https://github.com/glampert/debug-draw)                 | **public domain**    | C++ |**1**| API-agnostic immediate-mode debug rendering
|**[lightmapper](https://github.com/ands/lightmapper#lightmapper)**     | **public domain**    |C/C++|**1**| use your OpenGL renderer to offline bake lightmaps
|  [mikktspace](https://developer.blender.org/diffusion/B/browse/master/intern/mikktspace)| zlib|C/C++| 2  | compute tangent space for normal mapping
|  [rjm_raytrace.h](https://github.com/rmitton/rjm)                     | **public domain**    |C/C++|**1**| minimalistic SSE packet raytracer for offline baking
|**[seamoptimizer](https://github.com/ands/seamoptimizer)**             | **public domain**    |C/C++|**1**| modify lightmap data to hide seams
|[Simple OpenGL Loader](https://github.com/tsherif/simple-opengl-loader)| MIT                  |C/C++|**1**| extensible, cross-platform OpenGL loader
|  [small3dlib](https://gitlab.com/drummyfish/small3dlib)               | CC0 + patent waiver  |C/C++|**1**| fast and portable software renderer
|  [sokol_gfx.h](https://github.com/floooh/sokol)                       | MIT                  |C/C++|**1**| cross-platform 3D API wrapper (GLES2+3/GL3/D3D11/Metal)
|  [Swarmz](https://github.com/Cultrarius/Swarmz)                       | **public domain**    | C++ |**1**| swarming/flocking algorithm
|  [tinygizmo](https://github.com/ddiakopoulos/tinygizmo)               | **public domain**    | C++ |  2  | gizmo objects for interactively editing 3d transformations
|**[Vertex Cache Optimizer](https://github.com/Sigkill79/sts)**         | **public domain**    |C/C++|**1**| vertex cache optimization of meshes
|  [Vulkan Memory Allocator](https://github.com/GPUOpen-LibrariesAndSDKs/VulkanMemoryAllocator)|MIT|C/C++|**1**| memory allocator for Vulkan
|  [yocto_trace.h](https://github.com/xelatihy/yocto-gl)                | MIT                  |C/C++|**1**| physically-based unidirectional path tracer w/ MIS for direct lights
|  [yocto_symrigid.h](https://github.com/xelatihy/yocto-gl)             | MIT                  |C/C++|**1**| rigid body simulator (sequential impulse/PGS) with support for concave objects
|  [px_render.h](https://github.com/pplux/px/blob/master/px_render.h)   | MIT                  | C++ |**1**| cross-platform, Multithreaded, command based, 3D render API (GL/GLES) [info](https://github.com/pplux/px/blob/master/README_px_render.md)

# hardware
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|**[EasyTab](https://github.com/ApoorvaJ/EasyTab)**                     | **public domain**    |C/C++|**1**| multi-platform tablet input
|  [libue](https://github.com/houqp/libue)                              | MIT                  |C/C++|  1  | Helper library for Linux device hot-plug event

# hashing
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [xxHash](https://github.com/Cyan4973/xxHash)                         | BSD                  |C/C++|  2  | fast hash function

# images
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  EXR [miniexr](https://github.com/aras-p/miniexr)                     | **public domain**    | C++ |  2  | OpenEXR writer, needs header file
|  EXR [tinyexr](https://github.com/syoyo/tinyexr)                      | BSD                  |C/C++|**1**| EXR image read/write, uses miniz internally
|  GIF [gif.h](https://github.com/ginsweater/gif-h)                     | **public domain**    | C++ |**1**| animated GIF writer (can only include once)
|  GIF **[gif_load](https://github.com/hidefromkgb/gif_load)**          | **public domain**    |C/C++|**1**| (animated) GIF reader
|  GIF [jo_gif.cpp](http://www.jonolick.com/home/gif-writer)            | **public domain**    | C++ |**1**| animated GIF writer (CPP file can also be used as H file)
|  JPG [jpeg-compressor](https://github.com/richgel999/jpeg-compressor) | **public domain**    | C++ |  2  | 2-file JPEG compress, 2-file JPEG decompress
|  JPG [NanoJPEG](http://keyj.emphy.de/nanojpeg/)                       | MIT                  |C/C++|**1**| JPEG decoder
|  JPG **[tiny_jpeg.h](https://github.com/serge-rgb/TinyJPEG/)**        | **public domain**    |C/C++|**1**| JPEG encoder
|  JPG EXIF [easyexif](https://github.com/mayanklahiri/easyexif)        | BSD2                 | C++ |  2  | EXIF metadata extractor for JPEG images
|  JPG EXIF [TinyEXIF](https://github.com/cdcseacave/TinyEXIF)          | BSD                  | C++ |  2  | Parse EXIF data from JPEG (XMP w/ TinyXML2 lib)
|  PDF [PDFgen](https://github.com/AndreRenaud/PDFGen)                  | **public domain**    |  C  |  2  | PDF writer |
|  PNG [lodepng](http://lodev.org/lodepng/)                             | zlib                 |C/C++|  2  | PNG encoder/decoder
|  PNG [picopng.cpp](http://lodev.org/lodepng/picopng.cpp)              | zlib                 | C++ |  2  | tiny PNG loader
|  PNG [TinyPngOutput](https://www.nayuki.io/page/tiny-png-output)      | LGPLv3               |C/C++|  2  | PNG writer |
|  PNM [PNM](https://github.com/dmilos/PNM)                             | Apache 2.0           | C++ |  1  | PBM, PGM and PPM reader and writer |
|  SVG [nanoSVG](https://github.com/memononen/nanosvg)                  | zlib                 |C/C++|**1**| 1-file SVG parser; 1-file SVG rasterizer
|**[cro_mipmap.h](https://github.com/thebeast33/cro_lib)**              | **public domain**    |C/C++|**1**| average, min, max mipmap generators
|  [rjm_texbleed.h](https://github.com/rmitton/rjm)                     | **public domain**    |C/C++|**1**| Fills in the color of pixels where alpha==0

# math
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [amoeba](https://github.com/starwing/amoeba)                         | MIT                  |C/C++|**1**| constraint solver (Cassowary) w/Lua binding
|  [ceval-single-header](https://github.com/e-t-sudo/ceval-single-header)| MIT                 |C/C++|**1**| A single-header library for parsing and evaluation of arithmetic expressions
|  [fft](https://github.com/wareya/fft)                                 | **public domain**    | C++ |**1**| Fast Fourier Transform |
|  [ExprTk](https://www.partow.net/programming/exprtk/index.html)       | **MIT**              | C++ |**1**| Runtime mathematical expression parser and evaluation engine.
|  [PoissonGenerator.h](https://github.com/corporateshark/poisson-disk-generator) | MIT        | C++ |**1**| Poisson disk points generator (disk or rect)
|  [prns.h](http://marc-b-reynolds.github.io/shf/2016/04/19/prns.html)  | **public domain**    |C/C++|**1**| seekable pseudo-random number sequences
|  [rfft.h](https://github.com/grego/rfft.h)				| **public domain**    |C/C++|**1**| Fast Fourier Tranform for arbitrary array sizes
|**[rnd.h](https://github.com/mattiasgustavsson/libs)**                 | **public domain**    |C/C++|**1**| pseudo-random number generation
|  [ShaderFastLibs](https://github.com/michaldrobot/ShaderFastLibs)     | MIT                  | C++ |**1**| (also HLSL) approximate transcendental functions optimized for shaders (esp. GCN)
|  [simrank.hpp](https://github.com/roukaour/simrank)                   | MIT                  | C++ |  2  | SimRank graph similarity algorithm
|  [SummedAreaTable](https://github.com/corporateshark/Summed-Area-Table.git) | MIT            | C++ |**1**| Summed-Area Table generation and sum/avg queries
|  [TinyExpr](https://github.com/codeplea/tinyexpr)                     | zlib                 |  C  |  2  | evaluation of math expressions from strings

# multithreading
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [bikeshed.h](https://github.com/DanEngelbrecht/bikeshed)             | MIT                  |C/C++|**1**| cross-platform lock free fixed memory hierarchical work scheduler
|  [mm_sched.h](https://github.com/vurtun/mmx)                          | zlib                 |C/C++|**1**| cross-platform multithreaded task scheduler based on [enkiTS](https://github.com/dougbinks/enkiTS)
|**[thread.h](https://github.com/mattiasgustavsson/libs)**              | **public domain**    |C/C++|**1**| cross-platform thread primitives
|  [TinyCThread](https://tinycthread.github.io/)                        | zlib                 |C/C++|  2  | cross-platform implementation of the C11 Threads API
|  [TinyThread++](https://tinythreadpp.bitsnbites.eu/)                  | zlib                 | C++ |  2  | cross-platform implementation of the C++11 Threads API
|  [px_sched.h](https://github.com/pplux/px/blob/master/px_sched.h)     | MIT                  | C++ |  1  | cross-platform task scheduler [info](https://github.com/pplux/px/blob/master/README_px_sched.md)

# network
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [cpp-httplib](https://github.com/yhirose/cpp-httplib)                | MIT                  |C/C++|  1  | cross-platform HTTP server/client
|  [civetweb](https://github.com/civetweb/civetweb)                     | MIT                  |C/C++|  2  | HTTP server, fork of Mongoose
|  [EWS](https://github.com/hellerf/EmbeddableWebServer)                | BSD                  |C/C++|**1**| HTTP server
|  [happyhttp](https://github.com/mingodad/HappyHTTP)                   | zlib                 | C++ |  2  | HTTP client requests
|**[http](https://github.com/mattiasgustavsson/libs)**                  | **public domain**    |C/C++|**1**| HTTP get/post
|  [libcluon](https://github.com/chrberger/libcluon)                    | MPL-2.0              | C++ |**1**| cross-platform socket wrapper and data marshalling with native implementations for [Protobuf](https://developers.google.com/protocol-buffers/), [LCM](http://lcm-proj.github.io/type_specification.html)/[ZCM](http://zerocm.github.io/zcm/), JSON, and [MsgPack](https://msgpack.org) serialization/deserialization
|  [LUrlParser](https://github.com/corporateshark/LUrlParser)           | MIT                  | C++ |  2  | lightweight URL & URI parser RFC 1738, RFC 3986
|  [mm_web.h](https://github.com/vurtun/mmx)                            | BSD                  |C/C++|**1**| lightweight webserver, fork of webby
|  [mongoose](https://github.com/cesanta/mongoose)                      | GPLv2                |C/C++|  2  | HTTP server
|  [par_easycurl.h](https://github.com/prideout/par)                    | MIT                  |C/C++|**1**| cURL wrapper
|**[sts_net](https://github.com/kieselsteini/sts)**                     | **public domain**    |C/C++|**1**| cross-platform socket wrapper (socket sets and packet API)
|  [yocto](https://github.com/tom-seddon/yhs)                           | **public domain**    |C/C++|  2  | non-production-use HTTP server
|**[zed_net](https://github.com/Smilex/zed_net)**                       | **public domain**    |C/C++|**1**| cross-platform socket wrapper
|  [znet](https://github.com/starwing/znet)                             | MIT                  |C/C++|**1**| cross-platform networking w/ Lua binding

# serialization
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [archive](https://github.com/voidah/archive)                         |**public domain**     | C++ |**1**| binary serialize & deserlize w/ STL support
|  [cista](https://github.com/felixguendling/cista)                     |MIT                   | C++ |**1**| cross-platform high performance zero copy C++17 serialization/deserialization
|  [libcluon](https://github.com/chrberger/libcluon)                    | MPL-2.0              | C++ |**1**| cross-platform data serialization/deserialization with native implementations for [Protobuf](https://developers.google.com/protocol-buffers/), [LCM](http://lcm-proj.github.io/type_specification.html)/[ZCM](http://zerocm.github.io/zcm/), JSON, and [MsgPack](https://msgpack.org)

# json
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [ajson](https://github.com/lordoffox/ajson)                          | Boost                | C++ |**1**| JSON serialize & deserialize w/ STL support
|  [cJSON](https://sourceforge.net/projects/cjson/)                     | MIT                  |C/C++|**1**| JSON parser
|  [json-build](https://github.com/lcsmuller/json-build)                | MIT                  |C/C++|**1**| JSON serializer
|  [cJSON](https://github.com/DaveGamble/cJSON)                         | MIT                  |C/C++|**1**| JSON parser
|  [json.h](https://github.com/sheredom/json.h)                         | **public domain**    |C/C++|**1**| JSON parser
|  [json.hpp](https://github.com/nlohmann/json)                         | MIT                  | C++ |**1**| JSON parse, serialize, deserialize
|  [jzon.h](https://github.com/Zguy/Jzon)                               | MIT                  | C++ |  2  | JSON parser
|  [PicoJSON](https://github.com/kazuho/picojson)                       | BSD                  | C++ |**1**| JSON parse/serializer
|  [parson](https://github.com/kgabis/parson)                           | MIT                  |C/C++|  2  | JSON parser and serializer
|  [jsonc](https://gitlab.com/bztsrc/jsonc)                             | MIT                  |C/C++|**1**| extremely fast and extremely small (~60 SLoC) JSON parser |

# yaml
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [mini-yaml](https://github.com/jimmiebergmann/mini-yaml)             | MIT                  | C++ |  2  | YAML parser and serializer

# csv
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [CSVstream](https://github.com/awdeorio/csvstream/)                  | MIT                  | C++ |**1**| CSV parser
|  [Fast C++ CSV Parser](https://github.com/ben-strasser/fast-cpp-csv-parser) | BSD            | C++ |**1**| CSV parser
|  [Rapidcsv](https://github.com/d99kris/rapidcsv/)                     | BSD                  | C++ |**1**| CSV parser
|  [Vince's CSV Parser](https://github.com/vincentlaucsb/csv-parser)    | MIT                  | C++ |**1**| CSV parser and serializer

# parsing
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [cmp](https://github.com/camgunz/cmp)                                | MIT                  |C/C++|  2  | MessagePack parser and serializer
|  [cpp-peglib](https://github.com/yhirose/cpp-peglib)                  | MIT                  |C/C++|  1  | PEG (Parsing Expression Grammars) library
|  [inih](https://github.com/benhoyt/inih)                              | BSD                  |C/C++|  2  | .ini file parser
|**[ini.h](https://github.com/mattiasgustavsson/libs)**                 | **public domain**    |C/C++|**1**| .ini file parser
|  [minilibs](https://github.com/ccxvii/minilibs)                       | **public domain**    |  C  |  2  | two-file regex (also binary tree, etc)
|  [mm_lexer.h](https://github.com/vurtun/mmx)                          | zlib                 |C/C++|**1**| C-esque language lexer
|  [SLRE](https://github.com/cesanta/slre)                              |_GPLv2_               |C/C++|**1**| regular expression matcher
|  [tinymemfile](https://github.com/RandyGaul/tinyheaders)              | zlib                 | C++ |**1**| fscanf on in-memory files
|  [udisasm](https://gitlab.com/bztsrc/udisasm)                         | MIT                  |C/C++|**1**| extremely small disassembler for ARMv8.2 AArch64 (~65k) |
|  [Unformat](https://github.com/adamyaxley/Unformat)                   | **public domain**    | C++ |**1**| parses formatted strings (reverse of std::format)

# profiling
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [MicroProfile](https://github.com/jonasmr/microprofile)              | **public domain**    | C++ | 2-4 | CPU (and GPU?) profiler, 1-3 header files, uses miniz internally
|  [prof](https://github.com/cyrus-and/prof)                            | MIT                  |C/C++|**1**| profiler for Linux
|  [Remotery](https://github.com/Celtoys/Remotery)                      | Apache 2.0           |C/C++|  2  | CPU/GPU profiler Win/Mac/Linux, using web browser for viewer

# scripting
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [Duktape](http://duktape.org/)                                       | MIT                  |  C  |  2  | embeddable JavaScript engine
|  [MY-BASIC](https://github.com/paladin-t/my_basic/)                   | MIT                  |  C  |  2  | interpreter for a BASIC dialect scripting language
|  [LIL](http://runtimeterror.com/tech/lil/)                            | zlib                 |C/C++|  2  | interpreter for a Tcl-like scripting language
|  [lualite](https://github.com/user1095108/lualite)                    | MIT                  | C++ |**1**| generate Lua bindings in C++
|  [Picol](https://chiselapp.com/user/dbohdan/repository/picol/)        | BSD                  |C/C++|**1**| interpreter for a Tcl-like scripting language
|  [s7](https://ccrma.stanford.edu/software/snd/snd/s7.html)            | BSD                  |C/C++|  2  | interpreter for a subset of Scheme (R5RS/R7RS)

# state machines
| library                                                                                | license              | API |files| description
| -------------------------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [FFSM2](https://github.com/andrew-gresyk/FFSM2/blob/master/include/ffsm2/machine.hpp) | MIT                  | C++ |**1**| flat FSM
|  [HFSM2](https://github.com/andrew-gresyk/HFSM2/blob/master/include/hfsm2/machine.hpp) | MIT                  | C++ |**1**| hierarchical FSM

# strings
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [dfa](http://bjoern.hoehrmann.de/utf-8/decoder/dfa/)                 | MIT                  |C/C++|  2  | fast UTF-8 decoder (need a header file)
|**[DG_misc.h](https://github.com/DanielGibson/Snippets/)**             | **public domain**    |C/C++|**1**| Daniel Gibson's stb.h-esque cross-platform helpers: path/file, strings
|**[gb_string.h](https://github.com/gingerBill/gb)**                    | **public domain**    |C/C++|**1**| dynamic strings
|  [Obfuscate](https://github.com/adamyaxley/Obfuscate)                 | **public domain**    | C++ |**1**| Guaranteed compile-time string literal obfuscation library for C++14
|  [inja.hpp](https://github.com/pantor/inja)                           | MIT                  | C++ |**1**| template engine
|  [str](https://github.com/maxim2266/str)                              | BSD                  |  C  |  2  | Yet another string library for C language
|**[strpool.h](https://github.com/mattiasgustavsson/libs)**             | **public domain**    |C/C++|**1**| string interning
|**[Str.h](https://github.com/ocornut/Str)**                            | **public domain**    | C++ |**1**| Simple C++ string type with an optional local buffer
|  [str_view.hpp](https://github.com/sawickiap/str_view)                | MIT                  | C++ |**1**| null-termination-aware string-view class
|**[utf8](https://github.com/sheredom/utf8.h)**                         | **public domain**    |C/C++|**1**| UTF-8 string library
| **[csplit](https://github.com/jwlodek/csplit)**                       | MIT                  |C/C++|**1**| String splitting and processing single-header library

# unit testing
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [catch](https://github.com/philsquared/Catch)                        | Boost                | C++ |**1**| unit testing
|  [catch2](https://github.com/catchorg/Catch2/)                        | Boost                | C++ |**1**| unit testing
|  [doctest](https://github.com/onqtam/doctest)                         | MIT                  | C++ |**1**| unit testing
|  [fctx](https://github.com/imb/fctx)                                  | BSD                  |C/C++|**1**| unit testing
|  [greatest](https://github.com/silentbicycle/greatest)                | iSC                  |  C  |**1**| unit testing
|  [hippomocks](https://github.com/dascandy/hippomocks)                 | LGPL                 | C++ |**1**| unit testing
|**[labrat](https://github.com/squarewave/labrat)**                     | **public domain**    |C/C++|**1**| unit testing
|  [minctest](https://github.com/codeplea/minctest)                     | zlib                 |  C  |**1**| unit testing
|  [munit](https://github.com/nemequ/munit)                             | MIT                  |  C  |**1**| unit testing
|**[Rexo](https://github.com/christophercrouzet/rexo)**                 | **public domain**    |C/C++|**1**| framework for C89/C++ featuring automatic registration of tests and a polished API
|  [picotest](https://github.com/colinbarry/picotest)                   | MIT                  |C/C++|**1**| unit testing
|  [SPUT](http://www.lingua-systems.com/unit-testing/)                  | BSD                  |C/C++|**1**| unit testing
|  [trompeloeil](https://github.com/rollbear/trompeloeil)               | Boost                | C++ |**1**| unit testing
|  [utest](https://github.com/evolutional/utest)                        | MIT                  |C/C++|**1**| unit testing
|**[utest.h](https://github.com/sheredom/utest.h)**                     | **public domain**    |C/C++|**1**| unit testing
|**[walter](https://github.com/ir33k/walter)**                          | **public domain**    |  C  |**1**| unit testing
|  [clove-unit](https://github.com/fdefelici/clove-unit)                | MIT                  |  C  |**1**| unit testing

# user interface
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [dear imgui](https://github.com/ocornut/imgui)                       | MIT                  | C++ |  9  | an immediate-mode GUI formerly named "ImGui"; [3rd-party C wrapper](https://github.com/Extrawurst/cimgui)
|  [libcmdf](https://github.com/ronen25/libcmdf)                        | **public domain**    | C   |**1**| a small library for writing CLI applications
|  [linenoise](https://github.com/antirez/linenoise)                    | BSD                  |C/C++|  2  | terminal readline w/ history etc
|  [noc_file_dialog.h](https://github.com/guillaumechereau/noc)         | MIT                  |C/C++|  1  | file open/save dialogs (Win/Mac/Linux)
|  [nuklear](https://github.com/Immediate-Mode-UI/Nuklear)              | **public domain**    |C/C++|**1**| minimal GUI toolkit
|  [tinyfiledialogs](https://sourceforge.net/projects/tinyfiledialogs/) | ZLIB                 |C/C++|  2  | modal dialogs inc. file open/save (Win/Mac/Linux)
|  [wcwidth9](https://github.com/joshuarubin/wcwidth9)                  | Apache 2.0           | C   |  1  | platform independent wcwidth with full unicode 9 support

# vectors
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [algebra3.h](http://www.animats.com/source/graphics/algebra3.h)      | **public domain**    | C++ |**1**| vector utilities for 2, 3, and 4 element vectors, all inline
|**[ccVector.h](https://github.com/jobtalle/ccVector)**                 | **public domain**    |C/C++|**1**| Vector, quaternion and matrix math
|**[gb_math](https://github.com/gingerBill/gb/blob/master/gb_math.h)**  | **public domain**    |C/C++|**1**| Vector, quaternion and matrix math w/o math.h
|**[Handmade Math](https://github.com/StrangeZak/Handmade-Math)**       | **public domain**    |C/C++|**1**| vector math
|  [linalg.h](https://github.com/sgorsten/linalg)                       | **public domain**    | C++ |**1**| vector/matrix/quaternion math
|  [linalg](https://github.com/ilyak/linalg)                            | ISC                  |C/C++|**1**| vector/matrix/quaternion math
|  [mm_vec.h](https://github.com/vurtun/mmx)                            | BSD                  |C/C++|**1**| SIMD vector math
|  [hypatia](https://github.com/dagostinelli/hypatia)                   | MIT                  |  C  |**1**| vector/matrix/quaternion math

# video
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [jo_mpeg](http://www.jonolick.com/home/mpeg-video-writer) / [(converted to C)](https://blog.frost.kiwi/jo-mpeg-in-c)            | **public domain**    | C/C++ |**1**| MPEG file writer

# videogames
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|**[app.h](https://github.com/mattiasgustavsson/libs)**                 | **public domain**    |C/C++|**1**| Windows-only-but-meant-to-be-cross-platform game-ish framework
|  [raycastlib.h](https://gitlab.com/drummyfish/raycastlib)             | CC0 + patent waiver  |C/C++|**1**| advanced raycasting rendering library, pure C99 with no dependencies, only 32bit int math

# miscellaneous
| library                                                               | license              | API |files| description
| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|  [ASAP](https://github.com/mobius3/asap)                              | MIT                  | C++ |**1**| library for parsing, printing, iterating and operating on dates.
|  [benchmark.hpp](https://github.com/burner/sweet.hpp/benchmark.hpp)   | LGPL3                | C++ |**1**| micro benchmark library for C++11 and beyond
|  [cpp-generators](https://github.com/c-smile/cpp-generators)          | BSD                  | C++ |**1**| generators in C++
|  [endianness.h](https://github.com/rofl0r/endianness.h)               | **public domain**    |  C  |**1**| endianness conversion and detection  
|  [ggformat](https://github.com/mikejsavage/ggformat)                  | ISC                  | C++ |  2  | printf replacement
|  [Hedley](https://nemequ.github.io/hedley/)                           | **public domain**    |C/C++|**1**| compiler portability, optimization, static analysis, etc.
|  [format.hpp](https.//github.com/burner/sweet.hpp/format.hpp)         | LGPL3                | C++ |**1**| dlang inspired typesafe string formatting
|  [levenshtein](https://github.com/wooorm/levenshtein.c)               | MIT                  |C/C++|  2  | compute edit distance between two strings
|  [MakeID.h](http://www.humus.name/3D/MakeID.h)                        | **public domain**    | C++ |**1**| allocate/deallocate small integer IDs efficiently
|  [openGA](https://github.com/Arash-codedev/openGA)                    | MPL-2.0              | C++ |**1**| A C++ Generic Algorithm solver library
|  [picobench](https://github.com/iboB/picobench)                       | MIT                  | C++ |**1**| microbenchmarking
|  [PlusCallback](https://github.com/codeplea/pluscallback)             | zlib                 | C++ |**1**| function/method callbacks
|**[process.h](https://github.com/sheredom/process.h)**                 | **public domain**    |C/C++|**1**| process control API
|  [random](https://github.com/effolkronium/random)                     | MIT                  | C++ |**1**| convenient API for random
|  [sokol_time.h](https://github.com/floooh/sokol)                      | MIT                  |C/C++|**1**| cross-platform time measurement
|  [stmr](https://github.com/wooorm/stmr.c)                             | MIT                  |  C  |  2  | extract English word stems
|  [tinyformat](https://github.com/c42f/tinyformat)                     | Boost                | C++ |**1**| typesafe printf
|  [tinytime](https://github.com/RandyGaul/tinyheaders)                 | zlib                 |C/C++|**1**| quick-and-dirty time elapsed time
|**[ubench.h](https://github.com/sheredom/ubench.h)**                   | **public domain**    |C/C++|**1**| microbenchmarking 
|  [visit_struct](https://github.com/cbeck88/visit_struct)              | Boost                | C++ |  2  | struct-field reflection
|  [sili-toolchain](https://github.com/EimaMei/sili-toolchain)          | **public domain**    |C/C++|**1**| C toolchain for modern C programming, strings, arrays, files, threading, ect
|  [RGFW](https://github.com/ColleagueRiley/RGFW)                        | zlib                 |C/C++|**1**| A multi-platform single-header user-friendly GUI framework as an alternative to GLFW 

There are also these XML libraries, but I am so significantly not a fan of XML that I've consigned these to the basement to make you think twice.

- parsing: [tinyxml2](https://github.com/leethomason/tinyxml2): XML (zlib license)
- parsing: [pugixml](http://pugixml.org/): XML (MIT license)
- parsing: [yxml](https://dev.yorhel.nl/yxml): XML (MIT license)

# uncategorized

| cat | library                                                               | license              | API |files| description
| ---- | --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
2d | [C-Turtle](https://github.com/walkerje/C-Turtle) | MIT | C++ | **1** | Port of Python's Turtle to C++
2d | [cgl](https://github.com/Jaysmito101/cgl) | MIT | C | 2 | C Game Library
2d | [daisy](https://github.com/sse2/daisy) | MIT | C++ | **1** | 2D Graphics and text
2d | [m_dist.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_dist.h) | zlib | C/C++ | **1** | fast distance transform and Voronoi
2d | [m_image.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_image.h) | zlib | C/C++ | **1** | image processing routines
2d | [m_path_finding.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_path_finding.h) | zlib | C/C++ | **1** | floodfill-based path finding
2d | [m_raster.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_raster.h) | zlib | C/C++ | **1** | simple rasterizer
2d | [pico_gfx.h](https://github.com/empyreanx/pico_headers/blob/main/pico_gfx.h) | **PD/zlib** | C | **1** | Graphics library (sokol_gfx)
2d | [pico_gl.h](https://github.com/empyreanx/pico_headers/blob/mainpico_gl.h) | **PD/zlib** | C | **1** | Graphics library (OpenGL)
2d | [scalable-font2](https://gitlab.com/bztsrc/scalable-font2) | MIT | C | **1** | Scalable Font renderer + specification
2d | [si_normalmap](https://github.com/Sir-Irk/si_normalmap) | **PD** | C | **1** | Image to Normal Map generator
3d | [model3d](https://gitlab.com/bztsrc/model3d) | MIT | C | **1** | 3D model format specification
audio | [atomix](https://github.com/BareRose/atomix) | **PD** | C | **1** | wait-free atomic sound mixer
audio | [chibi-xmplay](https://github.com/reduz/chibi-xmplay) | BSD3 | C | 2 | XM module playback library
audio | [jar-mod](https://github.com/kd7tck/jar/blob/master/jar_mod.h) | **PD** | C | **1** | MOD playback library
audio | [jar-xm](https://github.com/kd7tck/jar/blob/master/jar_xm.h) | **WTFPLv2** | C | **1** | XM playback library
audio | [mojoAL](https://github.com/icculus/mojoAL) | zlib | C | **1** | Full OpenAL 1.1 implementation
audio | [nanoalsa](https://gitlab.com/bztsrc/nanoalsa) | MIT | C | **1** | Tiny PCM playback under Linux
audio | [wav.h](https://github.com/dyeo/dyeo.h/blob/main/wav.h) | **PD/MIT** | C | **1** | .wav file encoding and decoding
b64 | [pico_b64.h](https://github.com/empyreanx/pico_headers/blob/main/pico_b64.h) | **PD/zlib** | C | **1** | Base64 en/decoder
crypt | [tiny-AES-c](https://github.com/kokke/tiny-AES-c) | **PD** | C | 2 | Small portable AES128/192/256 in C
crypt | [tiny-ECDH-c](https://github.com/kokke/tiny-ECDH-c) | **PD** | C | 2 | Small portable Elliptic-Curve Diffie-Hellman in C
date | [date](https://github.com/HowardHinnant/date) | MIT | C++ | **1** | date and time libraries
ds | [dynarr](https://github.com/BareRose/dynarr) | **PD** | C | **1** | dynamic array container
ds | [fifo_declare.h](https://github.com/buserror/simavr/blob/master/simavr/sim/fifo_declare.h) | LGPL2 | C/C++ | **1** | Thread/core safe FIFO
ds | [jhr_skip_list](https://github.com/Garfield1002/jhr_skip_list) | **PD** | C++ | **1** | Skip Lists
ds | [jrsl](https://github.com/Garfield1002/jrsl) | **PD** | C/C++ | **1** | Skip Lists
ds | [libintrusive](https://github.com/graphitemaster/libintrusive) | **PD** | C | 2 | Intrusive data structures
ds | [lstr.h](https://github.com/dyeo/dyeo.h/blob/main/lstr.h) | **PD/MIT** | C | **1** | length-bounded strings
ecs | [pico_ecs.h](https://github.com/empyreanx/pico_headers/blob/main/pico_ecs.h) | **PD/zlib** | C | **1** | Pure and simple ECS
engine | [FWK1](https://github.com/fwk3d/v1/blob/master/2024/2024.10/engine/joint.h) | **public domain** | C |**1**| Game engine
engine | [olcPixelGameEngine](https://github.com/OneLoneCoder/olcPixelGameEngine) | BSD3 | C++ | **1** | Game engine
eval | [mathe.h](https://github.com/dyeo/dyeo.h/blob/main/mathe.h) | **PD/MIT** | C | **1** | mathematical expression parsing
ext | [cor.h](https://github.com/dyeo/dyeo.h/blob/main/cor.h) | **PD/MIT** | C | **1** | coroutines
ext | [errnoname](https://github.com/mentalisttraceur/errnoname) | BSD0 | C | 2 | extended errno messages
ext | [filesystem](https://github.com/gulrak/filesystem) | MIT | C++ | **1** | implementation of std::filesystem
ext | [outcome](https://github.com/ned14/outcome/tree/develop/single-header) | Apache2/Boost | C++ | **1** | outcome and result C++ containers
gl | [final_dynamic_opengl.h](https://github.com/f1nalspace/final_game_tech/blob/master/final_dynamic_opengl.h) | MIT | C | **1** | opengl loader
gui | [webview](https://github.com/zserge/webview) | MIT | C/C++ | **1** | cross-platform webview library
hash | [hash.c](https://github.com/zzo38/freeheromesh/blob/trunk/hash.c) | **PD** | C | 2 | SHA1/SHA3/MD5 hashes
hash | [lonesha256](https://github.com/BareRose/lonesha256) | **PD** | C | **1** | SHA256 implementation
hash | [PicoSHA2](https://github.com/okdshin/PicoSHA2) | MIT | C++ | **1** | SHA256 implementation
image | [bitmap](https://github.com/ArashPartow/bitmap) | MIT | C++ | **1** | Bitmap decoder and utilities
image | [framepacker](https://github.com/paladin-t/framepacker) | MIT | C++ | **1** | texture bin packing algorithm
image | [tiffloader](https://github.com/MalcolmMcLean/tiffloader) | **PD** | C | 2 | TIFF image loader
json | [jsmn](https://github.com/zserge/jsmn) | MIT | C | **1** | Minimalistic JSON parser
json | [jsonc](https://gitlab.com/bztsrc/jsonc) | MIT | C | **1** | Fast JSON parser
json | [sjson](https://github.com/septag/sjson) | BSD2 | C | **1** | JSON encode/decoder
log | [pico_log.h](https://github.com/empyreanx/pico_headers/blob/main/pico_log.h) | **PD/zlib** | C | **1** | Flexible logging framework
math | [Delaunay](https://github.com/BrunoLevy/geogram.psm.Delaunay) | BSD3 | C++ | 2 | 2D and 3D Delaunay triangulation
math | [dvector](https://github.com/BareRose/dvector) | **PD** | C | **1** | 2D/3D vector/quaternion/matrix math library
math | [gm.h](https://github.com/dyeo/dyeo.h/blob/main/gm.h) | **PD/MIT** | C | **1** | vector/matrix/quaternion math
math | [HMM Toolkit](https://github.com/gerbenvoshol/Hidden-Markov-Model-Toolkit) | GPL2 | C/C++ | **1** | Discrete and continuous Hidden Markov Models (DHMM, CHMM)
math | [linmath.h](https://github.com/datenwolf/linmath.h) | **WTFPLv2** | C | **1** | vector library
math | [m_math.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_math.h) | zlib | C/C++ | **1** | math with C/OpenCL portability
math | [omm](https://github.com/Hectarea1996/omm) | MIT | C++ | **1** | Template open multi-methods
math | [OpenNL](https://github.com/BrunoLevy/geogram.psm.OpenNL) | BSD3 | C++ | 2 | linear and eigen solvers
math | [pico_hit.h](https://github.com/empyreanx/pico_headers/blob/main/pico_hit.h) | **PD/zlib** | C | **1** | 2D collision detection (SAT) and ray casting
math | [pico_math.h](https://github.com/empyreanx/pico_headers/blob/main/mpico_math.h) | **PD/zlib** | C | **1** | 2D math library for games
math | [pico_qt.h](https://github.com/empyreanx/pico_headers/blob/mainpico_qt.h) | **PD/zlib** | C | **1** | Quadtree library
math | [precision](https://github.com/possibly-wrong/precision) | **PD** | C++ | 3 | Arbitrary-precision integer and rational arithmetic
math | [simple_linear_regression](https://github.com/torkeldanielsson/simple_linear_regression) | MIT | C/C++ | **1** | Simple linear regression
math | [Statistics-Tool-Box](https://github.com/gerbenvoshol/Statistics-Tool-Box) | **PD** | C/C++ | **1** | Statistical functions
math | [tiny-bignum-c](https://github.com/kokke/tiny-bignum-c) | **PD** | C | 2 | Small portable multiple-precision unsigned integer arithmetic in C
math | [vmath](https://github.com/monolifed/vmath) | **PD** | C | **1** | Vector/matrix library
mem | [buddy_alloc](https://github.com/spaskalev/buddy_alloc) | BSD0 | C | **1** | buddy memory allocator
mem | [final_memory.h](https://github.com/f1nalspace/final_game_tech/blob/master/final_memory.h) | MIT | C | **1** | heap memory handler
misc | [args.h](https://github.com/dyeo/dyeo.h/blob/main/args.h) | **PD/MIT** | C | **1** | argparse-style argument parser
misc | [CLM_LIBS](https://github.com/CarlosLunaMota/CLM_LIBS) | **PD** | C | **1** | Diverse utilities
misc | [Color-Toolkit](https://github.com/gerbenvoshol/Color-Toolkit) | GPL2 | C/C++ | **1** | Color conversion utils (RGB, XYZ, Lab, CIE76, CIE94 and CIEDE200)
misc | [ebnn.h](https://github.com/kunglab/ebnn/blob/master/c/ebnn.h) | MIT | C | **1** | BNN (Binarized Neural Networks)
misc | [final_tiletrace.hpp](https://github.com/f1nalspace/final_game_tech/blob/master/final_tiletrace.hpp) | MIT | C++ | **1** | tilemap contour tracing
misc | [h.h](https://github.com/robertsdotpm/h.h) | GPL3 | C/C++ | **1** | Diverse utilities
misc | [ll.h](https://github.com/dyeo/dyeo.h/blob/main/ll.h) | **PD/MIT** | C | **1** | cross-platform library loading
misc | [mmu](https://github.com/CN-xLeaves/mmu) | MIT | C | 2 | memory management and data structure toolset
misc | [QR-Code-generator](https://github.com/nayuki/QR-Code-generator) | MIT | C | 2 | QR Code generator
misc | [qsort](https://github.com/svpv/qsort) | MIT | C | **1** | qsort algorithm as a C macro
misc | [scogem.c](https://github.com/zzo38/scorpion/blob/trunk/scogem.c) | **PD** | C | 2 | URL parser
misc | [smallxrm.c](https://github.com/zzo38/freeheromesh/blob/trunk/smallxrm.c) | **PD** | C | 2 | Implementation of X resource manager
misc | [x.h](https://github.com/Neur1n/x.h) | Mulan2 | C/C++ | **1** | cross-platform C/C++ utilities
net | [netq](https://gitlab.com/bztsrc/netq) | MIT | C | **1** | Reliable datagram library
net | [simpletls.c](https://github.com/zzo38/scorpion/blob/trunk/simpletls.c) | **PD** | C | 2 | Function to create a socket and connect to a remote server with TLS
net | [swrap](https://github.com/BareRose/swrap) | **PD** | C | **1** | TCP and UDP socket wrapper
net | [tiniest-analytics](https://github.com/Pintea/tiniest-analytics) | MIT | C++ | 2 | Cross-platform analytics for games (using Google Analytics <4)
net | [tiny-MQTT-c](https://github.com/kokke/tiny-MQTT-c) | **PD** | C | 2(4) | Small implementation of (some of) the MQTT protocol in C
net | [tlse](https://github.com/eduardsui/tlse) | **PD/BSD2** | C | 2 | TLS v1.0, 1.2, 1.3 and DTLS 1.0, 1.2 implementations
net | [udp.h](https://github.com/dyeo/dyeo.h/blob/main/udp.h) | **PD/MIT** | C | **1** | cross-platform udp networking
net | [webster](https://github.com/brunexgeek/webster) | Apache2 | C++ | 2 | Standalone HTTP server/client
pack | [nibrans](https://github.com/BareRose/nibrans) | **PD** | C | **1** | adaptive rANS library
pack | [rle](https://gitlab.com/bztsrc/rle) | MIT | C | **1** | RLE library
parser | [html-parse.c](https://git.savannah.gnu.org/cgit/wget.git/tree/src/html-parse.c) | GPL | C | 2 | HTML parser (wget)
parser | [tiny-regex-c](https://github.com/kokke/tiny-regex-c) | **PD** | C | 2 | Small portable regex in C
parser | [tiny-regex-mod](https://github.com/monolifed/tiny-regex-mod) | **PD** | C | **1** | Tiny regular expressions library 
parser | [tok](https://gitlab.com/bztsrc/tok) | MIT | C | **1** | Configurable tokenizer
parser | [tomlplusplus](https://github.com/marzer/tomlplusplus) | MIT | C++ | **1** | TOML parser and serializer 
prng | [ranxoshi256](https://github.com/BareRose/ranxoshi256) | **PD** | C | **1** | xoshiro256 algorithm
raster | [canvas_ity](https://github.com/a-e-k/canvas_ity) | ISC | C++ | **1** | 2D rasterizer
script | [xpl](https://github.com/paladin-t/xpl) | **WTFPLv2** | C | **1** | X Programming Language
serial | [blob_tree](https://github.com/dicroce/blob_tree) | MIT | C++ | **1** | Binary tree serializer
serial | [dt.h](https://github.com/dyeo/dyeo.h/blob/main/dt.h) | **PD/MIT** | C | **1** | datatag serializer/deserializer (superset of JSON)
serial | [qserial](https://github.com/earonesty/qserial) | BSD3 | C++ | **1** | Schema-driven serialization library
serial | [Serialization helper](https://gist.github.com/TheServer201/9ae5322cd52f76c7d36af15d3b366762) | **WTFPLv2** | C | **1** | Serialization helper
serial | [stream.h](https://github.com/dyeo/dyeo.h/blob/main/stream.h) | **PD/MIT** | C | **1** | byte streams
svg | [SimpleSVG](https://github.com/adishavit/simple-svg) | BSD3 | C++ | **1** | Easy to use SVG library
sys | [cpuid](https://github.com/anzz1/cpuid) | ?? | C/C++ | **1** | cross-platform cpuid intrinsic
sys | [doops](https://github.com/eduardsui/doops) | **PD** | C | **1** | Event loop library
sys | [final_platform_layer.h](https://github.com/f1nalspace/final_game_tech/blob/master/final_platform_layer.h) | MIT | C | **1** | platform abstraction
sys | [iathook](https://github.com/anzz1/iathook) | ?? | C/C++ | **1** | import address table hooking library (x86/x64,w32)
sys | [JArgsParser](https://github.com/ZhengqiaoWang/JArgsParser) | MIT | C++ | **1** | arguments parser
sys | [openmodal](https://gitlab.com/bztsrc/openmodal) | MIT | C | **1** | Native file modals
sys | [xproc](https://github.com/time-killer-games/xproc) | MIT | C++ | 2 | Foreign Process Information
test | [test.h](https://github.com/dyeo/dyeo.h/blob/main/test.h) | **PD/MIT** | C | **1** | unit testing
time | [pico_time.h](https://github.com/empyreanx/pico_headers/blob/main/tpico_time.h) | **PD/zlib** | C | **1** | Time management library
unit | [pico_unit.h](https://github.com/empyreanx/pico_headers/blob/main/upico_unit.h) | **PD/zlib** | C | **1** | Unit testing framework
video | [pl_mpeg](https://github.com/phoboslab/pl_mpeg) | MIT | C | **1** | MPEG1 video and audio decoder
xml | [final_xml.h](https://github.com/f1nalspace/final_game_tech/blob/master/final_xml.h) | MIT | C | **1** | xml parser

## New libraries and corrections

Submissions of new libraries: I accept submissions (as issues or as pull requests). Please
note that every file that must be included in a user's project counts; a header and a source
file is 2 files, but a header file, source file, and LICENSE (if the license isn't in the
source file) is 3 files, and won't be accepted, because it's not 2 files. But actually
'LICENSE' is a problem for just dropping the library in a source tree anyway, since it's
not scoped to just the library, so library authors are encouraged to include the license in the
source file and not require a separate LICENSE.

Corrections: if information for a library above is wrong, please send a correction as an
issue, pull request, or email. Note that if the list indicates a library works from both
C/C++, but it doesn't, this could be an error in the list or it could be a bug in the
library. If you find a library doesn't work in 32-bit or 64-bit, the library should be
removed from this list, unless it's a bug in the library.

## *List FAQ*

### Can I link directly to this list?

Yes. [This is the preferred link.](https://github.com/nothings/single_file_libs)

### Why isn't library XXX which is made of 3 or more files on this list?

I draw the line arbitrarily at 2 files at most. (Note that some libraries that appear to
be two files require a separate LICENSE file, which made me leave them out). Some of these
libraries are still easy to drop into your project and build, so you might still be ok with them.
But since people come to stb for single-file public domain libraries, I feel that starts
to get too far from what we do here.

### Why isn't library XXX which is at most two files and has minimal other dependencies on this list?

Probably because I don't know about it, feel free to submit a pull request, issue, email, or tweet it at
me (it can be your own library or somebody else's). But I might not include it for various
other reasons, including subtleties of what is 'minimal other dependencies' and subtleties
about what is 'lightweight'.

### Why isn't SQLite's amalgamated build on this list?

Come on.
