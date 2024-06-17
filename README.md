# Mass on Speed

## Inspiration
Our journey began with a fascination for efficiency and digitalization in computational design. As architects and designers, we cherish the creative freedom of freehand sketching, which allows us to think with our hands. However, collaborative sketching presents significant challenges, particularly in a modern work environment where remote work is becoming increasingly prevalent. This inspired us to create an interactive workflow to bridge the gap between initial hand-drawn drafts and 3D massing and visualization.

We drew inspiration from the project “Hybrid Cocreation” by Viktoria Sandor, Egor Gavrilov, and Serjoscha Düring, which utilized color detection. We aimed to expand this concept to facilitate real-time collaboration in remote settings.

## What We Learned
Throughout this project, we gained insights into integrating traditional sketching methods with modern computational tools. We explored the intricacies of color detection and its application in automating mass generation. Additionally, we learned to manage real-time data processing and remote collaboration, enhancing our skills in both technical and collaborative aspects.

## How We Built the Project

### Generalized Flow
1. **Live Stream Capture**: The design process is captured as a live stream.
2. **Color Detection**: Colors in the live stream are detected and used for generating massing and vegetation.
3. **Geometry Transmission**: The generated geometry is sent to Speckle and retrieved in Unity for real-time rendered walkthroughs.
4. **Buffer Logic**: A buffer logic to take into account the live stream and mass generation through color detection.

### Tools and Technologies
- **Rhino 8 & Grasshopper**: Running in the background for geometry processing.
- **Speckle & Unity**: For transmitting and rendering the geometry in real time.
- **Whiteboard Applications (e.g., Miro)**: For enabling remote collaboration and viewing collaborators' actions.

### Process
1. **Hand Sketching and Colorful Media**: Designers can sketch by hand or use colorful media like playdough.
2. **Remote Collaboration**: The drawing process can be brought online via whiteboard applications. A live screen recording feeds the design process into the color detection algorithm.
3. **Color Mapping**: Different colors are assigned to various elements:
    - Blue: 4-story buildings
    - Red: 3-story buildings
    - Green: Vegetation (trees, either singular or in population)

### Challenges Faced
- **Real-Time Data Processing**: Ensuring smooth and efficient real-time processing without bottlenecks.
- **Buffer Management**: Implementing a buffer logic to handle live stream data and maintain output quality.
- **Remote Collaboration**: Facilitating seamless collaboration in a remote work environment and integrating various tools effectively.

## Conclusion
With Mass on Speed, we aim to accelerate the early stages of urban design by integrating the tangible dimension of hand sketching with advanced computational tools. Our workflow not only enhances efficiency but also brings back the tactile experience as a valuable method of collaboration in the digital age.

## Requirements
- **Unity**: Our version was 2022.1.23f1
- **Rhino 8**: Ensure you are using the latest version of Rhino.
- **Plugins**: Install the following plugins:
  - Javid
  - Euglena
  - Bitmap+


For more details on how to utilize Unity for Speckle, please check out [Speckle Unity's official GitHub page](https://github.com/specklesystems/speckle-unity/blob/main/README.md).
