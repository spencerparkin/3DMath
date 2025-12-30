# CMakeLists.txt for 3DMath library.

cmake_minimum_required(VERSION 3.27)

project(3DMathLibrary)

set(3DMATH_SOURCES
    Source/AffineTransform.cpp
    Source/AffineTransform.h
    Source/AxisAlignedBox.cpp
    Source/AxisAlignedBox.h
    Source/BoundingBoxTree.cpp
    Source/BoundingBoxTree.h
    Source/BspTree.cpp
    Source/BspTree.h
    Source/Circle.cpp
    Source/Circle.h
    Source/Defines.h
    Source/Exception.cpp
    Source/Exception.h
    Source/FileFormat.cpp
    Source/FileFormat.h
    Source/Function.cpp
    Source/Function.h
    Source/Graph.cpp
    Source/Graph.h
    Source/HandleObject.cpp
    Source/HandleObject.h
    Source/IndexTriangle.cpp
    Source/IndexTriangle.h
    Source/Line.cpp
    Source/Line.h
    Source/LineSegment.cpp
    Source/LineSegment.h
    Source/LinearTransform.cpp
    Source/LinearTransform.h
    Source/ListFunctions.h
    Source/Matrix4x4.cpp
    Source/Matrix4x4.h
    Source/ParticleSystem.cpp
    Source/ParticleSystem.h
    Source/Plane.cpp
    Source/Plane.h
    Source/Polygon.cpp
    Source/Polygon.h
    Source/Random.cpp
    Source/Random.h
    Source/Renderer.cpp
    Source/Renderer.h
    Source/Sphere.cpp
    Source/Sphere.h
    Source/Spline.cpp
    Source/Spline.h
    Source/Surface.cpp
    Source/Surface.h
    Source/TimeKeeper.cpp
    Source/TimeKeeper.h
    Source/Triangle.cpp
    Source/Triangle.h
    Source/TriangleMesh.cpp
    Source/TriangleMesh.h
    Source/Vector.cpp
    Source/Vector.h
    Source/Vertex.cpp
    Source/Vertex.h
)

add_library(3DMathLibrary STATIC ${3DMATH_SOURCES})

target_include_directories(3DMathLibrary PUBLIC Source)