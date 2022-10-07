```python
import os
import imageio


png_dir = '../gif圖製做/分佈圖_縮小'
images = []
for file_name in os.listdir(png_dir):
    if file_name.endswith('.jpg'):
        file_path = os.path.join(png_dir, file_name)
        images.append(imageio.imread(file_path))
imageio.mimsave('../gif圖製做/分佈圖_縮小/test.gif', images,fps=0.8)
```
