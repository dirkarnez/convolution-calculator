[convolution-calculator](https://dirkarnez.github.io/convolution-calculator/)
===================================================================================
- [numpy.convolve — NumPy v1.26 Manual](https://numpy.org/doc/stable/reference/generated/numpy.convolve.html)
- [But what is a convolution? - YouTube](https://www.youtube.com/watch?v=KuXjwB4LzSA)
- [numpy中的convolve的理解_np.convolve-CSDN博客](https://blog.csdn.net/u011599639/article/details/76254442)

### TODOs
- [ ] 2D Convolution
  - [Example of 2D Convolution](https://www.songho.ca/dsp/convolution/convolution2d_example.html)
  - [Example of 2D Convolution](https://www.songho.ca/dsp/convolution/convolution2d_example.html)
  - [Proof of Separable Convolution 2D](https://www.songho.ca/dsp/convolution/convolution2d_separable.html)
  - [Proof of Commutative Property of Convolution](https://www.songho.ca/dsp/convolution/convolution_commutative.html)
  - ```python
    import numpy as np
    from scipy.signal import convolve2d
    
    # Example image (5x5)
    image = np.array([[1, 2, 3, 0, 1],
                      [4, 5, 6, 1, 0],
                      [7, 8, 9, 0, 1],
                      [0, 1, 2, 3, 4],
                      [1, 0, 1, 0, 5]])
    
    # Example kernel (3x3)
    kernel = np.array([[1, 0, -1],
                       [1, 0, -1],
                       [1, 0, -1]])
    
    # Perform convolution
    result = convolve2d(image, kernel, mode='valid')
    print(result)
    ```
