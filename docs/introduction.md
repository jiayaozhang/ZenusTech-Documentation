# Introduction

[![CMake](https://github.com/zenustech/zeno/actions/workflows/cmake.yml/badge.svg)](https://github.com/zenustech/zeno/actions/workflows/cmake.yml) [![License](https://img.shields.io/badge/license-MPLv2-blue)](LICENSE) [![Version](https://img.shields.io/github/v/release/zenustech/zeno)](https://github.com/zenustech/zeno/releases)
<a class="github-button" href="https://github.com/zenustech/zeno" data-icon="octicon-star" data-show-count="true" aria-label="Star zenustech/zeno on GitHub">Star</a>

[Download](https://github.com/zenustech/zeno/releases) | [Repo](https://github.com/zenustech/zeno) | [About us](https://zenustech.com) | [Tutorial](https://zenustech.com/tutorial) | [Videos](https://space.bilibili.com/263032155) | [Q&A Forum](https://github.com/zenustech/zeno/discussions) | [Bug report](https://github.com/zenustech/zeno/issues)

[国内高速下载](https://gitee.com/zenustech/zeno/releases) | [Gitee 镜像仓库](https://gitee.com/zenustech/zeno) | [公司主页](https://zenustech.com) | [中文教程](https://zenustech.com/tutorial) | [视频教程](https://space.bilibili.com/263032155) | [问答论坛](https://github.com/zenustech/zeno/discussions) | [BUG 反馈](https://github.com/zenustech/zeno/issues)

Open-source node system framework, to change your algorithmic code into useful tools to create much more complicated simulations!

![rigid3.zsg](/images/rigid3.jpg "arts/rigid3.zsg")

ZENO is an OpenSource, Node based 3D system able to produce cinematic physics effects at High Efficiency, it was designed for large scale simulations and has been tested on complex setups.
Aside of its simulation Tools, ZENO provides necessary visualization nodes for users to import and run simulations if you feel that the current software you are using is too slow.

## Features

Integrated Toolbox, from volumetric geometry process tools (OpenVDB), to state-of-art, commercially robust, highly optimized physics solvers and visualization
nodes, and various VFX and simulation solutions based on our nodes (provided by .zsg file in `graphs/` folder).

## Gallery

![robot hit water](/images/crag_hit_water.gif)

![SuperSonic Flow](/images/shock.gif)


# End-user Installation

## Download binary release

Go to the [release page](https://github.com/zenustech/zeno/releases/), and click Assets -> download `zeno-linux-20xx.x.x.tar.gz`.
Then, extract this archive, and simply run `./launcher` (`launcher.exe` for Windows), then the node editor window will shows up if everything is working well.

## How to play

There are some example graphs in the `graphs/` folder, you may open them in the editor and have fun!
Hint: To run an animation for 100 frames, change the `1` on the top-left of node editor to `100`, then click `Run`.
Also MMB to drag in the node editor, LMB click on sockets to create connections. MMB drag in the viewport to orbit camera, Shift+MMB to pan camera.
More details are available in [our official tutorial](https://zenustech.com/tutorial).

## Bug report

If you find the binary version didn't worked properly or some error message has been thrown on your machine, please let me know by opening an [issue](https://github.com/zenustech/zeno/issues) on GitHub, thanks for you support!


# Developer Build

To build ZENO, you need:

- GCC 9+ or MSVC 19+, CMake 3.12+, and Python 3.6+ to build ZENO.
- Pybind11, NumPy and PySide2 (Qt for Python) to run ZENO editor.
- (Optional) OpenVDB for building volume nodes; CUDA for GPU nodes.

> Hint: for Python, please try avoid using virtualenv and Conda if possible.
> WSL is also not recommended because of its limited GUI and OpenGL support.

Click links below for detailed setup for each platform:

- [Windows 10](/docs/dev_win10.md)
- [Ubuntu 20.04](/docs/dev_ubuntu20.md)
- [CentOS 7](/docs/dev_centos7.md)
- [Arch Linux](/docs/dev_archlinux.md)

After finishing building, use `run.py` to run ZENO for development! You may click `File -> Open` to play `graphs/LorenzParticleTrail.zsg` to confirm everything is working well :)


# Miscellaneous

## Write your own extension!

See [zenustech/zeno_addon_wizard](https://github.com/zenustech/zeno_addon_wizard) for an example on how to write custom nodes in ZENO.

## Blender addon

Like Blender? Be sure to check out [ZenoBlend](https://github.com/zenustech/zenoblend)!

## Contact & Support

- Create a [GitHub issue](https://github.com/zenustech/zeno/issues) for bug reports, feature requests, or questions.
- Follow [@jiayaozhang](https://github.com/jiayaozhang) and [@archibate](https://github.com/archibate) for announcements.
- Add a ⭐️ [star on GitHub](https://github.com/zenustech/zeno) or ❤️ [tweet](https://twitter.com/archibate) to support the project!

## License

This project is licensed under the [Mozilla Public License](https://github.com/zenustech/zeno/blob/master/LICENSE).

Copyright (c) ZENUSTECH ([@ZENUS](https://github.com/zenustech/zeno))

<!-- GitHub Buttons -->
<script async defer src="https://buttons.github.io/buttons.js"></script>
