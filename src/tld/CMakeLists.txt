add_library(tld
    Clustering.cpp
    DetectionResult.cpp
    DetectorCascade.cpp
    EnsembleClassifier.cpp
    ForegroundDetector.cpp
    MedianFlowTracker.cpp
    NNClassifier.cpp
    TLD.cpp
    TLDUtil.cpp
    VarianceFilter.cpp)

target_link_libraries(tld cvblobs mftracker ${OpenCV_LIBS})

include_directories(${OpenCV_INCLUDE_DIRS})
