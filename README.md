# Awesome CAD — Curated List of Open-Source CAD Projects

A curated list of **valuable open-source CAD (Computer-Aided Design) software, libraries, and tools**, organized by category.  
This list focuses on **practical, reusable, and technically interesting** CAD projects for developers, engineers, and researchers.

Inspired by the *awesome-list* philosophy.

## 📑 Table of Contents

- [✏️ 2D CAD Software](#️-2d-cad-software)
  - [Desktop 2D CAD](#desktop-2d-cad)
  - [Web-Based 2D CAD](#web-based-2d-cad)

- [🧩 3D CAD Modelers](#-3d-cad-modelers)
  - [Desktop 3D CAD](#desktop-3d-cad)
  - [Web-Based 3D CAD](#web-based-3d-cad)

- [🌐 Web-Based CAD / DXF Viewers](#-web-based-cad--dxf-viewers)

- [📐 DXF / DWG Parsers & Libraries](#-dxf--dwg-parsers--libraries)

- [🧰 CAD Libraries & Kernels](#-cad-libraries--kernels)
  - [Geometry & Modeling Kernels](#geometry--modeling-kernels)
  - [Constraint Solvers](#constraint-solvers)
  - [Mesh Processing & Boolean Engines](#mesh-processing--boolean-engines)

- [📊 CAD Datasets](#-cad-datasets)

- [🤝 Contributing](#-contributing)

## ✏️ 2D CAD Software

### Desktop 2D CAD

#### LibreCAD

<https://github.com/LibreCAD/LibreCAD>

A mature, free 2D CAD application focused on DXF drafting.

**Key Features**

-   Native DXF support
-   Layers, blocks, snapping, dimensions
-   Cross-platform (Qt)
-   AutoCAD LT–style workflow

#### QCAD Community Edition

<https://github.com/qcad/qcad>

Professional-grade 2D drafting software with a long development history.

**Key Features**

-   Excellent DXF compatibility
-   ECMAScript scripting
-   Clean UI and stable core
-   Widely used in industry

### Web-Based 2D CAD

#### cad-viewer

[https://github.com/mlightcad/cad-viewer](https://github.com/mlightcad/cad-viewer)

A modern **browser-native CAD viewer** that parses DXF/DWG directly on the client.

**Key Features**

-   Client-side DXF/DWG parsing (no upload)
-   Optimized for very large drawings
-   Accurate snapping & layers
-   WebGL / Three.js based
-   Privacy-first architecture

#### Maker.js

[https://github.com/microsoft/maker.js]()

A JavaScript library for **programmatic 2D CAD geometry**.

**Key Features**

-   Declarative geometry modeling
-   DXF / SVG output
-   Perfect for CNC & laser cutting
-   Strong TypeScript support

## 🧩 3D CAD Modelers

### Desktop 3D CAD

#### FreeCAD

[https://github.com/FreeCAD/FreeCAD](https://github.com/FreeCAD/FreeCAD)

A full-featured **parametric 3D CAD system** for engineering and design.

**Key Features**

-   B-Rep modeling (OpenCascade)
-   Sketch constraints & parametrics
-   Assemblies, FEM, CAM, TechDraw
-   Massive plugin ecosystem

#### Blender

<https://github.com/blender/blender>

A world-class **mesh-based 3D creation suite** (not B-Rep CAD).

**Key Features**

-   Advanced mesh modeling
-   Geometry Nodes (procedural)
-   Python scripting
-   Industry standard for mesh workflows

#### OpenSCAD

<https://github.com/openscad/openscad>

A script-based solid modeling tool emphasizing precision and reproducibility.

**Key Features**

-   Text-based parametric modeling
-   Exact geometry
-   Excellent for 3D printing
-   Deterministic CAD output

#### build123d

[https://github.com/gumyr/build123d](https://github.com/gumyr/build123d?utm_source=chatgpt.com)

A modern **Pythonic parametric CAD framework** built on OpenCascade.

**Key Features**

-   Python-first CAD API
-   Clean, composable design
-   B-Rep modeling
-   Ideal for automation & pipelines

### Web-Based 3D CAD

#### jsketcher

[https://github.com/xibyte/jsketcher](https://github.com/xibyte/jsketcher)

A **parametric, sketch-based CAD system running in the browser**.

**Key Features**

-   Constraint-driven sketches
-   OpenCascade via WebAssembly
-   Browser-native CAD kernel
-   One of the most advanced web CAD projects

#### chili3d

[https://github.com/xiangechen/chili3d](https://github.com/xiangechen/chili3d)

A lightweight **web-based 2D/3D CAD editor** focused on sketches and parametric modeling.

**Key Features**

-   Sketch-driven CAD workflow
-   2D + 3D modeling
-   Runs fully in the browser
-   Three.js rendering
-   Ideal for CAD experimentation

## 🌐 Web-Based CAD / DXF Viewers

#### cad-viewer

[https://github.com/mlightcad/cad-viewer](https://github.com/mlightcad/cad-viewer)

High-performance CAD viewer focused on correctness and scale.

**Key Features**

-   DXF/DWG support
-   Large drawing optimization
-   Layer control & snapping
-   No server dependency

#### dxf-viewer

<https://github.com/vagran/dxf-viewer>

A minimal DXF viewer for quick embedding.

**Key Features**

-   Lightweight
-   Canvas-based rendering
-   Simple DXF support

#### three-dxf

<https://github.com/gdsestimating/three-dxf>

DXF loader for Three.js scenes.

**Key Features**

-   DXF → Three.js conversion
-   WebGL-friendly
-   Easy integration with 3D viewers

## 📐 DXF / DWG Parsers & Libraries

#### dxflib

[https://github.com/LibreCAD/dxflib]()

A widely used C++ DXF parsing library.

**Key Features**

-   Accurate DXF spec support
-   Mature & battle-tested
-   Used by LibreCAD

#### libdxfrw

<https://github.com/LibreCAD/libdxfrw>

An open-source DXF/DWG read/write library.

**Key Features**

-   DXF + DWG support
-   Multiple AutoCAD versions
-   Core dependency for LibreCAD

#### dxf-parser

<https://github.com/gdsestimating/dxf-parser>

A JavaScript DXF parser for web and Node.js.

**Key Features**

-   Browser-friendly
-   Common in web CAD viewers
-   Easy to extend

## 🧰 CAD Libraries & Kernels

### Geometry & Modeling Kernels

#### Open Cascade Technology (OCCT)

[https://github.com/Open-Cascade-SAS/occt]()

An industrial-grade **B-Rep geometry kernel**.

**Key Features**

-   Booleans, fillets, lofts, NURBS
-   STEP / IGES support
-   Used by FreeCAD, CadQuery

#### pythonOCC

<https://github.com/tpaviot/pythonocc>

Python bindings for OpenCascade.

**Key Features**

-   Rapid CAD prototyping
-   Scriptable B-Rep modeling
-   Research & automation friendly

#### libfive

<https://github.com/libfive/libfive>

A functional CAD kernel based on implicit geometry (SDF).

**Key Features**

-   Infinite resolution geometry
-   Functional modeling paradigm
-   Excellent for generative CAD

### Constraint Solvers

#### KittyCAD / ezpz

[https://github.com/KittyCAD/ezpz](https://github.com/KittyCAD/ezpz

A modern geometric constraint solver for parametric CAD.

**Key Features**

-   Rust + WebAssembly
-   Designed for sketches
-   Web-CAD ready

#### NeoGeoSolver.NET

[https://github.com/NoteCAD/NeoGeoSolver.NET](https://github.com/NoteCAD/NeoGeoSolver.NET?utm_source=chatgpt.com)

A geometric constraint solver written in C#.

**Key Features**

-   Sketch constraint solving
-   Educational & practical
-   Clean solver design

### Mesh Processing & Boolean Engines

#### CGAL

<https://github.com/CGAL/cgal>

The gold standard for computational geometry.

**Key Features**

-   Robust mesh booleans
-   Exact arithmetic
-   Research & industrial use

#### libigl

<https://github.com/libigl/libigl>

A simple geometry processing library.

**Key Features**

-   Mesh analysis & deformation
-   Academic-friendly
-   Easy integration

#### Manifold

<https://github.com/elalish/manifold>

A fast and robust mesh boolean engine.

**Key Features**

-   Handles non-manifold input
-   Used by OpenSCAD
-   Performance-focused



#### OpenVDB

<https://github.com/AcademySoftwareFoundation/openvdb>

A sparse volumetric representation library.

**Key Features**

-   Voxel-based booleans
-   CAD ↔ VFX pipelines
-   Extremely scalable



## 📊 CAD Datasets

#### ABC Dataset (Autodesk)

[https://github.com/AutodeskAILab/abc]()

A large-scale dataset of real CAD models.

**Key Features**

-   B-Rep + mesh
-   Industry-grade geometry
-   Research benchmark

#### Fusion 360 Gallery Dataset

<https://github.com/AutodeskAILab/Fusion360GalleryDataset>

Parametric CAD models with design history.

**Key Features**

-   Feature trees included
-   Ideal for ML on CAD
-   High-quality solids

## 🤝 Contributing

Contributions are welcome!
