# Point Cloud Renderer

![mitsuba rendering](mitsuba_rendering.png)

This Python script allows you to convert your point cloud data into beautifully rendered 3D images using Mitsuba.

- The script creates a XML file describes a 3D scene in the format used by the Mitsuba renderer. 
- Then proceeds to render this scene and save the result as a PNG file. 
- If your data tensor contains multiple point clouds, the script will iterate over them and produce multiple renderings.

Currently, the script supports both `.ply` and `.npy` file formats.

This project is inspired by the amazing work done at [Point Flow Renderer](https://github.com/zekunhao1995/PointFlowRenderer). 

Everyone is welcome to use Point Cloud Renderer. 
If you have any enhancements or fixes, I encourage you to make a pull request.

## Dependencies

### Pre-requisites:
- **Python**: Version 3.8 or newer. You can download it from the [official website](https://www.python.org/downloads/).

### Installing Dependencies:
All the Python dependencies required for this project are listed in the requirements.txt file. To install them, navigate to the directory containing requirements.txt and run:

```bash
pip install -r requirements.txt
```
This will install the following Python packages:

- **NumPy**: A fundamental package for scientific computing with Python.
- **Plyfile**: A Python module for reading and writing PLY files.
- **Mitsuba 3**: A research-oriented rendering system. The script is tailored for Mitsuba 3. For more details or troubleshooting, visit the [official Mitsuba website](http://www.mitsuba-renderer.org).

Ensure you've set up all these dependencies correctly before running the script.

## Instructions

To use the script and render your point cloud data, simply run:
```bash
python point_cloud_renderer.py <path_to_your_file>
```

For example:

```bash
python point_cloud_renderer.py chair.npy
```

The output PNG file will be saved in the same directory as your input file.
