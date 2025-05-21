cmake_minimum_required(VERSION 3.11)

project(utils)

include_directories(
    ../include
)

add_executable(text-scroller text-scroller.cc)

target_link_libraries(text-scroller
PRIVATE rgbmatrix
) 

# add_executable(led-image-viewer led-image-viewer.cc)

# target_link_libraries(led-image-viewer
# PRIVATE rgbmatrix
# ) 

# add_executable(video-viewer video-viewer.cc)

# target_link_libraries(video-viewer
# PRIVATE rgbmatrix
# ) 



# text-scroller: text-scroller.o $(RGB_LIBRARY)
# 	$(CXX) $(CXXFLAGS) text-scroller.o -o $@ $(LDFLAGS) $(RGB_LDFLAGS)

# led-image-viewer: led-image-viewer.o $(RGB_LIBRARY)
# 	$(CXX) $(CXXFLAGS) led-image-viewer.o -o $@ $(LDFLAGS) $(RGB_LDFLAGS) $(MAGICK_LDFLAGS)

# video-viewer: video-viewer.o $(RGB_LIBRARY)
# 	$(CXX) $(CXXFLAGS) video-viewer.o -o $@ $(LDFLAGS) $(RGB_LDFLAGS) $(AV_LDFLAGS)

# %.o : %.cc
# 	$(CXX) -I$(RGB_INCDIR) $(CXXFLAGS) -c -o $@ $<

# led-image-viewer.o : led-image-viewer.cc
# 	$(CXX) -I$(RGB_INCDIR) $(CXXFLAGS) $(MAGICK_CXXFLAGS) -c -o $@ $<