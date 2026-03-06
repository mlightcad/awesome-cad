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

- [🤖 AI-Assisted Design](#-ai-assisted-design)

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

## 🤖 AI-Assisted Design

#### CADAM

<https://github.com/Adam-CAD/CADAM>

An open-source AI-powered text-to-CAD web application that turns natural language and images into parametric 3D models in the browser.

**Key Features**

-   Natural language input to describe 3D models
-   Image-assisted model generation
-   Parametric controls with interactive sliders
-   Real-time 3D preview in browser
-   Export to .STL and .SCAD formats
-   Browser-based with no installation required

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

#### ACadSharp

<https://github.com/DomCR/ACadSharp>

A .NET library for reading, writing, and manipulating DXF and DWG files without requiring AutoCAD.

**Key Features**

-   Native C# / .NET API
-   Read and write DXF (ASCII & binary) and DWG files
-   Strong support for CAD structures (Entities, Blocks, Layers, Tables, Styles)
-   Multi-version DXF/DWG compatibility
-   Fine-grained control over geometry and document data
-   No AutoCAD dependency
-   Open-source (MIT license), suitable for automation and CAD tooling

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

- Solid & surface modeling: robust B-Rep modeling with Booleans, fillets, chamfers, offsets, sweeps, drafts, and advanced construction tools.

- Rich geometric algorithms: point/surface projection, curve/surface intersections, analytical and approximate constructions.

- NURBS & parametric geometry: support for NURBS curves and surfaces, transformations, and analytic primitives (planes, cylinders, cones, spheres, etc.).

- Data interoperability: import/export for STEP, IGES, STL, VRML, BREP plus extended exchange with attributes and assembly (XCAF).

- Shape healing & model repair: tools to correct inconsistencies in imported CAD models.

- Visualization & rendering: interactive 3D display, selection, shading, real-time ray tracing, layered display controls.

- Mesh handling: conversion between exact geometry and tessellated meshes for display and rapid prototyping workflows.

- Application framework: document management (OCAF), undo/redo, attribute tracking, and extensible architecture.

- Modular C++ class libraries designed for rapid development of domain-specific CAD/CAM/CAE applications.

#### pythonOCC

<https://github.com/tpaviot/pythonocc>

Python bindings for OpenCascade.

**Key Features**

-   Rapid CAD prototyping
-   Scriptable B-Rep modeling
-   Research & automation friendly

#### TiGL

<https://github.com/DLR-SC/tigl>

A parametric geometry kernel for aircraft design based on CPACS and OpenCASCADE.

**Key Features**

- Parametric aircraft geometry (wings, fuselages, control surfaces)
- CPACS-driven modeling workflow
- NURBS-based surface generation (built on OCCT)
- Geometry queries (surface points, intersections, sections)
- Export to STEP, IGES, STL, VTK, Collada
- Multi-language bindings (C, C++, Python, Java, MATLAB)
- Includes TiGL Viewer for geometry visualization

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

CAD datasets organized by **representation and supervision type**, covering **mesh-based geometry**, **parametric / B-Rep CAD**, and **language-guided (Text-to-CAD)** datasets.

### 🔺 Mesh-Based CAD / Shape Datasets

Datasets where geometry is represented primarily as **triangle meshes or point clouds**.  
Commonly used in **3D vision**, **shape generation**, and **geometry learning**, but *not* ideal for parametric CAD reconstruction.

#### ShapeNet (CAD subset)

<https://github.com/ShapeNet/ShapeNet>

A massive dataset of 3D shapes, including many CAD-like objects.

**Key Features**

-   Large-scale mesh dataset
-   Category-level annotations
-   Widely used ML benchmark
-   Not parametric or editable CAD

#### PartNet

<https://github.com/daerduoCarey/PartNet>

A structured dataset with hierarchical part annotations built on ShapeNet.

**Key Features**

-   Fine-grained part decomposition
-   Semantic part labels
-   Assembly-aware structure
-   Mesh-based representation

#### Text2Shape

[https://github.com/kchen92/text2shape]()

A dataset pairing natural language descriptions with 3D shapes.

**Key Features**

-   Text ↔ mesh pairs
-   Early benchmark for text-driven 3D generation
-   Useful for multimodal pretraining
-   Not parametric CAD

### 📐 Parametric / B-Rep CAD Datasets

Datasets that represent geometry as **procedural CAD programs**, **feature trees**, or **B-Rep solids**.  
These are critical for **editable CAD**, **design automation**, and **engineering-focused ML**.

#### ABC Dataset (Autodesk)

<https://github.com/AutodeskAILab/abc>

A large-scale dataset of real-world CAD models.

**Key Features**

-   B-Rep + mesh representations
-   Industry-grade CAD geometry
-   High-quality solids
-   Popular benchmark for CAD reconstruction

#### Fusion 360 Gallery Dataset

<https://github.com/AutodeskAILab/Fusion360GalleryDataset>

A dataset of parametric CAD models with full design history.

**Key Features**

-   Feature trees and construction sequences
-   Sketches + operations
-   Ideal for learning parametric modeling
-   Strong foundation for CAD ML research

#### DeepCAD

<https://github.com/ChrisWu1997/DeepCAD>

A parametric CAD dataset with explicit procedural construction sequences.

**Key Features**

-   Programmatic CAD modeling steps
-   Sketch-based operations
-   Clean parametric representation
-   Ideal for sequence learning and CAD synthesis

#### WHUCAD

<https://github.com/fazhihe/WHUCAD>  
Paper: <https://journals.sagepub.com/doi/10.3233/ICA-240744>

A large-scale **feature-level parametric CAD dataset** designed to model advanced CAD operations beyond simple sketch–extrude workflows.

**Key Features**

-   Parametric CAD programs with structured command sequences
-   Includes advanced modeling features
-   Bridges low-level commands and high-level feature representations
-   Suitable for procedural CAD generation and feature learning

### 📝 Text-Guided / Text-to-CAD Datasets

Datasets that **align natural language with CAD models or CAD programs**, enabling research in  
**Text → CAD generation**, **language-guided modeling**, and **multimodal CAD understanding**.

#### Text2CAD Dataset

<https://sadilkhan.github.io/text2cad-project/>

A large-scale dataset explicitly designed for **Text-to-CAD research**, aligning natural language with parametric CAD models.

**Key Features**

-   Natural language ↔ parametric CAD pairs
-   CAD represented as procedural programs
-   Fine-grained design intent annotations
-   Supports Text → CAD and CAD → Text tasks

**Primary Use Cases**

-   Text-to-parametric CAD generation
-   Language-driven CAD editing
-   CAD retrieval from natural language
-   Multimodal representation learning

#### Omni-CAD Dataset

<https://huggingface.co/datasets/jingwei-xu-00/Omni-CAD>

A large-scale **multimodal CAD dataset** designed for unified learning across **geometry, CAD programs, and natural language**.

**Key Features**

-   Multimodal CAD representation (geometry + program + language)
-   Supports **Text ↔ CAD ↔ Geometry** tasks
-   Includes parametric CAD construction sequences
-   Designed for training **foundation models for CAD**
-   Suitable for **CAD generation, understanding, and editing**

**Primary Use Cases**

-   Text-to-CAD generation
-   CAD program synthesis
-   Multimodal CAD representation learning
-   CAD understanding with language supervision

#### ShapeTalk

[https://github.com/ShapeTalk/ShapeTalk]()

A dataset of language grounded in 3D geometry.

**Key Features**

-   Referring expressions for shapes
-   Language grounding in geometry
-   Useful for semantic understanding
-   Often combined with CAD datasets

#### Fusion 360 Gallery + Language (Derived)

<https://github.com/AutodeskAILab/Fusion360GalleryDataset>

While not natively textual, Fusion 360 Gallery is frequently **augmented with synthetic or human-written descriptions** for Text-to-CAD experiments.

**Key Features**

-   Parametric CAD + feature trees
-   Common base dataset for text annotation
-   Used in weakly supervised Text-to-CAD research
-   Bridges classic CAD ML and language models

## 🤝 Contributing

Contributions are welcome!
