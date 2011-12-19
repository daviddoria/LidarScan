ENABLE_TESTING()

ADD_EXECUTABLE(TestScan TestScan.cpp)
TARGET_LINK_LIBRARIES(TestScan MyLibs boost_program_options-mt)
ADD_TEST(TestScan TestScan)

############################################
ADD_EXECUTABLE(TestScanner TestScanner.cpp)
TARGET_LINK_LIBRARIES(TestScanner MyLibs)
ADD_TEST(TestScan TestScan)

############################################
ADD_EXECUTABLE(TestStrip TestStrip.cpp)
TARGET_LINK_LIBRARIES(TestStrip MyLibs)
ADD_TEST(TestStrip TestStrip)

###########################################
ADD_EXECUTABLE(TestPoint TestPoint.cpp)
TARGET_LINK_LIBRARIES(TestPoint MyLibs)
ADD_TEST(TestPoint TestPoint)

###########################################
ADD_EXECUTABLE(TestScanImage TestScanImage.cpp)
TARGET_LINK_LIBRARIES(TestScanImage MyLibs)
ADD_TEST(TestScanImage TestScanImage)
