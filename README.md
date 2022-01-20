# DeepI2P(CVPR2021)

[github](https://github.com/lijx10/DeepI2P)

- **Network Architecture**
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled.png)
    
    The final result only use the Frustum Classification.
    
- **Pose Estimation**
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled%201.png)
    
    **For those points with label 1(predicted on the image)**
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled%202.png)
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled%203.png)
    
    **For those points with label 0(prediced not on the image)**
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled%204.png)
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled%205.png)
    
    **Cost Function**
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled%206.png)
    
    Gauss Newton Method to search the optimization.
    
- **Result**
    
    The pose estimation of DeepI2P only use the **Frustum Classification**, which determine if the point can be projected onto the Image.
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled%207.png)
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled%208.png)
    
- **Cross Attention module**
    
    ![Untitled](DeepI2P(CVPR2021)%20e12a5d8b1b874500a80f591eda2ee7ee/Untitled%209.png)
    
- **Something strange about this paper**
    - Only show the **Frustum Classification** result but nothing about that of **Grid Classification.**(In my opinion, it might be very low.)
    - The code calculate the success rate(RRE<5° and RTE<2m), but the paper did not mention it.
    - There is a pre-registration and almost align the image.
