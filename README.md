# 3D-KEN-BURNS-EFFECT 

### ABOUT
The Ken Burns effect allows animating still images with a virtual camera scan and zoom. Adding parallax, which results in the 3D Ken Burns effect, enables significantly more compelling results. Creating such effects manually is time-consuming and demands sophisticated editing skills. Existing automatic methods, however, require multiple input images from varying viewpoints. In this paper, we introduce a framework that synthesizes the 3D Ken Burns effect from a single image, supporting both a fully automatic mode and an interactive mode with the user controlling the camera. Our framework first leverages a depth prediction pipeline, which estimates scene depth that is suitable for view synthesis tasks. To address the limitations of existing depth estimation methods such as geometric distortions, semantic distortions, and inaccurate depth boundaries, we develop a semantic-aware neural network for depth prediction, couple its estimate with a segmentation-based depth adjustment process, and employ a refinement neural network that facilitates accurate depth predictions at object boundaries. According to this depth estimate, our framework then maps the input image to a point cloud and synthesizes the resulting video frames by rendering the point cloud from the corresponding camera positions. To address disocclusions while maintaining geometrically and temporally coherent synthesis results, we utilize context-aware color- and depth-inpainting to fill in the missing information in the extreme views of the camera path, thus extending the scene geometry of the point cloud. Experiments with a wide variety of image content show that our method enables realistic synthesis results. Our study demonstrates that our system allows users to achieve better results while requiring little effort compared to existing solutions for the 3D Ken Burns effect creation.



## Idead Behind

Once Again , on my search for art for my room. I came accross this project which allows me to convert 2d images into a short 3d video with depth perception. The depth prediction combined with segmentation based depth adjustance alows us to create beautiful 3D videos.





NORMAL IMAGE               |  3D KEN BURN EFFECT
:-------------------------:|:-------------------------:
![](https://github.com/Yega-Noragami/3D-KEN-BURNS/blob/main/test_images/skm.png)|  ![](https://github.com/Yega-Noragami/3D-KEN-BURNS/blob/main/results/skm.gif)





