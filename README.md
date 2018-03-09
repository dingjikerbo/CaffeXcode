# CaffeXCode

```
Undefined symbols for architecture x86_64:
  "cv::imread(cv::String const&, int)", referenced from:
```

出现上述信息的原因是cv::imread是在opencv_imgcodecs中定义的，然而这篇博客中并没有加-lopencv_imgcodecs,将它在Linker Flags也加上即可