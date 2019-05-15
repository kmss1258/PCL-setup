# Point Cloud Library (PCL) Setup method (VS 2015, PCL 1.8.1)
Using All-In-One Installer (.exe)

File Link : https://github.com/PointCloudLibrary/pcl/releases/download/pcl-1.8.1/PCL-1.8.1-AllInOne-msvc2015-win64.exe
> PCL 1.8.1, Boost 1.64.0, Eigen 3.3.4, FLANN 1.9.1, VTK 8.0.0 (OpenGL backend), QHull 2015.2, OpenNI 2.2.0.33 Beta

# PCL 설치
ㅁㄴㅇ

# PCL 라이브러리 세팅
아래의 세팅은 Debugging Mode 기준. Release로 실행하고 싶다면 include files을 제외하고 library는 **d, gd...** 등이 붙지 않은 것을 추가하면 됨

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

# 동작

Result Image
------
C:\Program Files\PCL 1.8.1\share\doc\pcl-1.8\tutorials\sources\pcl_visualizer 의 경로에 있는 샘플 코드를 사용    
제어는 마우스로 가능하며, 왼쪽 버튼은 Point Cloud의 이동을, 오른쪽 버튼과 마우스 휠로는 Point Cloud와의 시야 거리를 조정    
아래는 argv로 -c 인자를 주어 실행한 결과


Sample Code
-----
main.cpp

