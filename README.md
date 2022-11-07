Depth Presentation Attack Detection Dataset
=============

The Depth Presentation Attack Detection Dataset (DPADD) accompanies the following publication: 
*Alexander Tarasov, Anna Denisova and Victor Fedoseev* "Detection of Presentation Attacks on Facial 
Authentication Systems using Intel RealSense Depth Cameras", accepted to [IAS 2022]
(http://www.mirlabs.org/ias22/)

This dataset contains 399 image pairs captured by Intel® RealSense™ D435 for Presentation Attack Detection problem.
Each image pair contains a Depth image and an RGB image. Depth resolution is 1280×720, the data is stored in a 16-bit format in millimeters as a NumPy array. The resolution of RGB data is 1920×1080.

The following parameters vary for different pairs in the dataset:
- distance to a face: 1, 1.5, and 2 m
- the authenticity of a person: a bonafide, a printed photo, and a printed photo cropped along the contour with holes for the eyes
- position of a face relative to the frame center: 9 rectangular sectors dividing the frame area into equal parts
- 5 different people,
- 3 backgrounds.

Data format
-----

Dataset is divided into three folders containing photos captured in three dates. Filenames in the folders are not unique!

File naming format: `{person}\_\{distance}_{in-frame face position}_{background}_{attack type}_{channel}`


- Distance: a - 1 m, b - 1.5 m, c - 2 m.
- In-frame face position: the area is divided into 3 by 3 rectangles marked as 1a, 1b, 1c, 2a, 2b, 2c, 3a, 3b, 3c, where digits are row numbers and letters are column numbers.
- Attack type: a - bonafide, b - printed photo, c - printed photo cropped along the contour with holes for the eyes
- Channel: c - RGB, d - Depth.

Download
-----

Dataset download links:
- Folder 1 (108 image pairs): https://mega.nz/file/zwMlgSRZ#ywe5SwCAaode_7E1zHlUhf2IawItXRS4qr4nnC0KHXQ
- Folder 2  (48 image pairs): https://mega.nz/file/moNRnYwQ#Qrv21hGKDgnJsqiUjCLwtL9aKPmZo3f5v3j64epRvRw
- Folder 3 (243 image pairs): https://mega.nz/file/r49zDCxK#WSAGQhfpPYOZ027oggJ-ygU5p--BNexrKArui-FjKXk

Paper
-----
Paper will be presented at [IAS 2022](http://www.mirlabs.org/ias22/) during December 13-15, 2022.
Now the paper is accepted and its camera-ready copy is submitted to Program Committee.
Main contributor is Alexander Tarasov.

Bibtex:
```
@inproceedings{tarasov22,
  author={Tarasov, Alexander, Denisova, Anna and Fedoseev, Victor},
  title={Detection of Presentation Attacks on Facial Authentication Systems using Intel RealSense Depth Cameras},
  year={2022},
  booktitle={Information assurance and security},
}
```

Use
---
All data is subject to copyright and may only be used for non-commercial research. In case of use please cite our publication.
