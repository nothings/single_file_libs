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
[**andrewwillmott**](https://github.com/andrewwillmott?tab=repositories&q=&type=source&language=&sort=),
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

### Main listing

Single-header C files with clause-less licenses are highlighted.

|tag      | library | description
|:-------:|:---------|:-----------------
*2d*      |[Blendish](https://hg.sr.ht/~duangle/oui-blendish)                                                                    (1   C, MIT)           |Blender-style widget rendering using NanoVG
*2d*      |[C-Turtle](https://github.com/walkerje/C-Turtle)                                                                      (1 C++, MIT)           |Port of Python's Turtle to C++
*2d*      |[Cgl](https://github.com/Jaysmito101/cgl)                                                                             (2   C, MIT)           |C Game Library
*2d*      |[Cimg](https://cimg.eu/)                                                                                              (1 C++, CeCILL)        |Image processing toolkit (60K LoC)
*2d*      |[Colourblind](https://github.com/azmr/colourblind)                                                                    (1   C, ISC)           |Simulating colourblindness
*2d*      |[Daisy](https://github.com/sse2/daisy)                                                                                (1 C++, MIT)           |2D Graphics and text
*2d*      |[Immediate2D](https://github.com/npiegdon/immediate2d)                                                                (2 C++, PD)            |Zero-configuration, immediate-mode 2D graphics for Windows
*2d*      |[M_image.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_image.h)                   (1   C, ZLIB)          |Image processing routines
*2d*      |[RFont](https://github.com/ColleagueRiley/RFont)                                                                      (1   C, ZLIB)          |Simple-to-use lightweight single header modular font rendering library
*2d*      |[RGL](https://github.com/ColleagueRiley/RGL)                                                                          (1   C, ZLIB)          |Simple ultra-lightweight OpenGL version abstraction based on RLGL (pipeline system)
*2d*      |[Scalable-font2](https://gitlab.com/bztsrc/scalable-font2)                                                            (1   C, MIT)           |Scalable Font renderer + specification
*2d*      |[Si_normalmap](https://github.com/Sir-Irk/si_normalmap)                                                             **(1   C, PD)**          |**Image to Normal Map generator**
*2d*      |[Tigr](https://bitbucket.org/rmitton/tigr/src)                                                                        (2   C, PD)            |Quick-n-dirty window text/graphics for Windows and macOS
*2d*      |[Wfc](https://github.com/krychu/wfc)                                                                                  (1   C, MIT)           |Generate image locally similar to the input image using WFC algorithm
*3d*      |[Debug-draw](https://github.com/glampert/debug-draw)                                                                  (1 C++, PD)            |API-agnostic immediate-mode debug rendering
*3d*      |[Lightmapper](https://github.com/ands/lightmapper#lightmapper)                                                      **(1   C, PD)**          |**Use your OpenGL renderer to offline bake lightmaps**
*3d*      |[Mikktspace](https://developer.blender.org/diffusion/B/browse/master/intern/mikktspace)                               (2   C, ZLIB)          |Compute tangent space for normal mapping
*3d*      |[Model3d](https://gitlab.com/bztsrc/model3d)                                                                          (1   C, MIT)           |3D model format specification
*3d*      |[Seamoptimizer](https://github.com/ands/seamoptimizer)                                                              **(1   C, PD)**          |**Modify lightmap data to hide seams**
*3d*      |[Simple OpenGL Loader](https://github.com/tsherif/simple-opengl-loader)                                               (1   C, MIT)           |Extensible, cross-platform OpenGL loader
*3d*      |[Small3dlib](https://gitlab.com/drummyfish/small3dlib)                                                              **(1   C, CC0)**         |**Fast and portable software renderer**
*3d*      |[Stb_voxel_render](https://github.com/nothings/stb/blob/master/stb_voxel_render.h)                                  **(1   C, PD)**          |**Minecraft-esque voxel rendering "engine" with many more features**
*3d*      |[Swarmz](https://github.com/Cultrarius/Swarmz)                                                                        (1 C++, PD)            |Swarming/flocking algorithm
*3d*      |[Tinygizmo](https://github.com/ddiakopoulos/tinygizmo)                                                                (2 C++, PD)            |Gizmo objects for interactively editing 3d transformations
*3d*      |[Vertex Cache Optimizer](https://github.com/Sigkill79/sts)                                                          **(1   C, PD)**          |**Vertex cache optimization of meshes**
*3d*      |[Vulkan Memory Allocator](https://github.com/GPUOpen-LibrariesAndSDKs/VulkanMemoryAllocator)                          (1   C, MIT)           |Memory allocator for Vulkan
*ai*      |[Genann](https://github.com/codeplea/genann)                                                                          (2   C, ZLIB)          |Simple neural networks (ANN)
*ai*      |[KANN](https://github.com/attractivechaos/kann)                                                                       (2   C, MIT)           |Automatic differentiation   (2 files)
*app*     |[RGFW](https://github.com/ColleagueRiley/RGFW)                                                                        (1   C, ZLIB)          |A multi-platform single-header user-friendly GUI framework as an alternative to GLFW
*argv*    |[Argh!](https://github.com/adishavit/argh)                                                                            (1 C++, BSD)           |Command-line argument parsing
*argv*    |[Clara](https://github.com/catchorg/Clara)                                                                            (1 C++, BOOST)         |Composable, command line parser for C++ 11 and beyond
*argv*    |[CLI11](https://github.com/CLIUtils/CLI11)                                                                            (1 C++, BSD)           |Feature-rich CLI parsing in modern C++11
*argv*    |[Cmdline](https://github.com/tanakh/cmdline)                                                                          (1 C++, BSD)           |Command-line argument parsing
*argv*    |[Flags](https://github.com/sailormoon/flags)                                                                          (1 C++, PD)            |Command-line argument parsing
*argv*    |[Kgflags](https://github.com/kgabis/kgflags)                                                                          (1   C, MIT)           |Command-line argument parsing
*argv*    |[Linkom](https://github.com/hernandp/linkom)                                                                          (1   C, MIT)           |Command-line argument parsing w/ DOS-style options
*argv*    |[Optionparser](https://optionparser.sourceforge.net/)                                                                 (1 C++, MIT)           |Command-line argument parsing
*argv*    |[Parg](https://github.com/jibsen/parg)                                                                                (2   C, PD)            |Command-line argument parsing
*argv*    |[ProgramOptions.hxx](https://github.com/Fytch/ProgramOptions.hxx)                                                     (1 C++, MIT)           |Command-line argument parsing
*audio*   |[Atomix](https://github.com/BareRose/atomix)                                                                        **(1   C, PD)**          |**Wait-free atomic sound mixer**
*audio*   |[Aw_ima.h](https://github.com/afterwise/aw-ima/blob/master/aw-ima.h)                                                  (1   C, MIT)           |IMA-ADPCM audio decoder
*audio*   |[Btac1c](https://github.com/cr88192/bgbtech_misc/blob/master/mini/btac1c_mini0.h)                                     (1   C, MIT)           |MS-IMA_ADPCM variant
*audio*   |[Chibi-xmplay](https://github.com/reduz/chibi-xmplay)                                                                 (2   C, BSD3)          |XM module playback library
*audio*   |[Geneva](https://github.com/KrzysztofSzewczyk/Geneva)                                                                 (1   C, MIT)           |Library generating 8-bit waveforms of various kinds
*audio*   |[Miniaudio](https://github.com/dr-soft/miniaudio)                                                                   **(1   C, PD)**          |**Audio playback and capture library**
*audio*   |[Minimp3](https://github.com/lieff/minimp3)                                                                         **(1   C, CC0)**         |**Minimalistic MP3 decoder with sse/neon support**
*audio*   |[MojoAL](https://github.com/icculus/mojoAL)                                                                           (1   C, ZLIB)          |Full OpenAL 1.1 implementation
*audio*   |[Nanoalsa](https://gitlab.com/bztsrc/nanoalsa)                                                                        (1   C, MIT)           |Tiny PCM playback under Linux
*audio*   |[Pocketmod](https://github.com/rombankzero/pocketmod)                                                                 (1   C, MIT)           |ProTracker MOD file renderer
*audio*   |[Stb_hexwave](https://github.com/nothings/stb/blob/master/stb_hexwave.h)                                            **(1   C, PD)**          |**Audio waveform synthesizer**
*audio*   |[Stb_vorbis](https://github.com/nothings/stb/blob/master/stb_vorbis.c)                                              **(1   C, PD)**          |**Decode ogg vorbis files from file/memory to float/16-bit signed output**
*audio*   |[TinySoundFont](https://github.com/schellingb/TinySoundFont)                                                          (1   C, MIT)           |SoundFont2 loader & synthesizer
*bench*   |[Picobench](https://github.com/iboB/picobench)                                                                        (1 C++, MIT)           |Microbenchmarking
*bench*   |[Ubench.h](https://github.com/sheredom/ubench.h)                                                                    **(1   C, PD)**          |**Microbenchmarking**
*c*       |[Errnoname](https://github.com/mentalisttraceur/errnoname)                                                            (2   C, BSD0)          |Extended errno messages
*c*       |[Minicoro](https://github.com/edubart/minicoro/)                                                                    **(1   C, PD-0MIT)**     |**Stackful cross-platform coroutine library**
*c*       |[Stb_sprintf](https://github.com/nothings/stb/blob/master/stb_sprintf.h)                                            **(1   C, PD)**          |**Fast sprintf, snprintf for C/C++**
*cpp*     |[Filesystem](https://github.com/gulrak/filesystem)                                                                    (1 C++, MIT)           |Implementation of std::filesystem
*cpp*     |[Outcome](https://github.com/ned14/outcome/tree/develop/single-header)                                                (1 C++, APACHE2-BOOST) |Outcome and result C++ containers
*crypt*   |[Ggentropy](https://github.com/mikejsavage/ggentropy)                                                                 (2 C++, ISC)           |Cross platform entropy library
*crypt*   |[Monocypher](https://monocypher.org)                                                                                  (2   C, PD)            |High-quality small cryptography library
*crypt*   |[Random3](https://github.com/MichelPaulissen/random3)                                                               **(1   C, PD)**          |**Crypt-random generator**
*crypt*   |[TweetNaCl](https://tweetnacl.cr.yp.to/software.html)                                                                 (2   C, PD)            |High-quality tiny cryptography library
*csv*     |[CSVstream](https://github.com/awdeorio/csvstream/)                                                                   (1 C++, MIT)           |CSV parser
*csv*     |[Fast C++ CSV Parser](https://github.com/ben-strasser/fast-cpp-csv-parser)                                            (1 C++, BSD)           |CSV parser
*csv*     |[Rapidcsv](https://github.com/d99kris/rapidcsv/)                                                                      (1 C++, BSD)           |CSV parser
*csv*     |[Vince's CSV Parser](https://github.com/vincentlaucsb/csv-parser)                                                     (1 C++, MIT)           |CSV parser and serializer
*date*    |[Date](https://github.com/HowardHinnant/date)                                                                         (1 C++, MIT)           |Date and time libraries
*debug*   |[B_stacktrace](https://github.com/iboB/b_stacktrace)                                                                  (1   C, MIT)           |Stack tracing
*debug*   |[Dbgtools](https://github.com/wc-duck/dbgtools)                                                                       (2   C, ZLIB)          |Cross-platform debug util libraries
*debug*   |[Debug-assert](https://github.com/foonathan/debug_assert)                                                             (1 C++, ZLIB)          |Modular assertion macro
*debug*   |[Debugbreak](https://github.com/scottt/debugbreak)                                                                    (1   C, BSD)           |Programmatic debug break
*debug*   |[Loguru](https://github.com/emilk/loguru)                                                                             (1 C++, PD)            |Flexible logging
*debug*   |[Pempek_assert.cpp](https://github.com/gpakosz/Assert)                                                                (2 C++, WTFPL2)        |Flexible assertions
*dev*     |[EasyTab](https://github.com/ApoorvaJ/EasyTab)                                                                      **(1   C, PD)**          |**Multi-platform tablet input**
*dev*     |[Libue](https://github.com/houqp/libue)                                                                               (1   C, MIT)           |Helper library for Linux device hot-plug event
*ds*      |[AArray](https://tse.gratis/aArray/)                                                                                **(1   C, PD)**          |**Arrays/strings: generic, safe**
*ds*      |[Avl](https://github.com/etherealvisage/avl)                                                                          (2   C, PD)            |AVL tree
*ds*      |[Cds_algo](https://github.com/cdwfs/algo)                                                                           **(1   C, PD)**          |**Collection of data structures (queue, stack, graph, heap...)**
*ds*      |[DG_dynarr.h](https://github.com/DanielGibson/Snippets/)                                                            **(1   C, PD)**          |**Typesafe dynamic arrays (like std::vector) for plain C**
*ds*      |[Dynarr](https://github.com/BareRose/dynarr)                                                                        **(1   C, PD)**          |**Dynamic array container**
*ds*      |[DynaVar](https://github.com/ArjArav98/DynaVar)                                                                       (1 C++, GPL3)          |Object which can store any type of primitive data type
*ds*      |[Fifo_declare.h](https://github.com/buserror/simavr/blob/master/simavr/sim/fifo_declare.h)                            (1   C, LGPL2)         |Thread/core safe FIFO
*ds*      |[Itlib](https://github.com/iboB/itlib)                                                                                (1 C++, MIT)           |Several C++11 standard-contaner-like libraries and helpers
*ds*      |[Jhr_skip_list](https://github.com/Garfield1002/jhr_skip_list)                                                        (1 C++, PD)            |Skip Lists
*ds*      |[Jrsl](https://github.com/Garfield1002/jrsl)                                                                        **(1   C, PD)**          |**Skip Lists**
*ds*      |[Klib](https://attractivechaos.github.io/klib/)                                                                       (2   C, MIT)           |Many 2-file libs: hash, sort, b-tree, etc
*ds*      |[Libintrusive](https://github.com/graphitemaster/libintrusive)                                                        (2   C, PD)            |Intrusive data structures
*ds*      |[Libpqueue](https://github.com/vy/libpqueue)                                                                          (2   C, BSD)           |Priority queue (heap)
*ds*      |[LinkedList](https://github.com/ivanseidel/LinkedList)                                                                (2   C, MIT)           |Linked list C++
*ds*      |[Mempool](https://github.com/hardikp/cpp-mempool)                                                                     (1 C++, MIT)           |Efficient minimal memory pool implementation for C++
*ds*      |[PackedArray](https://github.com/gpakosz/PackedArray)                                                                 (2   C, WTFPL2)        |Memory-efficient array of elements with non-pow2 bitcount
*ds*      |[Selist](https://github.com/ennorehling/clibs)                                                                        (2   C, ISC)           |Space-efficient linked-list
*ds*      |[Simclist](https://mij.oltrelinux.com/devel/simclist)                                                                 (2   C, BSD)           |Linked-list
*ds*      |[Stb_ds](https://github.com/nothings/stb/blob/master/stb_ds.h)                                                      **(1   C, PD)**          |**Typesafe dynamic array and hash tables for   C, will compile in C++**
*ds*      |[Uthash](https://github.com/troydhanson/uthash)                                                                       (2   C, BSD)           |Several 1-header, 1-license-file libs: generic hash, list, etc
*engine*  |[Kit](https://github.com/rxi/kit)                                                                                   **(1   C, PD)**          |**Tiny library for making small games with big pixels**
*engine*  |[OlcPixelGameEngine](https://github.com/OneLoneCoder/olcPixelGameEngine)                                              (1 C++, BSD3)          |Game engine
*engine*  |[Punity](https://github.com/martincohen/Punity)                                                                       (1   C, MIT)           |A tiny game engine in C
*file*    |[Dirent](https://github.com/tronkko/dirent)                                                                           (1   C, MIT)           |Dirent for Windows: retrieve file & dir info
*file*    |[Miniphysfs](https://github.com/edubart/miniphysfs)                                                                   (1   C, ZLIB)          |Single-file port of PhysFS, a fs/zip abstraction
*file*    |[Tfile](https://github.com/rec/tfile)                                                                                 (1 C++, MIT)           |FILE* wrapper does read-write-append-seek-close (Win/Mac/Unix)
*file*    |[TinyDir](https://github.com/cxong/tinydir)                                                                           (1   C, BSD)           |Cross-platform directory reading (Win/POSIX/MinGW)
*file*    |[Whereami](https://github.com/gpakosz/whereami)                                                                       (2   C, WTFPL2)        |Get path/filename of executable or module
*font*    |[Blit-fonts](https://github.com/azmr/blit-fonts)                                                                      (1   C, ISC)           |Bitmap font blitters
*font*    |[Ssfn.h](https://gitlab.com/bztsrc/scalable-font)                                                                     (1   C, MIT)           |Scalable/bitmap/pixmap font renderer
*font*    |[Stb_easy_font](https://github.com/nothings/stb/blob/master/stb_easy_font.h)                                        **(1   C, PD)**          |**Quick-and-dirty easy-to-deploy bitmap font for printing frame rate, etc**
*font*    |[Stb_truetype](https://github.com/nothings/stb/blob/master/stb_truetype.h)                                          **(1   C, PD)**          |**Parse, decode, and rasterize characters from truetype fonts**
*game*    |[Raycastlib.h](https://gitlab.com/drummyfish/raycastlib)                                                            **(1   C, CC0)**         |**Advanced raycasting rendering library, pure C99 with no dependencies, only 32bit int math**
*game*    |[Stb_connected_components](https://github.com/nothings/stb/blob/master/stb_connected_components.h)                  **(1   C, PD)**          |**Incrementally compute reachability on grids**
*game*    |[Stb_herringbone_wang_tile](https://github.com/nothings/stb/blob/master/stb_herringbone_wang_tile.h)                **(1   C, PD)**          |**Herringbone Wang tile map generator**
*game*    |[Stb_tilemap_editor](https://github.com/nothings/stb/blob/master/stb_tilemap_editor.h)                              **(1   C, PD)**          |**Embeddable tilemap editor**
*hash*    |[Hash.c](https://github.com/zzo38/freeheromesh/blob/trunk/hash.c)                                                     (2   C, PD)            |SHA1/SHA3/MD5 hashes
*hash*    |[Lonesha256](https://github.com/BareRose/lonesha256)                                                                **(1   C, PD)**          |**SHA256 implementation**
*hash*    |[PicoSHA2](https://github.com/okdshin/PicoSHA2)                                                                       (1 C++, MIT)           |SHA256 implementation
*hash*    |[XxHash](https://github.com/Cyan4973/xxHash)                                                                          (2   C, BSD)           |Fast hash function
*image*   |[Bitmap](https://github.com/ArashPartow/bitmap)                                                                       (1 C++, MIT)           |Bitmap decoder and utilities
*image*   |[Cro_mipmap.h](https://github.com/thebeast33/cro_lib)                                                               **(1   C, PD)**          |**Average, min, max mipmap generators**
*image*   |[Framepacker](https://github.com/paladin-t/framepacker)                                                               (1 C++, MIT)           |Texture bin packing algorithm
*image*   |[Jo_sift](https://www.jonolick.com/home/scale-invariant-feature-transform-sift-single-file-library)                 **(1   C, PD)**          |**Image feature detection and matching**
*image*   |[Stb_image](https://github.com/nothings/stb/blob/master/stb_image.h)                                                **(1   C, PD)**          |**Image loading/decoding from file/memory: JPG, PNG, TGA, BMP, PSD, GIF, HDR, PIC**
*image*   |[Stb_image_resize](https://github.com/nothings/stb/blob/master/stb_image_resize2.h)                                 **(1   C, PD)**          |**Resize images larger/smaller with good quality**
*image*   |[Stb_image_write](https://github.com/nothings/stb/blob/master/stb_image_write.h)                                    **(1   C, PD)**          |**Image writing to disk: PNG, TGA, BMP**
*image*   |[Stb_perlin](https://github.com/nothings/stb/blob/master/stb_perlin.h)                                              **(1   C, PD)**          |**Perlin's revised simplex noise w/ different seeds**
*image*   |[Stb_rect_pack](https://github.com/nothings/stb/blob/master/stb_rect_pack.h)                                        **(1   C, PD)**          |**Simple 2D rectangle packer with decent quality**
*image*   |[Tiffloader](https://github.com/MalcolmMcLean/tiffloader)                                                             (2   C, PD)            |TIFF image loader
*image*   |EXR [Miniexr](https://github.com/aras-p/miniexr)                                                                      (2 C++, PD)            |OpenEXR writer, needs header file
*image*   |EXR [Tinyexr](https://github.com/syoyo/tinyexr)                                                                       (1   C, BSD)           |EXR image read/write, uses miniz internally
*image*   |GIF [Gif.h](https://github.com/ginsweater/gif-h)                                                                      (1 C++, PD)            |Animated GIF writer (can only include once)
*image*   |GIF [Gif_load](https://github.com/hidefromkgb/gif_load)                                                             **(1   C, PD)**          |**(animated) GIF reader**
*image*   |GIF [Jo_gif.cpp](https://www.jonolick.com/home/gif-writer)                                                            (1 C++, PD)            |Animated GIF writer (CPP file can also be used as H file)
*image*   |JPG [Jpeg-compressor](https://github.com/richgel999/jpeg-compressor)                                                  (2 C++, PD)            |2-file JPEG compress, 2-file JPEG decompress
*image*   |JPG [NanoJPEG](https://keyj.emphy.de/nanojpeg/)                                                                       (1   C, MIT)           |JPEG decoder
*image*   |JPG [Tiny_jpeg.h](https://github.com/serge-rgb/TinyJPEG/)                                                           **(1   C, PD)**          |**JPEG encoder**
*image*   |JPG EXIF [Easyexif](https://github.com/mayanklahiri/easyexif)                                                         (2 C++, BSD2)          |EXIF metadata extractor for JPEG images
*image*   |JPG EXIF [TinyEXIF](https://github.com/cdcseacave/TinyEXIF)                                                           (2 C++, BSD)           |Parse EXIF data from JPEG (XMP w/ TinyXML2 lib)
*image*   |PDF [PDFgen](https://github.com/AndreRenaud/PDFGen)                                                                   (2   C, PD)            |PDF writer 
*image*   |PNG [Lodepng](https://lodev.org/lodepng/)                                                                             (2   C, ZLIB)          |PNG encoder/decoder
*image*   |PNG [Picopng.cpp](https://lodev.org/lodepng/picopng.cpp)                                                              (2 C++, ZLIB)          |Tiny PNG loader
*image*   |PNG [TinyPngOutput](https://www.nayuki.io/page/tiny-png-output)                                                       (2   C, LGPLv3)        |PNG writer 
*image*   |PNM [PNM](https://github.com/dmilos/PNM)                                                                              (1 C++, APACHE2)       |PBM, PGM and PPM reader and writer 
*image*   |SVG [NanoSVG](https://github.com/memononen/nanosvg)                                                                   (1   C, ZLIB)          |1-file SVG parser; 1-file SVG rasterizer
*image*   |WEBP [Jebp](https://github.com/matanui159/jebp)                                                                     **(1   C, 0MIT)**        |**Single header WebP decoder**
*ini*     |[Inih](https://github.com/benhoyt/inih)                                                                               (2   C, BSD)           |.ini file parser
*json*    |[Ajson](https://github.com/lordoffox/ajson)                                                                           (1 C++, BOOST)         |JSON serialize & deserialize w/ STL support
*json*    |[CJSON](https://github.com/DaveGamble/cJSON)                                                                          (1   C, MIT)           |JSON parser
*json*    |[CJSON](https://sourceforge.net/projects/cjson/)                                                                      (1   C, MIT)           |JSON parser
*json*    |[Jsmn](https://github.com/zserge/jsmn)                                                                                (1   C, MIT)           |Minimalistic JSON parser
*json*    |[Json-build](https://github.com/lcsmuller/json-build)                                                                 (1   C, MIT)           |JSON serializer
*json*    |[Json.h](https://github.com/sheredom/json.h)                                                                        **(1   C, PD)**          |**JSON parser**
*json*    |[Json.hpp](https://github.com/nlohmann/json)                                                                          (1 C++, MIT)           |JSON parse, serialize, deserialize
*json*    |[Jsonc](https://gitlab.com/bztsrc/jsonc)                                                                              (1   C, MIT)           |Extremely fast and extremely small (~60 SLoC) JSON parser
*json*    |[Jzon.h](https://github.com/Zguy/Jzon)                                                                                (2 C++, MIT)           |JSON parser
*json*    |[Parson](https://github.com/kgabis/parson)                                                                            (2   C, MIT)           |JSON parser and serializer
*json*    |[PicoJSON](https://github.com/kazuho/picojson)                                                                        (1 C++, BSD)           |JSON parse/serializer
*json*    |[Sjson](https://github.com/septag/sjson)                                                                              (1   C, BSD2)          |JSON encode/decoder
*logic*   |[FFSM2](https://github.com/andrew-gresyk/FFSM2/blob/master/include/ffsm2/machine.hpp)                                 (1 C++, MIT)           |Flat FSM
*logic*   |[HFSM2](https://github.com/andrew-gresyk/HFSM2/blob/master/include/hfsm2/machine.hpp)                                 (1 C++, MIT)           |Hierarchical FSM
*math*    |[Amoeba](https://github.com/starwing/amoeba)                                                                          (1   C, MIT)           |Constraint solver (Cassowary) w/Lua binding
*math*    |[Cds_spline](https://github.com/cdwfs/cds_spline/blob/master/cds_spline.h)                                          **(1   C, PD)**          |**Spline utils**
*math*    |[Ceval-single-header](https://github.com/e-t-sudo/ceval-single-header)                                                (1   C, MIT)           |A single-header library for parsing and evaluation of arithmetic expressions
*math*    |[Clipper](https://www.angusj.com/delphi/clipper.php)                                                                  (2 C++, BOOST)         |Line & polygon clipping & offsetting
*math*    |[Delaunay](https://github.com/BrunoLevy/geogram.psm.Delaunay)                                                         (2 C++, BSD3)          |2D and 3D Delaunay triangulation
*math*    |[Df](https://github.com/983/df)                                                                                     **(1   C, PD)**          |**Find voronoi region in linear time of size of lattice**
*math*    |[Dvector](https://github.com/BareRose/dvector)                                                                      **(1   C, PD)**          |**2D/3D vector/quaternion/matrix math library**
*math*    |[ExprTk](https://www.partow.net/programming/exprtk/index.html)                                                        (1 C++, MIT)           |Runtime mathematical expression parser and evaluation engine.
*math*    |[Fft](https://github.com/wareya/fft)                                                                                  (1 C++, PD)            |Fast Fourier Transform 
*math*    |[HMM Toolkit](https://github.com/gerbenvoshol/Hidden-Markov-Model-Toolkit)                                            (1   C, GPL2)          |Discrete and continuous Hidden Markov Models (DHMM, CHMM)
*math*    |[Jc_voronoi](https://github.com/JCash/voronoi)                                                                        (1   C, MIT)           |Find voronoi regions on float/double data
*math*    |[Linmath.h](https://github.com/datenwolf/linmath.h)                                                                 **(1   C, WTFPL2)**      |**Vector library**
*math*    |[M_math.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_math.h)                     (1   C, ZLIB)          |Math with C/OpenCL portability
*math*    |[Nanoflann](https://github.com/jlblancoc/nanoflann)                                                                   (1 C++, BSD)           |Build KD trees for point clouds
*math*    |[Nv_voronoi.h](https://www.icculus.org/~mordred/nvlib/)                                                             **(1   C, PD)**          |**Find voronoi regions on lattice w/ integer inputs**
*math*    |[Omm](https://github.com/Hectarea1996/omm)                                                                            (1 C++, MIT)           |Template open multi-methods
*math*    |[OpenNL](https://github.com/BrunoLevy/geogram.psm.OpenNL)                                                             (2 C++, BSD3)          |Linear and eigen solvers
*math*    |[Par_msquares](https://prideout.net/marching-squares)                                                                 (1   C, MIT)           |Convert (binarized) image to triangles
*math*    |[Par_shapes](https://prideout.net/shapes)                                                                             (1   C, MIT)           |Generate various 3d geometric shapes
*math*    |[Par_streamlines](https://prideout.net/blog/par_streamlines)                                                          (1   C, MIT)           |Tessellate wide lines and curves with shading attributes
*math*    |[PoissonGenerator.h](https://github.com/corporateshark/poisson-disk-generator)                                        (1 C++, MIT)           |Poisson disk points generator (disk or rect)
*math*    |[PolyPartition](https://github.com/ivanfratric/polypartition)                                                         (2 C++, MIT)           |Polygon triangulation, partitioning
*math*    |[Precision](https://github.com/possibly-wrong/precision)                                                              (1 C++, PD)            |Arbitrary-precision integer and rational arithmetic | 3 , PD) 
*math*    |[Prns.h](https://marc-b-reynolds.github.io/shf/2016/04/19/prns.html)                                                **(1   C, PD)**          |**Seekable pseudo-random number sequences**
*math*    |[Rfft.h](https://github.com/grego/rfft.h)                                                                           **(1   C, PD)**          |**Fast Fourier Tranform for arbitrary array sizes**
*math*    |[Sdf.h](https://github.com/memononen/SDF)                                                                             (1   C, MIT)           |Compute signed-distance field from antialiased image
*math*    |[ShaderFastLibs](https://github.com/michaldrobot/ShaderFastLibs)                                                      (1 C++, MIT)           |(also HLSL) Approximate transcendental functions optimized for shaders (esp. GCN)
*math*    |[Simple_linear_regression](https://github.com/torkeldanielsson/simple_linear_regression)                              (1   C, MIT)           |Simple linear regression
*math*    |[Simrank.hpp](https://github.com/roukaour/simrank)                                                                    (2 C++, MIT)           |SimRank graph similarity algorithm
*math*    |[Sobol.h](https://github.com/Marc-B-Reynolds/Stand-alone-junk/)                                                     **(1   C, PD)**          |**Sobol & stratified sampling sequences**
*math*    |[Statistics-Tool-Box](https://github.com/gerbenvoshol/Statistics-Tool-Box)                                          **(1   C, PD)**          |**Statistical functions**
*math*    |[Stb_divide](https://github.com/nothings/stb/blob/master/stb_divide.h)                                              **(1   C, PD)**          |**More useful 32-bit modulus**
*math*    |[SummedAreaTable](https://github.com/corporateshark/Summed-Area-Table.git)                                            (1 C++, MIT)           |Summed-Area Table generation and sum/avg queries
*math*    |[TinyExpr](https://github.com/codeplea/tinyexpr)                                                                      (2   C, ZLIB)          |Evaluation of math expressions from strings
*math*    |[Tomas Akenine-Moller snippets](https://tinyurl.com/ht79ndj)                                                          (2   C, PD)            |Various 3D intersection calculations, not lib-ified
*math*    |[Vmath](https://github.com/monolifed/vmath)                                                                         **(1   C, PD)**          |**Vector/matrix library**
*math*    |[Voxelizer](https://github.com/karimnaaji/voxelizer)                                                                  (1   C, MIT)           |Convert triangle mesh to voxel triangle mesh
*math*    |[Xatlas](https://github.com/jpcy/xatlas)                                                                              (2 C++, MIT)           |Mesh parameterization
*mem*     |[Buddy_alloc](https://github.com/spaskalev/buddy_alloc)                                                             **(1   C, BSD0)**        |**Buddy memory allocator**
*mem*     |[Stb_leakcheck](https://github.com/nothings/stb/blob/master/stb_leakcheck.h)                                        **(1   C, PD)**          |**Quick-and-dirty malloc/free leak-checking**
*mem*     |[Wb_alloc](https://github.com/WilliamBundy/wb_alloc)                                                                **(1   C, PD)**          |**Custom allocators in a single-header**
*mesh*    |[Cgltf](https://github.com/jkuhlmann/cgltf)                                                                           (1   C, MIT)           |GlTF 2.0 file loader
*mesh*    |[Fast_obj.h](https://github.com/thisistherk/fast_obj)                                                                 (1   C, MIT)           |Wavefront OBJ file loader
*mesh*    |[M3d.h](https://bztsrc.gitlab.io/model3d)                                                                             (1   C, MIT)           |Model 3D importer/exporter (with Blender, Goxel, WebGL JS and assimp integration) 
*mesh*    |[Objzero](https://github.com/jpcy/objzero)                                                                            (2   C, MIT)           |Wavefront OBJ file loader
*mesh*    |[Qll_q3.h](https://github.com/dav64/qll)                                                                              (1 C++, WTFPL2)        |Quake3 BSP loader
*mesh*    |[Tinyobjloader-c](https://github.com/syoyo/tinyobjloader-c)                                                           (1   C, MIT)           |Wavefront OBJ file loader
*mesh*    |[Tinyobjloader](https://github.com/syoyo/tinyobjloader)                                                               (1 C++, MIT)           |Wavefront OBJ file loader
*mesh*    |[Tinyply](https://github.com/ddiakopoulos/tinyply)                                                                    (2 C++, PD)            |PLY mesh file loader
*mesh*    |[Tk_objfile](https://github.com/joeld42/tk_objfile)                                                                   (1   C, MIT)           |OBJ file loader
*misc*    |[ASAP](https://github.com/mobius3/asap)                                                                               (1 C++, MIT)           |Library for parsing, printing, iterating and operating on dates.
*misc*    |[CLM_LIBS](https://github.com/CarlosLunaMota/CLM_LIBS)                                                              **(1   C, PD)**          |**Diverse utilities**
*misc*    |[Color-Toolkit](https://github.com/gerbenvoshol/Color-Toolkit)                                                        (1   C, GPL2)          |Color conversion utils (RGB, XYZ, Lab, CIE76, CIE94 and CIEDE200)
*misc*    |[Cpp-generators](https://github.com/c-smile/cpp-generators)                                                           (1 C++, BSD)           |Generators in C++
*misc*    |[Ebnn.h](https://github.com/kunglab/ebnn/blob/master/c/ebnn.h)                                                        (1   C, MIT)           |BNN (Binarized Neural Networks)
*misc*    |[H.h](https://github.com/robertsdotpm/h.h)                                                                            (1   C, GPL3)          |Diverse utilities
*misc*    |[Hedley](https://nemequ.github.io/hedley/)                                                                          **(1   C, PD)**          |**Compiler portability, optimization, static analysis, etc.**
*misc*    |[MakeID.h](https://www.humus.name/3D/MakeID.h)                                                                        (1 C++, PD)            |Allocate/deallocate small integer IDs efficiently
*misc*    |[Mmu](https://github.com/CN-xLeaves/mmu)                                                                              (2   C, MIT)           |Memory management and data structure toolset
*misc*    |[OpenGA](https://github.com/Arash-codedev/openGA)                                                                     (1 C++, MPL2)          |A C++ Generic Algorithm solver library
*misc*    |[PlusCallback](https://github.com/codeplea/pluscallback)                                                              (1 C++, ZLIB)          |Function/method callbacks
*misc*    |[Process.h](https://github.com/sheredom/process.h)                                                                  **(1   C, PD)**          |**Process control API**
*misc*    |[QR-Code-generator](https://github.com/nayuki/QR-Code-generator)                                                      (2   C, MIT)           |QR Code generator
*misc*    |[Qsort](https://github.com/svpv/qsort)                                                                                (1   C, MIT)           |Qsort algorithm as a C macro
*misc*    |[Scogem.c](https://github.com/zzo38/scorpion/blob/trunk/scogem.c)                                                     (2   C, PD)            |URL parser
*misc*    |[Sili](https://github.com/EimaMei/sili)                                                                             **(1   C, PD)**          |**C toolchain for modern C programming, strings, arrays, files, threading, ect**
*misc*    |[Smallxrm.c](https://github.com/zzo38/freeheromesh/blob/trunk/smallxrm.c)                                             (2   C, PD)            |Implementation of X resource manager
*misc*    |[Stb_include](https://github.com/nothings/stb/blob/master/stb_include.h)                                            **(1   C, PD)**          |**Implement recursive #include support, particularly for GLSL**
*misc*    |[Stmr](https://github.com/wooorm/stmr.c)                                                                              (2   C, MIT)           |Extract English word stems
*misc*    |[X.h](https://github.com/Neur1n/x.h)                                                                                  (1   C, MULAN2)        |Cross-platform C/C++ utilities
*nav*     |[M_path_finding.h](https://github.com/anael-seghezzi/Maratis-Tiny-C-library/blob/master/include/m_path_finding.h)     (1   C, ZLIB)          |Floodfill-based path finding
*nav*     |[Micropather](https://www.grinninglizard.com/MicroPather/)                                                            (2 C++, ZLIB)          |Pathfinding with A\*
*net*     |[Civetweb](https://github.com/civetweb/civetweb)                                                                      (2   C, MIT)           |HTTP server, fork of Mongoose
*net*     |[Cpp-httplib](https://github.com/yhirose/cpp-httplib)                                                                 (1   C, MIT)           |Cross-platform HTTP server/client
*net*     |[Enet](https://github.com/zpl-c/enet)                                                                                 (1   C, MIT)           |Reliable UDP networking library
*net*     |[EWS](https://github.com/hellerf/EmbeddableWebServer)                                                                 (1   C, BSD)           |HTTP server
*net*     |[Happyhttp](https://github.com/mingodad/HappyHTTP)                                                                    (2 C++, ZLIB)          |HTTP client requests
*net*     |[Libcluon](https://github.com/chrberger/libcluon)                                                                     (1 C++, MPL2)          |Cross-platform socket wrapper and data marshalling with native implementations for [Protobuf](https://developers.google.com/protocol-buffers/), [LCM](https://lcm-proj.github.io/type_specification.html)/[ZCM](https://zerocm.github.io/zcm/), JSON, and [MsgPack](https://msgpack.org) serialization/deserialization
*net*     |[Librg](https://github.com/zpl-c/librg)                                                                               (1   C, BSD3)          |World/entity synchronization multiplayer library
*net*     |[LUrlParser](https://github.com/corporateshark/LUrlParser)                                                            (2 C++, MIT)           |Lightweight URL & URI parser RFC 1738, RFC 3986
*net*     |[Mongoose](https://github.com/cesanta/mongoose)                                                                       (2   C, GPLv2)         |HTTP server
*net*     |[Netq](https://gitlab.com/bztsrc/netq)                                                                                (1   C, MIT)           |Reliable datagram library
*net*     |[Par_easycurl.h](https://github.com/prideout/par)                                                                     (1   C, MIT)           |CURL wrapper
*net*     |[Simpletls.c](https://github.com/zzo38/scorpion/blob/trunk/simpletls.c)                                               (2   C, PD)            |Function to create a socket and connect to a remote server with TLS
*net*     |[Swrap](https://github.com/BareRose/swrap)                                                                          **(1   C, PD)**          |**TCP and UDP socket wrapper**
*net*     |[Tiniest-analytics](https://github.com/Pintea/tiniest-analytics)                                                      (2 C++, MIT)           |Cross-platform analytics for games (using Google Analytics <4)
*net*     |[Tiny-MQTT-c](https://github.com/kokke/tiny-MQTT-c)                                                                   (4   C, PD)            |Small implementation of (some of) the MQTT protocol in C
*net*     |[Tlse](https://github.com/eduardsui/tlse)                                                                             (2   C, PD-BSD2)       |TLS v1.0, 1.2, 1.3 and DTLS 1.0, 1.2 implementations
*net*     |[Webster](https://github.com/brunexgeek/webster)                                                                      (2 C++, APACHE2)       |Standalone HTTP server/client
*net*     |[Yocto](https://github.com/tom-seddon/yhs)                                                                            (2   C, PD)            |Non-production-use HTTP server
*net*     |[Zed_net](https://github.com/Smilex/zed_net)                                                                        **(1   C, PD)**          |**Cross-platform socket wrapper**
*net*     |[Znet](https://github.com/starwing/znet)                                                                              (1   C, MIT)           |Cross-platform networking w/ Lua binding
*pack*    |[Dmc_unrar](https://github.com/DrMcCoy/dmc_unrar)                                                                     (1   C, GPL2)          |RAR file decompression
*pack*    |[Fastlz](https://code.google.com/archive/p/fastlz/source/default/source)                                              (2   C, MIT)           |Fast but larger LZ compression
*pack*    |[Lz4](https://github.com/lz4/lz4)                                                                                     (2   C, BSD)           |Fast but larger LZ compression
*pack*    |[Microtar](https://github.com/rxi/microtar)                                                                           (2   C, MIT)           |Lightweight tar library
*pack*    |[Miniz.c](https://github.com/richgel999/miniz)                                                                        (1   C, MIT)           |Compression, decompression, ZIP file, PNG writing
*pack*    |[Nibrans](https://github.com/BareRose/nibrans)                                                                      **(1   C, PD)**          |**Adaptive rANS library**
*pack*    |[Pithy](https://github.com/johnezang/pithy)                                                                           (2   C, BSD)           |Fast but larger LZ compression
*pack*    |[Rle](https://gitlab.com/bztsrc/rle)                                                                                  (1   C, MIT)           |Run-length en/decoder
*pack*    |[Stb_dxt](https://github.com/nothings/stb/blob/master/stb_dxt.h)                                                    **(1   C, PD)**          |**Real-time DXT compressor**
*parse*   |[Cmp](https://github.com/camgunz/cmp)                                                                                 (2   C, MIT)           |MessagePack parser and serializer
*parse*   |[Cpp-peglib](https://github.com/yhirose/cpp-peglib)                                                                   (1   C, MIT)           |PEG (Parsing Expression Grammars) library
*parse*   |[Furi](https://github.com/iboB/furi)                                                                                  (1   C, MIT)           |URL & URI parsing
*parse*   |[Html-parse.c](https://git.savannah.gnu.org/cgit/wget.git/tree/src/html-parse.c)                                      (2   C, GPL)           |HTML parser (wget)
*parse*   |[SLRE](https://github.com/cesanta/slre)                                                                               (1   C, GPL2)          |Regular expression matcher
*parse*   |[Stb_c_lexer](https://github.com/nothings/stb/blob/master/stb_c_lexer.h)                                            **(1   C, PD)**          |**Simplify writing parsers for C-like languages**
*parse*   |[Tok](https://gitlab.com/bztsrc/tok)                                                                                  (1   C, MIT)           |Configurable tokenizer
*parse*   |[Tomlplusplus](https://github.com/marzer/tomlplusplus)                                                                (1 C++, MIT)           |TOML parser and serializer
*parse*   |[Udisasm](https://gitlab.com/bztsrc/udisasm)                                                                          (1   C, MIT)           |Extremely small disassembler for ARMv8.2 AArch64 (~65k) 
*parse*   |[Unformat](https://github.com/adamyaxley/Unformat)                                                                    (1 C++, PD)            |Parses formatted strings (reverse of std::format)
*prng*    |[Random](https://github.com/effolkronium/random)                                                                      (1 C++, MIT)           |Convenient API for random
*prng*    |[Ranxoshi256](https://github.com/BareRose/ranxoshi256)                                                              **(1   C, PD)**          |**Xoshiro256 algorithm**
*prng*    |[SimplexNoise](https://github.com/simongeilfus/SimplexNoise)                                                          (1 C++, BSD2)          |Collection of noise generators
*profile* |[MicroProfile](https://github.com/jonasmr/microprofile)                                                               (4 C++, PD)            |CPU (and GPU?) profiler, 1-3 header files, uses miniz internally 
*profile* |[Prof](https://github.com/cyrus-and/prof)                                                                             (1   C, MIT)           |Profiler for Linux
*profile* |[Remotery](https://github.com/Celtoys/Remotery)                                                                       (2   C, APACHE2)       |CPU/GPU profiler Win/Mac/Linux, using web browser for viewer
*raster*  |[Canvas_ity](https://github.com/a-e-k/canvas_ity)                                                                     (1 C++, ISC)           |2D rasterizer
*regex*   |[Remimu](https://github.com/wareya/Remimu)                                                                          **(1   C, CC0)**         |**Regex engine**
*script*  |[Duktape](https://duktape.org/)                                                                                       (2   C, MIT)           |Embeddable JavaScript engine
*script*  |[LIL](https://runtimeterror.com/tech/lil/)                                                                            (2   C, ZLIB)          |Interpreter for a Tcl-like scripting language
*script*  |[Lualite](https://github.com/user1095108/lualite)                                                                     (1 C++, MIT)           |Generate Lua bindings in C++
*script*  |[Minilua](https://github.com/edubart/minilua)                                                                         (1   C, MIT)           |Single-file port of Lua scripting language
*script*  |[MY-BASIC](https://github.com/paladin-t/my_basic/)                                                                    (2   C, MIT)           |Interpreter for a BASIC dialect scripting language
*script*  |[Picol](https://chiselapp.com/user/dbohdan/repository/picol/)                                                         (1   C, BSD)           |Interpreter for a Tcl-like scripting language
*script*  |[S7](https://ccrma.stanford.edu/software/snd/snd/s7.html)                                                             (2   C, BSD)           |Interpreter for a subset of Scheme (R5RS/R7RS)
*script*  |[Xpl](https://github.com/paladin-t/xpl)                                                                             **(1   C, WTFPL2)**      |**X Programming Language**
*serial*  |[Archive](https://github.com/voidah/archive)                                                                          (1 C++, PD)            |Binary serialize & deserlize w/ STL support
*serial*  |[Blob_tree](https://github.com/dicroce/blob_tree)                                                                     (1 C++, MIT)           |Binary tree serializer
*serial*  |[Cista](https://github.com/felixguendling/cista)                                                                      (1 C++, MIT)           |Cross-platform high performance zero copy C++17 serialization/deserialization
*serial*  |[Libcluon](https://github.com/chrberger/libcluon)                                                                     (1 C++, MPL2)          |Cross-platform data serialization/deserialization with native implementations for [Protobuf](https://developers.google.com/protocol-buffers/), [LCM](https://lcm-proj.github.io/type_specification.html)/[ZCM](https://zerocm.github.io/zcm/), JSON, and [MsgPack](https://msgpack.org)
*serial*  |[Qserial](https://github.com/earonesty/qserial)                                                                       (1 C++, BSD3)          |Schema-driven serialization library
*serial*  |[Serialization helper](https://gist.github.com/TheServer201/9ae5322cd52f76c7d36af15d3b366762)                       **(1   C, WTFPL2)**      |**Serialization helper**
*serial*  |[Visit_struct](https://github.com/cbeck88/visit_struct)                                                               (2 C++, BOOST)         |Struct-field reflection
*string*  |[Csplit](https://github.com/jwlodek/csplit)                                                                           (1   C, MIT)           |String splitting and processing single-header library
*string*  |[Dfa](https://bjoern.hoehrmann.de/utf-8/decoder/dfa/)                                                                 (2   C, MIT)           |Fast UTF-8 decoder (need a header file)
*string*  |[Gb_string.h](https://github.com/gingerBill/gb)                                                                     **(1   C, PD)**          |**Dynamic strings**
*string*  |[Ggformat](https://github.com/mikejsavage/ggformat)                                                                   (2 C++, ISC)           |Printf replacement
*string*  |[Inja.hpp](https://github.com/pantor/inja)                                                                            (1 C++, MIT)           |Template engine
*string*  |[Levenshtein](https://github.com/wooorm/levenshtein.c)                                                                (2   C, MIT)           |Compute edit distance between two strings
*string*  |[Obfuscate](https://github.com/adamyaxley/Obfuscate)                                                                  (1 C++, PD)            |Guaranteed compile-time string literal obfuscation library for C++14
*string*  |[Str.h](https://github.com/ocornut/Str)                                                                               (1 C++, PD)            |Simple C++ string type with an optional local buffer
*string*  |[Str](https://github.com/maxim2266/str)                                                                               (2   C, BSD)           |Yet another string library for C language
*string*  |[Str_view.hpp](https://github.com/sawickiap/str_view)                                                                 (1 C++, MIT)           |Null-termination-aware string-view class
*string*  |[Tinyformat](https://github.com/c42f/tinyformat)                                                                      (1 C++, BOOST)         |Typesafe printf
*string*  |[Utf8](https://github.com/sheredom/utf8.h)                                                                          **(1   C, PD)**          |**UTF-8 string library**
*svg*     |[SimpleSVG](https://github.com/adishavit/simple-svg)                                                                  (1 C++, BSD3)          |Easy to use SVG library
*sys*     |[Doops](https://github.com/eduardsui/doops)                                                                         **(1   C, PD)**          |**Event loop library**
*sys*     |[Endianness.h](https://github.com/rofl0r/endianness.h)                                                              **(1   C, PD)**          |**Endianness conversion and detection**
*sys*     |[JArgsParser](https://github.com/ZhengqiaoWang/JArgsParser)                                                           (1 C++, MIT)           |Arguments parser
*sys*     |[Openmodal](https://gitlab.com/bztsrc/openmodal)                                                                      (1   C, MIT)           |Native file modals
*sys*     |[Rang](https://github.com/agauniyal/rang)                                                                             (1 C++, PD)            |Cross-platform colored console text
*sys*     |[Xproc](https://github.com/time-killer-games/xproc)                                                                   (2 C++, MIT)           |Foreign Process Information
*thread*  |[Bikeshed.h](https://github.com/DanEngelbrecht/bikeshed)                                                              (1   C, MIT)           |Cross-platform lock free fixed memory hierarchical work scheduler
*thread*  |[Cds_job](https://github.com/cdwfs/cds_job)                                                                           (1 C++, PD)            |Lock-free job queue
*thread*  |[Cds_sync](https://github.com/cdwfs/cds_sync)                                                                       **(1   C, PD)**          |**Collection of synchronization primitives**
*thread*  |[TinyCThread](https://tinycthread.github.io/)                                                                         (2   C, ZLIB)          |Cross-platform implementation of the C11 Threads API
*thread*  |[TinyThread++](https://tinythreadpp.bitsnbites.eu/)                                                                   (2 C++, ZLIB)          |Cross-platform implementation of the C++11 Threads API
*ui*      |[Clay](https://github.com/nicbarker/clay)                                                                             (1   C, ZLIB)          |High performance 2D UI layout library
*ui*      |[Dear imgui](https://github.com/ocornut/imgui)                                                                        (9 C++, MIT)           |An immediate-mode GUI formerly named "ImGui"; [3rd-party C wrapper](https://github.com/Extrawurst/cimgui)
*ui*      |[Libcmdf](https://github.com/ronen25/libcmdf)                                                                       **(1   C, PD)**          |**A small library for writing CLI applications**
*ui*      |[Linenoise](https://github.com/antirez/linenoise)                                                                     (2   C, BSD)           |Terminal readline w/ history etc
*ui*      |[Nuklear](https://github.com/Immediate-Mode-UI/Nuklear)                                                             **(1   C, PD)**          |**Minimal GUI toolkit**
*ui*      |[Stb_textedit](https://github.com/nothings/stb/blob/master/stb_textedit.h)                                          **(1   C, PD)**          |**Guts of a text editor for games etc implementing them from scratch**
*ui*      |[Tinyfiledialogs](https://sourceforge.net/projects/tinyfiledialogs/)                                                  (2   C, ZLIB)          |Modal dialogs inc. file open/save (Win/Mac/Linux)
*ui*      |[Wcwidth9](https://github.com/joshuarubin/wcwidth9)                                                                   (1   C, APACHE2)       |Platform independent wcwidth with full unicode 9 support
*ui*      |[Webview](https://github.com/zserge/webview)                                                                          (1   C, MIT)           |Cross-platform webview library
*unit*    |[Catch2](https://github.com/catchorg/Catch2/)                                                                         (1 C++, BOOST)         |Unit testing
*unit*    |[Catch](https://github.com/philsquared/Catch)                                                                         (1 C++, BOOST)         |Unit testing
*unit*    |[Clove-unit](https://github.com/fdefelici/clove-unit)                                                                 (1   C, MIT)           |Unit testing
*unit*    |[Doctest](https://github.com/onqtam/doctest)                                                                          (1 C++, MIT)           |Unit testing
*unit*    |[Fctx](https://github.com/imb/fctx)                                                                                   (1   C, BSD)           |Unit testing
*unit*    |[Greatest](https://github.com/silentbicycle/greatest)                                                                 (1   C, ISC)           |Unit testing
*unit*    |[Hippomocks](https://github.com/dascandy/hippomocks)                                                                  (1 C++, LGPL)          |Unit testing
*unit*    |[Labrat](https://github.com/squarewave/labrat)                                                                      **(1   C, PD)**          |**Unit testing**
*unit*    |[Minctest](https://github.com/codeplea/minctest)                                                                      (1   C, ZLIB)          |Unit testing
*unit*    |[Munit](https://github.com/nemequ/munit)                                                                              (1   C, MIT)           |Unit testing
*unit*    |[Picotest](https://github.com/colinbarry/picotest)                                                                    (1   C, MIT)           |Unit testing
*unit*    |[Rexo](https://github.com/christophercrouzet/rexo)                                                                  **(1   C, PD)**          |**Framework for C89/C++ featuring automatic registration of tests and a polished API**
*unit*    |[SPUT](https://www.lingua-systems.com/unit-testing/)                                                                  (1   C, BSD)           |Unit testing
*unit*    |[Trompeloeil](https://github.com/rollbear/trompeloeil)                                                                (1 C++, BOOST)         |Unit testing
*unit*    |[Utest.h](https://github.com/sheredom/utest.h)                                                                      **(1   C, PD)**          |**Unit testing**
*unit*    |[Utest](https://github.com/evolutional/utest)                                                                         (1   C, MIT)           |Unit testing
*unit*    |[Walter](https://github.com/ir33k/walter)                                                                           **(1   C, PD)**          |**Unit testing**
*uuid*    |[Uuid4](https://github.com/gpakosz/uuid4)                                                                             (2   C, WTFPL2-MIT)    |UUID v4 generator
*uuid*    |[Uuid_h](https://github.com/wc-duck/uuid_h)                                                                           (1   C, ZLIB)          |UUID generator
*vector*  |[Algebra3.h](https://www.animats.com/source/graphics/algebra3.h)                                                      (1 C++, PD)            |Vector utilities for 2, 3, and 4 element vectors, all inline
*vector*  |[CcVector.h](https://github.com/jobtalle/ccVector)                                                                  **(1   C, PD)**          |**Vector, quaternion and matrix math**
*vector*  |[Handmade Math](https://github.com/StrangeZak/Handmade-Math)                                                        **(1   C, PD)**          |**Vector math**
*vector*  |[Hypatia](https://github.com/dagostinelli/hypatia)                                                                    (1   C, MIT)           |Vector/matrix/quaternion math
*vector*  |[Linalg.h](https://github.com/sgorsten/linalg)                                                                        (1 C++, PD)            |Vector/matrix/quaternion math
*vector*  |[Linalg](https://github.com/ilyak/linalg)                                                                             (1   C, ISC)           |Vector/matrix/quaternion math
*video*   |[Jo_mpeg](https://blog.frost.kiwi/jo-mpeg-in-c), [original](https://www.jonolick.com/home/mpeg-video-writer)        **(1   C, PD)**          |**MPEG file writer**
*video*   |[Pl_mpeg](https://github.com/phoboslab/pl_mpeg)                                                                       (1   C, MIT)           |MPEG1 video and audio decoder
*xml*     |[Pugixml](https://pugixml.org/)                                                                                       (2 C++, MIT)           |Light-weight C++ XML processing library
*xml*     |[Tinyxml2](https://github.com/leethomason/tinyxml2)                                                                   (2 C++, ZLIB)          |Simple, small, efficient, C++ XML parser
*xml*     |[Yxml](https://dev.yorhel.nl/yxml)                                                                                    (2   C, MIT)           |Small, fast and correct XML parser
*yaml*    |[Mini-yaml](https://github.com/jimmiebergmann/mini-yaml)                                                              (2 C++, MIT)           |YAML parser and serializer

### Secondary listing

Entries in this appendix either do not offer a single-header file directly, or the single-header file is computer generated, or you have to build the single-header by yourself, or lack any other major requirement mentioned above. However, some of you may find the links below still relevant.

|tag      | library | description
|:-------:|:---------|:-----------------
*db*      |[Sqlite](https://www.sqlite.org/amalgamation.html)                           (2   C, PD)     |Self-contained, SQL database engine.
*engine*  |[FWK1](https://github.com/fwk3d/v1)                                        **(1   C, PD)**   |**3D game framework in C**
*file*    |[DTW](https://github.com/OUIsolutions/DoTheWorld)                            (1   C, MIT)    |File and folder utilities
*net*     |[CWebStudio](https://github.com/OUIsolutions/CWebStudio)                     (1   C, MIT)    |WebServer with embedded JSON/HTML utilities
*pack*    |[Zstd](https://github.com/facebook/zstd/tree/dev/build/single_file_libs)     (?   C, BSD3)   |Fast real-time compression algorithm
*sys*     |[Cpuid](https://github.com/anzz1/cpuid)                                      (1   C, ???)    |Cross-platform cpuid intrinsic
*sys*     |[Iathook](https://github.com/anzz1/iathook)                                  (1   C, ???)    |Import address table hooking library (x86/x64,w32)

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

For the API column, "C" means a C library that *may be* C++ compatible but this not guaranteed nor verified,
"C++" means C++ only and thus not C compatible, and "C/C++" means a C library with additional features when compiled in C++ mode.
<!--
For the API column, "C" means C only, "C++" means C++ only, and "C/C++" means C/C++ usable
from either; some files may require *building* as C or C++ but still qualify as "C/C++" as
long as the header file uses `extern "C"` to make it work. (In some cases, a header-file-only
library may compile as both C or C++, but produce an implementation that can only be called from
one or the other, because of a lack of use of `extern "C"`; in this case the table still qualifies it
as C/C++, as this is not an obstacle to most users.)
-->

### Why are the LICENSING terms required in the header and source files?

Please note that every file that must be included in a user's project counts; a header and a source
file is 2 files, but a header file, source file, and LICENSE (if the license isn't in the
source file) is 3 files, and won't be accepted, because it's not 2 files. But actually
'LICENSE' is a problem for just dropping the library in a source tree anyway, since it's
not scoped to just the library, so library authors are encouraged to include the license in the
source file and not require a separate LICENSE.

<!--
### Why isn't SQLite's amalgamated build on this list?

Come on.
-->