```
/* \author Geoffrey Biggs */


#include <iostream>

#include <boost/thread/thread.hpp>
#include <pcl/common/common_headers.h>
#include <pcl/features/normal_3d.h>
#include <pcl/io/pcd_io.h>
#include <pcl/visualization/pcl_visualizer.h>
#include <pcl/console/parse.h>

// --------------
// -----Help-----
// --------------
void printUsage(const char* progName)
{
	std::cout << "\n\nUsage: " << progName << " [options]\n\n"
		<< "Options:\n"
		<< "-------------------------------------------\n"
		<< "-h           this help\n"
		<< "-s           Simple visualisation example\n"
		<< "-r           RGB colour visualisation example\n"
		<< "-c           Custom colour visualisation example\n"
		<< "-n           Normals visualisation example\n"
		<< "-a           Shapes visualisation example\n"
		<< "-v           Viewports example\n"
		<< "-i           Interaction Customization example\n"
		<< "\n\n";
}


boost::shared_ptr<pcl::visualization::PCLVisualizer> simpleVis(pcl::PointCloud<pcl::PointXYZ>::ConstPtr cloud)
{
	// --------------------------------------------
	// -----Open 3D viewer and add point cloud-----
	// --------------------------------------------
	boost::shared_ptr<pcl::visualization::PCLVisualizer> viewer(new pcl::visualization::PCLVisualizer("3D Viewer"));
	viewer->setBackgroundColor(0, 0, 0);
	viewer->addPointCloud<pcl::PointXYZ>(cloud, "sample cloud");
	viewer->setPointCloudRenderingProperties(pcl::visualization::PCL_VISUALIZER_POINT_SIZE, 1, "sample cloud");
	viewer->addCoordinateSystem(1.0);
	viewer->initCameraParameters();
	return (viewer);
}


boost::shared_ptr<pcl::visualization::PCLVisualizer> rgbVis(pcl::PointCloud<pcl::PointXYZRGB>::ConstPtr cloud)
{
	// --------------------------------------------
	// -----Open 3D viewer and add point cloud-----
	// --------------------------------------------
	boost::shared_ptr<pcl::visualization::PCLVisualizer> viewer(new pcl::visualization::PCLVisualizer("3D Viewer"));
	viewer->setBackgroundColor(0, 0, 0);
	pcl::visualization::PointCloudColorHandlerRGBField<pcl::PointXYZRGB> rgb(cloud);
	viewer->addPointCloud<pcl::PointXYZRGB>(cloud, rgb, "sample cloud");
	viewer->setPointCloudRenderingProperties(pcl::visualization::PCL_VISUALIZER_POINT_SIZE, 3, "sample cloud");
	viewer->addCoordinateSystem(1.0);
	viewer->initCameraParameters();
	return (viewer);
}


boost::shared_ptr<pcl::visualization::PCLVisualizer> customColourVis(pcl::PointCloud<pcl::PointXYZ>::ConstPtr cloud)
{
	// --------------------------------------------
	// -----Open 3D viewer and add point cloud-----
	// --------------------------------------------
	boost::shared_ptr<pcl::visualization::PCLVisualizer> viewer(new pcl::visualization::PCLVisualizer("3D Viewer"));
	viewer->setBackgroundColor(0, 0, 0);
	pcl::visualization::PointCloudColorHandlerCustom<pcl::PointXYZ> single_color(cloud, 0, 255, 0);
	viewer->addPointCloud<pcl::PointXYZ>(cloud, single_color, "sample cloud");
	viewer->setPointCloudRenderingProperties(pcl::visualization::PCL_VISUALIZER_POINT_SIZE, 3, "sample cloud");
	viewer->addCoordinateSystem(1.0);
	viewer->initCameraParameters();
	return (viewer);
}


boost::shared_ptr<pcl::visualization::PCLVisualizer> normalsVis(
	pcl::PointCloud<pcl::PointXYZRGB>::ConstPtr cloud, pcl::PointCloud<pcl::Normal>::ConstPtr normals)
{
	// --------------------------------------------------------
	// -----Open 3D viewer and add point cloud and normals-----
	// --------------------------------------------------------
	boost::shared_ptr<pcl::visualization::PCLVisualizer> viewer(new pcl::visualization::PCLVisualizer("3D Viewer"));
	viewer->setBackgroundColor(0, 0, 0);
	pcl::visualization::PointCloudColorHandlerRGBField<pcl::PointXYZRGB> rgb(cloud);
	viewer->addPointCloud<pcl::PointXYZRGB>(cloud, rgb, "sample cloud");
	viewer->setPointCloudRenderingProperties(pcl::visualization::PCL_VISUALIZER_POINT_SIZE, 3, "sample cloud");
	viewer->addPointCloudNormals<pcl::PointXYZRGB, pcl::Normal>(cloud, normals, 10, 0.05, "normals");
	viewer->addCoordinateSystem(1.0);
	viewer->initCameraParameters();
	return (viewer);
}


boost::shared_ptr<pcl::visualization::PCLVisualizer> shapesVis(pcl::PointCloud<pcl::PointXYZRGB>::ConstPtr cloud)
{
	// --------------------------------------------
	// -----Open 3D viewer and add point cloud-----
	// --------------------------------------------
	boost::shared_ptr<pcl::visualization::PCLVisualizer> viewer(new pcl::visualization::PCLVisualizer("3D Viewer"));
	viewer->setBackgroundColor(0, 0, 0);
	pcl::visualization::PointCloudColorHandlerRGBField<pcl::PointXYZRGB> rgb(cloud);
	viewer->addPointCloud<pcl::PointXYZRGB>(cloud, rgb, "sample cloud");
	viewer->setPointCloudRenderingProperties(pcl::visualization::PCL_VISUALIZER_POINT_SIZE, 3, "sample cloud");
	viewer->addCoordinateSystem(1.0);
	viewer->initCameraParameters();

	//------------------------------------
	//-----Add shapes at cloud points-----
	//------------------------------------
	viewer->addLine<pcl::PointXYZRGB>(cloud->points[0],
		cloud->points[cloud->size() - 1], "line");
	viewer->addSphere(cloud->points[0], 0.2, 0.5, 0.5, 0.0, "sphere");

	//---------------------------------------
	//-----Add shapes at other locations-----
	//---------------------------------------
	pcl::ModelCoefficients coeffs;
	coeffs.values.push_back(0.0);
	coeffs.values.push_back(0.0);
	coeffs.values.push_back(1.0);
	coeffs.values.push_back(0.0);
	viewer->addPlane(coeffs, "plane");
	coeffs.values.clear();
	coeffs.values.push_back(0.3);
	coeffs.values.push_back(0.3);
	coeffs.values.push_back(0.0);
	coeffs.values.push_back(0.0);
	coeffs.values.push_back(1.0);
	coeffs.values.push_back(0.0);
	coeffs.values.push_back(5.0);
	viewer->addCone(coeffs, "cone");

	return (viewer);
}


boost::shared_ptr<pcl::visualization::PCLVisualizer> viewportsVis(
	pcl::PointCloud<pcl::PointXYZRGB>::ConstPtr cloud, pcl::PointCloud<pcl::Normal>::ConstPtr normals1, pcl::PointCloud<pcl::Normal>::ConstPtr normals2)
{
	// --------------------------------------------------------
	// -----Open 3D viewer and add point cloud and normals-----
	// --------------------------------------------------------
	boost::shared_ptr<pcl::visualization::PCLVisualizer> viewer(new pcl::visualization::PCLVisualizer("3D Viewer"));
	viewer->initCameraParameters();

	int v1(0);
	viewer->createViewPort(0.0, 0.0, 0.5, 1.0, v1);
	viewer->setBackgroundColor(0, 0, 0, v1);
	viewer->addText("Radius: 0.01", 10, 10, "v1 text", v1);
	pcl::visualization::PointCloudColorHandlerRGBField<pcl::PointXYZRGB> rgb(cloud);
	viewer->addPointCloud<pcl::PointXYZRGB>(cloud, rgb, "sample cloud1", v1);

	int v2(0);
	viewer->createViewPort(0.5, 0.0, 1.0, 1.0, v2);
	viewer->setBackgroundColor(0.3, 0.3, 0.3, v2);
	viewer->addText("Radius: 0.1", 10, 10, "v2 text", v2);
	pcl::visualization::PointCloudColorHandlerCustom<pcl::PointXYZRGB> single_color(cloud, 0, 255, 0);
	viewer->addPointCloud<pcl::PointXYZRGB>(cloud, single_color, "sample cloud2", v2);

	viewer->setPointCloudRenderingProperties(pcl::visualization::PCL_VISUALIZER_POINT_SIZE, 3, "sample cloud1");
	viewer->setPointCloudRenderingProperties(pcl::visualization::PCL_VISUALIZER_POINT_SIZE, 3, "sample cloud2");
	viewer->addCoordinateSystem(1.0);

	viewer->addPointCloudNormals<pcl::PointXYZRGB, pcl::Normal>(cloud, normals1, 10, 0.05, "normals1", v1);
	viewer->addPointCloudNormals<pcl::PointXYZRGB, pcl::Normal>(cloud, normals2, 10, 0.05, "normals2", v2);

	return (viewer);
}


unsigned int text_id = 0;
void keyboardEventOccurred(const pcl::visualization::KeyboardEvent &event,
	void* viewer_void)
{
	pcl::visualization::PCLVisualizer *viewer = static_cast<pcl::visualization::PCLVisualizer *> (viewer_void);
	if (event.getKeySym() == "r" && event.keyDown())
	{
		std::cout << "r was pressed => removing all text" << std::endl;

		char str[512];
		for (unsigned int i = 0; i < text_id; ++i)
		{
			sprintf(str, "text#%03d", i);
			viewer->removeShape(str);
		}
		text_id = 0;
	}
}

void mouseEventOccurred(const pcl::visualization::MouseEvent &event,
	void* viewer_void)
{
	pcl::visualization::PCLVisualizer *viewer = static_cast<pcl::visualization::PCLVisualizer *> (viewer_void);
	if (event.getButton() == pcl::visualization::MouseEvent::LeftButton &&
		event.getType() == pcl::visualization::MouseEvent::MouseButtonRelease)
	{
		std::cout << "Left mouse button released at position (" << event.getX() << ", " << event.getY() << ")" << std::endl;

		char str[512];
		sprintf(str, "text#%03d", text_id++);
		viewer->addText("clicked here", event.getX(), event.getY(), str);
	}
}

boost::shared_ptr<pcl::visualization::PCLVisualizer> interactionCustomizationVis()
{
	boost::shared_ptr<pcl::visualization::PCLVisualizer> viewer(new pcl::visualization::PCLVisualizer("3D Viewer"));
	viewer->setBackgroundColor(0, 0, 0);
	viewer->addCoordinateSystem(1.0);

	viewer->registerKeyboardCallback(keyboardEventOccurred, (void*)viewer.get());
	viewer->registerMouseCallback(mouseEventOccurred, (void*)viewer.get());

	return (viewer);
}


// --------------
// -----Main-----
// --------------
int
main(int argc, char** argv)
{
	// --------------------------------------
	// -----Parse Command Line Arguments-----
	// --------------------------------------
	if (pcl::console::find_argument(argc, argv, "-h") >= 0)
	{
		printUsage(argv[0]);
		return 0;
	}
	bool simple(false), rgb(false), custom_c(false), normals(false),
		shapes(false), viewports(false), interaction_customization(false);
	if (pcl::console::find_argument(argc, argv, "-s") >= 0)
	{
		simple = true;
		std::cout << "Simple visualisation example\n";
	}
	else if (pcl::console::find_argument(argc, argv, "-c") >= 0)
	{
		custom_c = true;
		std::cout << "Custom colour visualisation example\n";
	}
	else if (pcl::console::find_argument(argc, argv, "-r") >= 0)
	{
		rgb = true;
		std::cout << "RGB colour visualisation example\n";
	}
	else if (pcl::console::find_argument(argc, argv, "-n") >= 0)
	{
		normals = true;
		std::cout << "Normals visualisation example\n";
	}
	else if (pcl::console::find_argument(argc, argv, "-a") >= 0)
	{
		shapes = true;
		std::cout << "Shapes visualisation example\n";
	}
	else if (pcl::console::find_argument(argc, argv, "-v") >= 0)
	{
		viewports = true;
		std::cout << "Viewports example\n";
	}
	else if (pcl::console::find_argument(argc, argv, "-i") >= 0)
	{
		interaction_customization = true;
		std::cout << "Interaction Customization example\n";
	}
	else
	{
		printUsage(argv[0]);
		return 0;
	}

	// ------------------------------------
	// -----Create example point cloud-----
	// ------------------------------------
	pcl::PointCloud<pcl::PointXYZ>::Ptr basic_cloud_ptr(new pcl::PointCloud<pcl::PointXYZ>);
	pcl::PointCloud<pcl::PointXYZRGB>::Ptr point_cloud_ptr(new pcl::PointCloud<pcl::PointXYZRGB>);
	std::cout << "Genarating example point clouds.\n\n";
	// We're going to make an ellipse extruded along the z-axis. The colour for
	// the XYZRGB cloud will gradually go from red to green to blue.
	uint8_t r(255), g(15), b(15);
	for (float z(-1.0); z <= 1.0; z += 0.05)
	{
		for (float angle(0.0); angle <= 360.0; angle += 5.0)
		{
			pcl::PointXYZ basic_point;
			basic_point.x = 0.5 * cosf(pcl::deg2rad(angle));
			basic_point.y = sinf(pcl::deg2rad(angle));
			basic_point.z = z;
			basic_cloud_ptr->points.push_back(basic_point);

			pcl::PointXYZRGB point;
			point.x = basic_point.x;
			point.y = basic_point.y;
			point.z = basic_point.z;
			uint32_t rgb = (static_cast<uint32_t>(r) << 16 |
				static_cast<uint32_t>(g) << 8 | static_cast<uint32_t>(b));
			point.rgb = *reinterpret_cast<float*>(&rgb);
			point_cloud_ptr->points.push_back(point);
		}
		if (z < 0.0)
		{
			r -= 12;
			g += 12;
		}
		else
		{
			g -= 12;
			b += 12;
		}
	}
	basic_cloud_ptr->width = (int)basic_cloud_ptr->points.size();
	basic_cloud_ptr->height = 1;
	point_cloud_ptr->width = (int)point_cloud_ptr->points.size();
	point_cloud_ptr->height = 1;

	// ----------------------------------------------------------------
	// -----Calculate surface normals with a search radius of 0.05-----
	// ----------------------------------------------------------------
	pcl::NormalEstimation<pcl::PointXYZRGB, pcl::Normal> ne;
	ne.setInputCloud(point_cloud_ptr);
	pcl::search::KdTree<pcl::PointXYZRGB>::Ptr tree(new pcl::search::KdTree<pcl::PointXYZRGB>());
	ne.setSearchMethod(tree);
	pcl::PointCloud<pcl::Normal>::Ptr cloud_normals1(new pcl::PointCloud<pcl::Normal>);
	ne.setRadiusSearch(0.05);
	ne.compute(*cloud_normals1);

	// ---------------------------------------------------------------
	// -----Calculate surface normals with a search radius of 0.1-----
	// ---------------------------------------------------------------
	pcl::PointCloud<pcl::Normal>::Ptr cloud_normals2(new pcl::PointCloud<pcl::Normal>);
	ne.setRadiusSearch(0.1);
	ne.compute(*cloud_normals2);

	boost::shared_ptr<pcl::visualization::PCLVisualizer> viewer;
	if (simple)
	{
		viewer = simpleVis(basic_cloud_ptr);
	}
	else if (rgb)
	{
		viewer = rgbVis(point_cloud_ptr);
	}
	else if (custom_c)
	{
		viewer = customColourVis(basic_cloud_ptr);
	}
	else if (normals)
	{
		viewer = normalsVis(point_cloud_ptr, cloud_normals2);
	}
	else if (shapes)
	{
		viewer = shapesVis(point_cloud_ptr);
	}
	else if (viewports)
	{
		viewer = viewportsVis(point_cloud_ptr, cloud_normals1, cloud_normals2);
	}
	else if (interaction_customization)
	{
		viewer = interactionCustomizationVis();
	}

	//--------------------
	// -----Main loop-----
	//--------------------
	while (!viewer->wasStopped())
	{
		viewer->spinOnce(100);
		boost::this_thread::sleep(boost::posix_time::microseconds(100000));
	}
}

```


# 오류 디버깅 (Debugging)

Warning! PATH too long installer unable to modify PATH!
-----
PCL 설치 도중, 환경변수를 모든 유저들에게 등록 한다는 탭을 클릭하였을 때 간헐적으로 일어나는 오류 
임의로 PCL에 대한 환경변수를 위와 같이 설정해주면 된다. 

vcomp140d.dll에 오류가 있거나...
--------
System32 폴더에 있는 openMP 라이브러리가 손상되었을 경우 나타나는 현상일 가능성이 큼.
다른 컴퓨터에서 해당 파일을 검색하여 다운로드 하는 것을 추천.

