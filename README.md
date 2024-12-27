# HandwritingRecognition ✍️

An Intelligent system for identifying the writer based on the handwriting patterns and characteristics.

## Overview 🎯
The system analyzes unique writing patterns and characteristics to determine the identity of the writer. Using advanced machine learning techniques, it can recognize individual writing styles and authenticate the author of handwritten text.

## System Architecture 🏗️

```mermaid
graph TD
    A[Input Image] --> B[Preprocessing]
    B --> C[Feature Extraction]
    C --> D[Pattern Analysis]
    D --> E[Writer Identification]
    
    subgraph Preprocessing
        B1[Image Normalization]
        B2[Background Removal]
        B3[Line Segmentation]
        B4[Contour Detection]
        B5[Character Bounding Boxes]
        B6[Character Resizing]
    end
    
    subgraph Feature Extraction
        C1[Stroke Analysis]
        C2[Style Features]
        C3[Pattern Recognition]
    end
    
    subgraph Pattern Analysis
        D1[Compare Features]
        D2[Calculate Similarity]
        D3[Generate Score]
    end
    
    subgraph Writer Identification
        E1[Match Database]
        E2[Confidence Score]
        E3[Final Result]
    end

    B ==> B1
    B1 --> B2
    B2 --> B3 & B4 & B5 & B6
    
    C ==> C1
    C1 ==> C2
    C2 --> C3
    
    D ==> D1
    D1 --> D2
    D2 --> D3
    
    E ==> E1
    E1 --> E2
    E2 --> E3
```
## Features 🌟
- Writer identification from handwritten samples
- Pattern analysis of writing style
- Support for different writing formats
- High accuracy identification

## Requirements 🔧
- Python 3.12
- Required Python packages (install via pip):
  - TensorFlow
  - OpenCV
  - NumPy
  - scikit-learn

## Installation 🛠️
```bash
git clone https://github.com/yourusername/HandwritingRecognition.git
cd HandwritingRecognition
```

## License 📝
This project is licensed under the MIT License.

```
MIT License

Copyright (c) 2024 Tecson Gacrama, Yuanpeng Zhong

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Team 👥
- Co-Developer: Tecson Gacrama
- Co-Developer: Yuanpeng Zhong
