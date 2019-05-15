# Point Cloud Library (PCL) Setup method (VS 2015, PCL 1.8.1)
Using All-In-One Installer (.exe)

File Link : https://github.com/PointCloudLibrary/pcl/releases/download/pcl-1.8.1/PCL-1.8.1-AllInOne-msvc2015-win64.exe
> PCL 1.8.1, Boost 1.64.0, Eigen 3.3.4, FLANN 1.9.1, VTK 8.0.0 (OpenGL backend), QHull 2015.2, OpenNI 2.2.0.33 Beta

# PCL 설치


# PCL 라이브러리 세팅

추가 포함 디렉터리 (adding include files)
-------
속성 - C/C++ - 일반 - 추가 포함 디렉터리

```
C:\Program Files\PCL 1.8.1\include\pcl-1.8
C:\Program Files\PCL 1.8.1\3rdParty\Boost\include\boost-1_64
C:\Program Files\PCL 1.8.1\3rdParty\Eigen\eigen3
C:\Program Files\PCL 1.8.1\3rdParty\FLANN\include
C:\Program Files\PCL 1.8.1\3rdParty\VTK\include\vtk-8.0
C:\Program Files\PCL 1.8.1\3rdParty\Qhull\include
```

라이브러리 추가 (adding .lib files)
-------
속성 - 링커 - 추가 라이브러리 디렉터리

```
C:\Program Files\PCL 1.8.1\lib
C:\Program Files\OpenNI2\Lib
C:\Program Files\PCL 1.8.1\3rdParty\VTK\lib
C:\Program Files\PCL 1.8.1\3rdParty\Boost\lib
C:\Program Files\PCL 1.8.1\3rdParty\Qhull\lib
C:\Program Files\PCL 1.8.1\3rdParty\FLANN\lib
```

속성 - 링커 - 입력 - 추가 종속성

