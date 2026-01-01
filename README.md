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
 
- [🧑‍💻 Code-Driven / Scriptable CAD](#-code-driven--scriptable-cad)

- [🌐 Web-Based CAD / DXF Viewers](#-web-based-cad--dxf-viewers)

- [📐 DXF / DWG Parsers & Libraries](#-dxf--dwg-parsers--libraries)

- [🧰 CAD Libraries & Kernels](#-cad-libraries--kernels)
  - [Geometry & Modeling Kernels](#geometry--modeling-kernels)
  - [Constraint Solvers](#constraint-solvers)
  - [Mesh Processing & Boolean Engines](#mesh-processing--boolean-engines)
 
- [🛠 Specialized CAD Tools](#-specialized-cad-tools)

- [📊 CAD Datasets](#-cad-datasets)

- [📚 CAD Research & Related](#-cad-research--related)

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

<https://github.com/mlightcad/cad-viewer>

A modern **browser-native CAD viewer** that parses DXF/DWG directly on the client.

**Key Features**

-   Client-side DXF/DWG parsing (no upload)
-   Optimized for very large drawings
-   Accurate snapping & layers
-   WebGL / Three.js based
-   Privacy-first architecture

#### Maker.js

<https://github.com/microsoft/maker.js>

A JavaScript library for **programmatic 2D CAD geometry**.

**Key Features**

-   Declarative geometry modeling
-   DXF / SVG output
-   Perfect for CNC & laser cutting
-   Strong TypeScript support

## 🧩 3D CAD Modelers

### Desktop 3D CAD

#### FreeCAD

<https://github.com/FreeCAD/FreeCAD>

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

<https://github.com/gumyr/build123d>

A modern **Pythonic parametric CAD framework** built on OpenCascade.

**Key Features**

-   Python-first CAD API
-   Clean, composable design
-   B-Rep modeling
-   Ideal for automation & pipelines

#### cadquery-editor

<https://github.com/CadQuery/CQ-editor>

A desktop IDE for **script-driven parametric 3D CAD** based on CadQuery and OpenCascade.

**Key Features**

-   Script-driven parametric modeling
-   Python-based CAD logic
-   Built on CadQuery + OpenCascade
-   Interactive 3D preview
-   Popular in engineering automation and design pipelines

#### SolveSpace

<https://github.com/solvespace/solvespace>

A lightweight **constraint-based parametric 2D/3D CAD system** focused on precision and simplicity.

**Key Features**

-   Strong geometric constraint solver (core strength)
-   2D sketching and 3D solid modeling
-   Parametric dimensions and relations
-   Very small, fast, and deterministic
-   Popular for mechanical sketches, linkages, and educational use
-   Fully open-source and self-contained

### Web-Based 3D CAD

#### jsketcher

<https://github.com/xibyte/jsketcher>

A **parametric, sketch-based CAD system running in the browser**.

**Key Features**

-   Constraint-driven sketches
-   OpenCascade via WebAssembly
-   Browser-native CAD kernel
-   One of the most advanced web CAD projects

#### chili3d

<https://github.com/xiangechen/chili3d>

A lightweight **web-based 2D/3D CAD editor** focused on sketches and parametric modeling.

**Key Features**

-   Sketch-driven CAD workflow
-   2D + 3D modeling
-   Runs fully in the browser
-   Three.js rendering
-   Ideal for CAD experimentation

## 🧑‍💻 Code-Driven / Scriptable CAD

Design CAD models using **code instead of GUI interactions** — ideal for **reproducible, parametric, automated, and version-controlled** workflows.

#### CadQuery

<https://github.com/CadQuery/cadquery>

A Python library for **parametric, script-based CAD modeling** built on OpenCascade.

**Key Features**

-   Pythonic CAD API
-   B-Rep modeling via OpenCascade
-   Constraint-friendly workflows
-   Widely used in engineering automation
-   Strong ecosystem (CQ-editor, exporters)

#### OpenJSCAD

<https://github.com/jscad/OpenJSCAD.org>

A JavaScript-based CAD system for **scriptable solid modeling** in the browser and Node.js.

**Key Features**

-   JavaScript CAD modeling
-   Browser and CLI support
-   CSG-based modeling
-   STL / AMF / 3MF export
-   Popular in maker and web CAD communities

#### Manifold

<https://github.com/azrecol/manifold>

A fast and robust **mesh geometry library** supporting CSG and implicit (SDF) operations.

**Key Features**

-   High-performance mesh booleans
-   CSG and SDF-based modeling
-   Robust handling of non-manifold geometry
-   Used internally by OpenSCAD
-   Suitable for CAD → mesh pipelines

#### SolidPython

<https://github.com/SolidCode/SolidPython>

A Python frontend that generates **OpenSCAD-compatible code**.

**Key Features**

-   Pythonic wrapper for OpenSCAD
-   Parametric & reproducible designs
-   Easy integration with Python tooling
-   Ideal for quick scripting and automation

## 🌐 Web-Based CAD / DXF Viewers

#### cad-viewer

<https://github.com/mlightcad/cad-viewer>

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

#### gemini-viewer-examples

<https://github.com/pattern-x/gemini-viewer-examples>

Example projects and demos showcasing the **Gemini CAD viewer**, a WebGL-based 3D viewer optimized for CAD data.

**Key Features**

-   Interactive 3D model viewing in the browser
-   WebGL/WebGPU rendering
-   Includes examples for various CAD formats
-   Good starting point for integrating web CAD viewers

## 📐 DXF / DWG Parsers & Libraries

#### LibreDWG

<https://github.com/LibreDWG/libredwg>

A C library for **reading and writing DWG files**, part of the GNU project.

**Key Features**

-   Native DWG read/write support
-   Covers multiple AutoCAD DWG versions
-   Low-level, spec-oriented implementation
-   Suitable for CAD import/export pipelines

#### ezdxf

<https://github.com/mozman/ezdxf>

A Python library for **reading, writing, and modifying DXF files**.

**Key Features**

-   High-level Python API
-   Excellent DXF spec coverage
-   Actively maintained
-   Ideal for CAD automation and data processing
-   Popular in scripting and batch workflows

#### dxflib

<https://github.com/LibreCAD/dxflib>

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

#### dxf-json

<https://github.com/dotoritos-kim/dxf-json>

A tool for **converting DXF files to JSON format** for easier processing in web and scripting environments.

**Key Features**

-   Converts DXF to structured JSON
-   Browser and Node.js friendly
-   Lightweight and easy to integrate

## 🧰 CAD Libraries & Kernels

### Geometry & Modeling Kernels

#### Open Cascade Technology (OCCT)

<https://github.com/Open-Cascade-SAS/occt>

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

<https://github.com/KittyCAD/ezpz>

A modern geometric constraint solver for parametric CAD.

**Key Features**

-   Rust + WebAssembly
-   Designed for sketches
-   Web-CAD ready

#### NeoGeoSolver.NET

<https://github.com/NoteCAD/NeoGeoSolver.NET>

A geometric constraint solver written in C#.

**Key Features**

-   Sketch constraint solving
-   Educational & practical
-   Clean solver design

#### Frontier

<https://github.com/Geoplexity/Frontier>

A research-oriented **geometric constraint solving framework** for parametric CAD systems.

**Key Features**

-   Focused on geometric constraint solving
-   Designed for sketch-based CAD
-   Emphasizes robustness and correctness
-   Suitable for academic and experimental CAD engines
-   Clear separation between geometry and solver logic

#### pygeosolve

<https://github.com/SeanDS/pygeosolve>

A Python-based **geometric constraint solver** using numerical optimization techniques.

**Key Features**

-   Written in Python
-   Uses numerical methods to solve constraints
-   Suitable for prototyping and research
-   Easy to integrate with Python CAD workflows
-   Helpful for understanding constraint-solving fundamentals

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

## 🛠 Specialized CAD Tools

#### OpenVSP

<https://github.com/OpenVSP/OpenVSP>

A parametric aircraft geometry modeling tool developed by NASA.

**Key Features**

-   Aircraft-specific parametric modeling
-   Aerospace-grade geometry
-   Industry & research usage

#### Fritzing

<https://github.com/fritzing/fritzing-app>

An electronics CAD and prototyping tool.

**Key Features**

-   Schematic + PCB + breadboard views
-   Maker-friendly
-   Open hardware ecosystem

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

#### ShapeNet (CAD subset)

<https://github.com/ShapeNet/ShapeNet>

A large 3D shape dataset containing CAD-like models.

**Key Features**

-   Massive scale
-   Mesh-focused
-   Common ML benchmark

#### PartNet

<https://github.com/daerduoCarey/PartNet>

A dataset with hierarchical part-level annotations.

**Key Features**

-   Fine-grained part decomposition
-   Semantic labels
-   Ideal for assembly & reasoning research

#### DeepCAD

<https://github.com/ChrisWu1997/DeepCAD>

A parametric CAD dataset with procedural construction sequences.

**Key Features**

-   Programmatic modeling history
-   Sketch-based operations
-   Ideal for CAD sequence learning

## 📚 CAD Research & Related

#### Awesome-CAD (Research Papers)

[https://github.com/bertjiazheng/Awesome-CAD](https://github.com/bertjiazheng/Awesome-CAD)

A curated list of academic CAD research resources.

**Key Features**

-   CAD geometry processing papers
-   ML on CAD
-   Research-oriented references

## 🤝 Contributing

Contributions are welcome!
