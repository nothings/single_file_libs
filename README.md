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
- Libraries should use at most two files

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
    - [unit testing etc.](#tests)
  - other
    - [AI](#ai)
    - [cryptography](#crypto)
    - [user interface](#user-interface)
    - [miscellaneous](#miscellaneous)

# AI
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   | [micropather](http://www.grinninglizard.com/MicroPather/)             | zlib                 | C++ |  2  | pathfinding with A\*
|   | [Genann](https://github.com/codeplea/genann)                          | zlib                 |C/C++|  2  | simple neural networks (ANN)
|   | [KANN](https://github.com/attractivechaos/kann)                       | MIT                  |C/C++|  2  | automatic differentiation (2 files)

# argv
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [parg](https://github.com/jibsen/parg)                               | **public domain**    |  C  |  2  | command-line argument parsing
|   |  [flags](https://github.com/sailormoon/flags)                         | **public domain**    | C++ |**1**| command-line argument parsing
|   |  [Argh!](https://github.com/adishavit/argh)                           | BSD                  | C++ |**1**| command-line argument parsing
|   |  [optionparser](http://optionparser.sourceforge.net/)                 | MIT                  | C++ |**1**| command-line argument parsing
|   |  [cmdline](https://github.com/tanakh/cmdline)                         | BSD                  | C++ |**1**| command-line argument parsing
|   |  [linkom](https://github.com/hernandp/linkom)                         | MIT                  |C/C++|**1**| command-line argument parsing w/ DOS-style options
|   |  [ProgramOptions.hxx](https://github.com/Fytch/ProgramOptions.hxx)    | MIT                  | C++ |**1**| command-line argument parsing

# audio
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [aw_ima.h](https://github.com/afterwise/aw-ima/blob/master/aw-ima.h) | MIT                  |C/C++|**1**| IMA-ADPCM audio decoder
|   |**[dr_flac](https://github.com/mackron/dr_libs)**                      | **public domain**    |C/C++|**1**| FLAC audio decoder
|   |**[dr_wav](https://github.com/mackron/dr_libs)**                       | **public domain**    |C/C++|**1**| WAV audio loader
|   |**[sts_mixer](https://github.com/kieselsteini/sts)**                   | **public domain**    |C/C++|**1**| simple stereo audio mixer
|   |  [tinysound](https://github.com/RandyGaul/tinyheaders)                | zlib                 |C/C++|**1**| direct sound audio mixer & WAV loader
|   |  [btac1c](https://github.com/cr88192/bgbtech_misc/blob/master/mini/btac1c_mini0.h)| MIT      |C/C++|**1**| MS-IMA_ADPCM variant
|   |  [TinySoundFont](https://github.com/schellingb/TinySoundFont)         | MIT                  |C/C++|**1**| SoundFont2 loader & synthesizer

# compression
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |**[miniz.c](https://github.com/richgel999/miniz)**                     |**public&nbsp;domain**|C/C++|**1**| compression, decompression, ZIP file, PNG writing
|   |  [lz4](https://github.com/lz4/lz4)                                    | BSD                  |C/C++|  2  | fast but larger LZ compression
|   |  [fastlz](https://code.google.com/archive/p/fastlz/source/default/source) | MIT              |C/C++|  2  | fast but larger LZ compression
|   |  [pithy](https://github.com/johnezang/pithy)                          | BSD                  |C/C++|  2  | fast but larger LZ compression
|   |  [microtar](https://github.com/rxi/microtar)                          | MIT                  |C/C++|  2  | lightweight tar library

# crypto
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [TweetNaCl](http://tweetnacl.cr.yp.to/software.html)                 | **public domain**    |  C  |  2  | high-quality tiny cryptography library

# data structures
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [klib](http://attractivechaos.github.io/klib/)                       | MIT                  |C/C++|  2  | many 2-file libs: hash, sort, b-tree, etc
|   |  [uthash](https://github.com/troydhanson/uthash)                      | BSD                  |C/C++|  2  | several 1-header, 1-license-file libs: generic hash, list, etc
|   |  [PackedArray](https://github.com/gpakosz/PackedArray)                | **WTFPLv2**          |  C  |  2  | memory-efficient array of elements with non-pow2 bitcount
|   |  [minilibs](https://github.com/ccxvii/minilibs)                       | **public domain**    |  C  |  2  | two-file binary tress (also regex, etc)
|   |**[DG_dynarr.h](https://github.com/DanielGibson/Snippets/)**           | **public domain**    |C/C++|**1**| typesafe dynamic arrays (like std::vector) for plain C
|   |  [chobo-shl](https://github.com/Chobolabs/chobo-shl)                  | MIT                  | C++ |**1**| several C++11 standard contaner like libraries and helpers 
|   |  [libpqueue](https://github.com/vy/libpqueue)                         | BSD                  |C/C++|  2  | priority queue (heap)
|   |  [simclist](http://mij.oltrelinux.com/devel/simclist)                 | BSD                  |C/C++|  2  | linked-list
|   |  [selist](https://github.com/ennorehling/clibs)                       | ISC                  |C/C++|  2  | space-efficient linked-list
|   |  [avl](https://github.com/etherealvisage/avl)                         | **public domain**    |C/C++|  2  | AVL tree

# debugging
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [loguru](https://github.com/emilk/loguru)                            | **public domain**    | C++ |**1**| flexible logging
|   |  [pempek_assert.cpp](https://github.com/gpakosz/Assert)               | **WTFPLv2**          | C++ |  2  | flexible assertions
|   |  [debug-assert](https://github.com/foonathan/debug_assert)            | zlib                 | C++ |**1**| modular assertion macro
|   |  [dbgtools](https://github.com/wc-duck/dbgtools)                      | zlib                 |C/C++|  2  | cross-platform debug util libraries
|   | [debugbreak](https://github.com/scottt/debugbreak)                    | BSD                  |C/C++|**1**| programmatic debug break

# files & filenames
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |**[DG_misc.h](https://github.com/DanielGibson/Snippets/)**             | **public domain**    |C/C++|**1**| Daniel Gibson's stb.h-esque cross-platform helpers: path/file, strings
|   |  [whereami](https://github.com/gpakosz/whereami)                      | **WTFPLv2**          |C/C++|  2  | get path/filename of executable or module
|   |  [dirent](https://github.com/tronkko/dirent)                          | MIT                  |C/C++|**1**| dirent for Windows: retrieve file & dir info
|   |  [TinyDir](https://github.com/cxong/tinydir)                          | BSD                  |  C  |**1**| cross-platform directory reading (Win/POSIX/MinGW)
|   |  [tinyfiles](https://github.com/RandyGaul/tinyheaders)                | zlib                 |C/C++|**1**| cross-platform directory reading (Win/Mac/Unix)
|   |  [tfile](https://github.com/rec/tfile)                                | MIT                  |C++|**1**| FILE* wrapper does read-write-append-seek-close (Win/Mac/Unix)

# geometry file
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [tk_objfile](https://github.com/joeld42/tk_objfile)                  | MIT                  |C/C++|**1**| OBJ file loader
|   |  [tinyply](https://github.com/ddiakopoulos/tinyply)                   | **public domain**    | C++ |  2  | PLY mesh file loader
|   |  [tinyobjloader](https://github.com/syoyo/tinyobjloader)              | MIT                  | C++ |**1**| wavefront OBJ file loader
|   |  [tinyobjloader-c](https://github.com/syoyo/tinyobjloader-c)          | MIT                  |  C  |**1**| wavefront OBJ file loader
|   |  [yocto_obj.h](https://github.com/xelatihy/yocto-gl)                  | MIT                  |C/C++|**1**| wavefront OBJ file loader

# geometry math
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |**[nv_voronoi.h](http://www.icculus.org/~mordred/nvlib/)**             | **public domain**    |C/C++|**1**| find voronoi regions on lattice w/ integer inputs
|   |**[df](https://github.com/983/df)**                                    | **public domain**    |C/C++|**1**| find voronoi region in linear time of size of lattice 
|   |**[sobol.h](https://github.com/Marc-B-Reynolds/Stand-alone-junk/)**    | **public domain**    |C/C++|**1**| sobol & stratified sampling sequences
|   |  [sdf.h](https://github.com/memononen/SDF)                            | MIT                  |C/C++|**1**| compute signed-distance field from antialiased image
|   |  [nanoflann](https://github.com/jlblancoc/nanoflann)                  | BSD                  | C++ |**1**| build KD trees for point clouds
|   |  [jc_voronoi](https://github.com/JCash/voronoi)                       | MIT                  |C/C++|**1**| find voronoi regions on float/double data
|   |  [par_msquares](https://github.com/prideout/par)                      | MIT                  |C/C++|**1**| convert (binarized) image to triangles
|   |  [par_shapes](http://github.prideout.net/shapes)                      | MIT                  |C/C++|**1**| generate various 3d geometric shapes
|   |  [Tomas Akenine-Moller snippets](http://tinyurl.com/ht79ndj)          | **public domain**    |C/C++|  2  | various 3D intersection calculations, not lib-ified
|   |  [Clipper](http://www.angusj.com/delphi/clipper.php)                  | Boost                | C++ |  2  | line & polygon clipping & offsetting
|   |  [PolyPartition](https://github.com/ivanfratric/polypartition)        | MIT                  | C++ |  2  | polygon triangulation, partitioning
|   |  [Voxelizer](https://github.com/karimnaaji/voxelizer)                 | MIT                  |C/C++|**1**| convert triangle mesh to voxel triangle mesh
|   |  [yocto_bvh.h](https://github.com/xelatihy/yocto-gl)                  | MIT                  |C/C++|**1**| ray-casting and closest-element queries of bounding-volume hierarchy
|   |  [yocto_shape.h](https://github.com/xelatihy/yocto-gl)                | MIT                  |C/C++|**1**| shape generation, tesselation, normals, etc.
|   |**[rjm](https://github.com/rmitton/rjm)**                              | **public domain**    |C/C++|**1**| marching cubes triangulator

# graphics (text)
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [rang](https://github.com/agauniyal/rang)                            | **public domain**    | C++ |**1**| cross-platform colored console text 

# graphics (2d)
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [blendish](https://bitbucket.org/duangle/oui-blendish/src)           | MIT                  |C/C++|  1  | blender-style widget rendering using NanoVG
|   |  [tigr](https://bitbucket.org/rmitton/tigr/src)                       | **public domain**    |C/C++|  2  | quick-n-dirty window text/graphics for Windows and macOS
|   |  [noc_turtle](https://github.com/guillaumechereau/noc)                | MIT                  |C/C++|  2  | procedural graphics generator
|   |  [Cimg](http://cimg.eu/)                                              | CeCILL/CeCILL-C      | C++ |**1**| image processing toolkit (60K LoC)
|   |  [Immediate2D](https://github.com/npiegdon/immediate2d)               | **public domain**    | C++ |  2  | zero-configuration, immediate-mode 2D graphics for Windows

# graphics (3d)
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [yocto_trace.h](https://github.com/xelatihy/yocto-gl)                | MIT                  |C/C++|**1**| physically-based unidirectional path tracer w/ MIS for direct lights
|   |  [yocto_symrigid.h](https://github.com/xelatihy/yocto-gl)             | MIT                  |C/C++|**1**| rigid body simulator (sequential impulse/PGS) with support for concave objects
|   |  [mikktspace](https://developer.blender.org/diffusion/B/browse/master/intern/mikktspace)                             | zlib                 |C/C++|  2  | compute tangent space for normal mapping
|   |  [debug-draw](https://github.com/glampert/debug-draw)                 | **public domain**    | C++ |**1**| API-agnostic immediate-mode debug rendering
|   |  [Swarmz](https://github.com/Cultrarius/Swarmz)                       | **public domain**    | C++ |**1**| swarming/flocking algorithm
|   |**[lightmapper](https://github.com/ands/lightmapper#lightmapper)**     | **public domain**    |C/C++|**1**| use your OpenGL renderer to offline bake lightmaps
|   |**[seamoptimizer](https://github.com/ands/seamoptimizer)**             | **public domain**    |C/C++|**1**| modify lightmap data to hide seams
|   |  [tinygizmo](https://github.com/ddiakopoulos/tinygizmo)               | **public domain**    | C++ |  2  | gizmo objects for interactively editing 3d transformations
|   |**[Vertex Cache Optimizer](https://github.com/Sigkill79/sts)**         | **public domain**    |C/C++|**1**| vertex cache optimization of meshes

# hardware
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |**[EasyTab](https://github.com/ApoorvaJ/EasyTab)**                     | **public domain**    |C/C++|**1**| multi-platform tablet input
|   |  [libue](https://github.com/houqp/libue)                              | MIT                  |C/C++|  1  | Helper library for Linux device hot-plug event

# hashing
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [xxHash](https://github.com/Cyan4973/xxHash)                         | BSD                  |C/C++|  2  | fast hash function

# images
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [jo_gif.cpp](http://www.jonolick.com/home/gif-writer)                | **public domain**    | C++ |**1**| animated GIF writer (CPP file can also be used as H file)
|   |  [gif.h](https://github.com/ginsweater/gif-h)                         | **public domain**    | C++ |**1**| animated GIF writer (can only include once)
|   |**[tiny_jpeg.h](https://github.com/serge-rgb/TinyJPEG/)**              | **public domain**    |C/C++|**1**| JPEG encoder
|   |**[gif_load](https://github.com/hidefromkgb/gif_load)**                | **public domain**    |C/C++|**1**| (animated) GIF reader
|   |  [miniexr](https://github.com/aras-p/miniexr)                         | **public domain**    | C++ |  2  | OpenEXR writer, needs header file
|   |  [tinyexr](https://github.com/syoyo/tinyexr)                          | BSD                  |C/C++|**1**| EXR image read/write, uses miniz internally  
|   |  [lodepng](http://lodev.org/lodepng/)                                 | zlib                 |C/C++|  2  | PNG encoder/decoder
|   |  [NanoJPEG](http://keyj.emphy.de/nanojpeg/)                           | MIT                  |C/C++|**1**| JPEG decoder
|   |  [nanoSVG](https://github.com/memononen/nanosvg)                      | zlib                 |C/C++|**1**| 1-file SVG parser; 1-file SVG rasterizer
|   |  [picopng.cpp](http://lodev.org/lodepng/picopng.cpp)                  | zlib                 | C++ |  2  | tiny PNG loader
|   |  [jpeg-compressor](https://github.com/richgel999/jpeg-compressor)     | **public domain**    | C++ |  2  | 2-file JPEG compress, 2-file JPEG decompress
|   |  [easyexif](https://github.com/mayanklahiri/easyexif)                 | MIT                  | C++ |  2  | EXIF metadata extractor for JPEG images
|   |  [TinyEXIF](https://github.com/cdcseacave/TinyEXIF)                   | BSD                  | C++ |  2  | Parse EXIF data from JPEG (XMP w/ TinyXML2 lib)
|   |**[cro_mipmap.h](https://github.com/thebeast33/cro_lib)**              | **public domain**    |C/C++|**1**| average, min, max mipmap generators
|   |  [PDFgen](https://github.com/AndreRenaud/PDFGen)                      | **public domain**    |  C  |  2  | PDF writer |

# math
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [ShaderFastLibs](https://github.com/michaldrobot/ShaderFastLibs)     | MIT                  | C++ |**1**| (also HLSL) approximate transcendental functions optimized for shaders (esp. GCN)
|   |  [TinyExpr](https://github.com/codeplea/tinyexpr)                     | zlib                 |  C  |  2  | evaluation of math expressions from strings
|   |  [PoissonGenerator.h](https://github.com/corporateshark/poisson-disk-generator) | MIT        | C++ |**1**| Poisson disk points generator (disk or rect)
|   |  [prns.h](http://marc-b-reynolds.github.io/shf/2016/04/19/prns.html)  | **public domain**    |C/C++|**1**| seekable pseudo-random number sequences
|   |  [amoeba](https://github.com/starwing/amoeba)                         | MIT                  |C/C++|**1**| constraint solver (Cassowary) w/Lua binding
|   |  [simrank.hpp](https://github.com/roukaour/simrank)                   | MIT                  | C++ |  2  | SimRank graph similarity algorithm
|   |**[rnd.h](https://github.com/mattiasgustavsson/libs)**                 | **public domain**    |C/C++|**1**| pseudo-random number generation

# multithreading
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [mm_sched.h](https://github.com/vurtun/mmx)                          | zlib                 |C/C++|**1**| cross-platform multithreaded task scheduler based on [enkiTS](https://github.com/dougbinks/enkiTS)
|   |**[thread.h](https://github.com/mattiasgustavsson/libs)**              | **public domain**    |C/C++|**1**| cross-platform thread primitives

# network
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |**[zed_net](https://github.com/Smilex/zed_net)**                       | **public domain**    |C/C++|**1**| cross-platform socket wrapper
|   |**[sts_net](https://github.com/kieselsteini/sts)**                     | **public domain**    |C/C++|**1**| cross-platform socket wrapper (socket sets and packet API)
|   |  [znet](https://github.com/starwing/znet)                             | MIT                  |C/C++|**1**| cross-platform networking w/ Lua binding
|   |  [mm_web.h](https://github.com/vurtun/mmx)                            | BSD                  |C/C++|**1**| lightweight webserver, fork of webby
|   |  [yocto](https://github.com/tom-seddon/yhs)                           | **public domain**    |C/C++|  2  | non-production-use HTTP server
|   |  [mongoose](https://github.com/cesanta/mongoose)                      | GPLv2                |C/C++|  2  | HTTP server
|   |  [EWS](https://github.com/hellerf/EmbeddableWebServer)                | BSD                  |C/C++|**1**| HTTP server
|   |  [civetweb](https://github.com/civetweb/civetweb)                     | MIT                  |C/C++|  2  | HTTP server, fork of Mongoose
|   |  [par_easycurl.h](https://github.com/prideout/par)                    | MIT                  |C/C++|**1**| cURL wrapper
|   |  [happyhttp](https://github.com/Zintinio/HappyHTTP)                   | zlib                 | C++ |  2  | HTTP client requests
|   |**[http](https://github.com/mattiasgustavsson/libs)**                  | **public domain**    |C/C++|**1**| HTTP get/post
|   |  [LUrlParser](https://github.com/corporateshark/LUrlParser)           | MIT                  | C++ |  2  | lightweight URL & URI parser RFC 1738, RFC 3986

# serialization
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [archive](https://github.com/voidah/archive)                         |**public domain**     | C++ |**1**| binary serialize & deserlize w/ STL support

# json
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [PicoJSON](https://github.com/kazuho/picojson)                       | BSD                  | C++ |**1**| JSON parse/serializer
|   |  [json.h](https://github.com/sheredom/json.h)                         | **public domain**    |C/C++|  2  | JSON parser
|   |  [jzon.h](https://github.com/Zguy/Jzon)                               | MIT                  | C++ |  2  | JSON parser
|   |  [parson](https://github.com/kgabis/parson)                           | MIT                  |C/C++|  2  | JSON parser and serializer
|   |  [json.hpp](https://github.com/nlohmann/json)                         | MIT                  | C++ |**1**| JSON parse, serialize, deserialize
|   |  [cJSON](https://sourceforge.net/projects/cjson/)                     | MIT                  |C/C++|**1**| JSON parser
|   |  [ajson](https://github.com/lordoffox/ajson)                          | Boost                | C++ |**1**| JSON serialize & deserialize w/ STL support

# parsing
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [SLRE](https://github.com/cesanta/slre)                              |_GPLv2_               |C/C++|**1**| regular expression matcher
|   |  [mm_lexer.h](https://github.com/vurtun/mmx)                          | zlib                 |C/C++|**1**| C-esque language lexer
|   |  [minilibs](https://github.com/ccxvii/minilibs)                       | **public domain**    |  C  |  2  | two-file regex (also binary tree, etc)
|   |  [tinymemfile](https://github.com/RandyGaul/tinyheaders)              | zlib                 | C++ |**1**| fscanf on in-memory files
|   |  [inih](https://github.com/benhoyt/inih)                              | BSD                  |C/C++|  2  | .ini file parser
|   |**[ini.h](https://github.com/mattiasgustavsson/libs)**                 | **public domain**    |C/C++|**1**| .ini file parser
|   |  [cmp](https://github.com/camgunz/cmp)                                | MIT                  |C/C++|  2  | MessagePack parser and serializer

# profiling
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [Remotery](https://github.com/Celtoys/Remotery)                      | Apache 2.0           |C/C++|  2  | CPU/GPU profiler Win/Mac/Linux, using web browser for viewer
|   |  [MicroProfile](https://github.com/jonasmr/microprofile)              | **public domain**    | C++ | 2-4 | CPU (and GPU?) profiler, 1-3 header files, uses miniz internally
|   |  [prof](https://github.com/cyrus-and/prof)                            | MIT                  |C/C++|**1**| profiler for Linux

# scripting
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [LIL](http://runtimeterror.com/tech/lil/)                            | zlib                 |C/C++|  2  | interpreter for a Tcl-like scripting language
|   |  [lualite](https://github.com/user1095108/lualite)                    | MIT                  | C++ |**1**| generate Lua bindings in C++
|   |  [Picol](https://chiselapp.com/user/dbohdan/repository/picol/)        | BSD                  |C/C++|**1**| interpreter for a Tcl-like scripting language
|   |  [s7](https://ccrma.stanford.edu/software/snd/snd/s7.html)            | BSD                  |C/C++|  2  | interpreter for a subset of Scheme (R5RS/R7RS)
|   |  [Duktape](http://duktape.org/)                                       | MIT                  |  C  |  2  | embeddable JavaScript engine
|   |  [MY-BASIC](https://github.com/paladin-t/my_basic/)                   | MIT                  |  C  |  2  | interpreter for a BASIC dialect scripting language

# strings
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |**[DG_misc.h](https://github.com/DanielGibson/Snippets/)**             | **public domain**    |C/C++|**1**| Daniel Gibson's stb.h-esque cross-platform helpers: path/file, strings         
|   |**[utf8](https://github.com/sheredom/utf8.h)**                         | **public domain**    |C/C++|**1**| UTF-8 string library
|   |**[strpool.h](https://github.com/mattiasgustavsson/libs)**             | **public domain**    |C/C++|**1**| string interning
|   |  [dfa](http://bjoern.hoehrmann.de/utf-8/decoder/dfa/)                 | MIT                  |C/C++|  2  | fast UTF-8 decoder (need a header file)
|   |**[gb_string.h](https://github.com/gingerBill/gb)**                    | **public domain**    |C/C++|**1**| dynamic strings
|   |  [inja.hpp](https://github.com/pantor/inja)                           | MIT                  | C++ |**1**| template engine

# tests
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [utest](https://github.com/evolutional/utest)                        | MIT                  |C/C++|**1**| unit testing
|   |  [catch](https://github.com/philsquared/Catch)                        | Boost                | C++ |**1**| unit testing
|   |  [doctest](https://github.com/onqtam/doctest)                         | MIT                  | C++ |**1**| unit testing
|   |  [SPUT](http://www.lingua-systems.com/unit-testing/)                  | BSD                  |C/C++|**1**| unit testing
|   |  [minctest](https://github.com/codeplea/minctest)                     | zlib                 |  C  |**1**| unit testing
|   |  [greatest](https://github.com/silentbicycle/greatest)                | iSC                  |  C  |**1**| unit testing
|   |  [µnit](https://github.com/nemequ/munit)                              | MIT                  |  C  |**1**| unit testing
|   |**[labrat](https://github.com/squarewave/labrat)**                     | **public domain**    |C/C++|**1**| unit testing
|   |  [hippomocks](https://github.com/dascandy/hippomocks)                 | LGPL                 | C++ |**1**| unit testing
|   |  [fctx](https://github.com/imb/fctx)                                  | BSD                  |C/C++|**1**| unit testing
|   |  [catch](https://github.com/philsquared/Catch)				                | Boost                | C++ |**1**| unit testing
|   |  [trompeloeil](https://github.com/rollbear/trompeloeil)                                   | Boost                | C++ |**1**| unit testing

# user interface
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [dear imgui](https://github.com/ocornut/imgui)                       | MIT                  | C++ |  9  | an immediate-mode GUI formerly named "ImGui"; [3rd-party C wrapper](https://github.com/Extrawurst/cimgui)
|   |  [nuklear](https://github.com/vurtun/nuklear)                         | **public domain**    |C/C++|**1**| minimal GUI toolkit
|   |  [noc_file_dialog.h](https://github.com/guillaumechereau/noc)         | MIT                  |C/C++|  1  | file open/save dialogs (Win/Mac/Linux)
|   |  [tinyfiledialogs](https://sourceforge.net/projects/tinyfiledialogs/) | ZLIB                 |C/C++|  2  | modal dialogs inc. file open/save (Win/Mac/Linux)
|   |  [linenoise](https://github.com/antirez/linenoise)                    | BSD                  |C/C++|  2  | terminal readline w/ history etc
|   |  [wcwidth9](https://github.com/joshuarubin/wcwidth9)                  | Apache 2.0           | C   |  1  | platform independent wcwidth with full unicode 9 support

# vectors
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [mm_vec.h](https://github.com/vurtun/mmx)                            | BSD                  |C/C++|**1**| SIMD vector math
|   |**[Handmade Math](https://github.com/StrangeZak/Handmade-Math)**       | **public domain**    |C/C++|**1**| vector math
|   |**[gb_math](https://github.com/gingerBill/gb/blob/master/gb_math.h)**  | **public domain**    |C/C++|**1**| Vector, quaternion and matrix math w/o math.h
|   |**[ccVector.h](https://github.com/jobtalle/ccVector)**                 | **public domain**    |C/C++|**1**| Vector, quaternion and matrix math
|   |  [linalg.h](https://github.com/sgorsten/linalg)                       | **public domain**    | C++ |**1**| vector/matrix/quaternion math
|   |  [linalg](https://github.com/ilyak/linalg)                            | ISC                  |C/C++|**1**| vector/matrix/quaternion math
|   |  [algebra3.h](http://www.animats.com/source/graphics/algebra3.h)      | **public domain**    | C++ |**1**| vector utilities for 2, 3, and 4 element vectors, all inline

# video
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [jo_mpeg](http://www.jonolick.com/home/mpeg-video-writer)            | **public domain**    | C++ |**1**| MPEG file writer

# videogames
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |**[app.h](https://github.com/mattiasgustavsson/libs)**                 | **public domain**    |C/C++|**1**| Windows-only-but-meant-to-be-cross-platform game-ish framework

# miscellaneous
|   | library                                                               | license              | API |files| description
|---| --------------------------------------------------------------------- |:--------------------:|:---:|:---:| -----------
|   |  [MakeID.h](http://www.humus.name/3D/MakeID.h)                        | **public domain**    | C++ |**1**| allocate/deallocate small integer IDs efficiently
|   |  [tinyformat](https://github.com/c42f/tinyformat)                     | Boost                | C++ |**1**| typesafe printf
|   |  [visit_struct](https://github.com/cbeck88/visit_struct)              | Boost                | C++ |  2  | struct-field reflection
|   |  [stmr](https://github.com/wooorm/stmr.c)                             | MIT                  |  C  |  2  | extract English word stems
|   |  [levenshtein](https://github.com/wooorm/levenshtein.c)               | MIT                  |C/C++|  2  | compute edit distance between two strings
|   |  [tinytime](https://github.com/RandyGaul/tinyheaders)                 | zlib                 |C/C++|**1**| quick-and-dirty time elapsed time
|   |  [cpp-generators](https://github.com/c-smile/cpp-generators)          | BSD                  | C++ |**1**| generators in C++
|   |  [PlusCallback](https://github.com/codeplea/pluscallback)             | zlib                 | C++ |**1**| function/method callbacks
|   |  [random](https://github.com/effolkronium/random)                     | MIT                  | C++ |**1**| convenient API for random


There are also these XML libraries, but if you're using XML, shame on you:                                             

- parsing: [tinyxml2](https://github.com/leethomason/tinyxml2): XML                                                    
- parsing: [pugixml](http://pugixml.org/): XML (MIT license)

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