```
pcl_common_debug.lib
pcl_features_debug.lib
pcl_filters_debug.lib
pcl_io_debug.lib
pcl_kdtree_debug.lib
pcl_keypoints_debug.lib
pcl_octree_debug.lib
pcl_registration_debug.lib
pcl_sample_consensus_debug.lib
pcl_search_debug.lib
pcl_segmentation_debug.lib
pcl_surface_debug.lib
pcl_tracking_debug.lib
pcl_visualization_debug.lib
OpenNI2.lib
vtkalglib-8.0-gd.lib
vtkChartsCore-8.0-gd.lib
vtkCommonColor-8.0-gd.lib
vtkCommonComputationalGeometry-8.0-gd.lib
vtkCommonCore-8.0-gd.lib
vtkCommonDataModel-8.0-gd.lib
vtkCommonExecutionModel-8.0-gd.lib
vtkCommonMath-8.0-gd.lib
vtkCommonMisc-8.0-gd.lib
vtkCommonSystem-8.0-gd.lib
vtkCommonTransforms-8.0-gd.lib
vtkDomainsChemistry-8.0-gd.lib
vtkexoIIc-8.0-gd.lib
vtkexpat-8.0-gd.lib
vtkFiltersAMR-8.0-gd.lib
vtkFiltersCore-8.0-gd.lib
vtkFiltersExtraction-8.0-gd.lib
vtkFiltersFlowPaths-8.0-gd.lib
vtkFiltersGeneral-8.0-gd.lib
vtkFiltersGeneric-8.0-gd.lib
vtkFiltersGeometry-8.0-gd.lib
vtkFiltersHybrid-8.0-gd.lib
vtkFiltersHyperTree-8.0-gd.lib
vtkFiltersImaging-8.0-gd.lib
vtkFiltersModeling-8.0-gd.lib
vtkFiltersParallel-8.0-gd.lib
vtkFiltersParallelImaging-8.0-gd.lib
vtkFiltersPoints-8.0-gd.lib
vtkFiltersProgrammable-8.0-gd.lib
vtkFiltersSelection-8.0-gd.lib
vtkFiltersSMP-8.0-gd.lib
vtkFiltersSources-8.0-gd.lib
vtkFiltersStatistics-8.0-gd.lib
vtkFiltersTexture-8.0-gd.lib
vtkFiltersTopology-8.0-gd.lib
vtkFiltersVerdict-8.0-gd.lib
vtkfreetype-8.0-gd.lib
vtkGeovisCore-8.0-gd.lib
vtkgl2ps-8.0-gd.lib
vtkhdf5_hl-8.0-gd.lib
vtkhdf5-8.0-gd.lib
vtkImagingColor-8.0-gd.lib
vtkImagingCore-8.0-gd.lib
vtkImagingFourier-8.0-gd.lib
vtkImagingGeneral-8.0-gd.lib
vtkImagingHybrid-8.0-gd.lib
vtkImagingMath-8.0-gd.lib
vtkImagingMorphological-8.0-gd.lib
vtkImagingSources-8.0-gd.lib
vtkImagingStatistics-8.0-gd.lib
vtkImagingStencil-8.0-gd.lib
vtkInfovisCore-8.0-gd.lib
vtkInfovisLayout-8.0-gd.lib
vtkInteractionImage-8.0-gd.lib
vtkInteractionStyle-8.0-gd.lib
vtkInteractionWidgets-8.0-gd.lib
vtkIOAMR-8.0-gd.lib
vtkIOCore-8.0-gd.lib
vtkIOEnSight-8.0-gd.lib
vtkIOExodus-8.0-gd.lib
vtkIOExport-8.0-gd.lib
vtkIOExportOpenGL-8.0-gd.lib
vtkIOGeometry-8.0-gd.lib
vtkIOImage-8.0-gd.lib
vtkIOImport-8.0-gd.lib
vtkIOInfovis-8.0-gd.lib
vtkIOLegacy-8.0-gd.lib
vtkIOLSDyna-8.0-gd.lib
vtkIOMINC-8.0-gd.lib
vtkIOMovie-8.0-gd.lib
vtkIONetCDF-8.0-gd.lib
vtkIOParallel-8.0-gd.lib
vtkIOParallelXML-8.0-gd.lib
vtkIOPLY-8.0-gd.lib
vtkIOSQL-8.0-gd.lib
vtkIOTecplotTable-8.0-gd.lib
vtkIOVideo-8.0-gd.lib
vtkIOXML-8.0-gd.lib
vtkIOXMLParser-8.0-gd.lib
vtkjpeg-8.0-gd.lib
vtkjsoncpp-8.0-gd.lib
vtklibharu-8.0-gd.lib
vtklibxml2-8.0-gd.lib
vtklz4-8.0-gd.lib
vtkmetaio-8.0-gd.lib
vtknetcdf_c++-gd.lib
vtkNetCDF-8.0-gd.lib
vtkoggtheora-8.0-gd.lib
vtkParallelCore-8.0-gd.lib
vtkpng-8.0-gd.lib
vtkproj4-8.0-gd.lib
vtkRenderingAnnotation-8.0-gd.lib
vtkRenderingContext2D-8.0-gd.lib
vtkRenderingContextOpenGL-8.0-gd.lib
vtkRenderingCore-8.0-gd.lib
vtkRenderingFreeType-8.0-gd.lib
vtkRenderingGL2PS-8.0-gd.lib
vtkRenderingImage-8.0-gd.lib
vtkRenderingLabel-8.0-gd.lib
vtkRenderingLIC-8.0-gd.lib
vtkRenderingLOD-8.0-gd.lib
vtkRenderingOpenGL-8.0-gd.lib
vtkRenderingVolume-8.0-gd.lib
vtkRenderingVolumeOpenGL-8.0-gd.lib
vtksqlite-8.0-gd.lib
vtksys-8.0-gd.lib
vtktiff-8.0-gd.lib
vtkverdict-8.0-gd.lib
vtkViewsContext2D-8.0-gd.lib
vtkViewsCore-8.0-gd.lib
vtkzlib-8.0-gd.lib
```

동적 라이브러리 추가 (adding DLL files)
-----
시작 - (검색) 시스템 환경 변수 편집 - 환경 변수 - 시스템 변수 - Path 탭 클릭 - 편집 - 새로 만들기

```
C:\Program Files\PCL 1.8.1\bin
```

