# OklahomaAI-CLI
XCode project to classify Deer vs No Deer on trailcam images. Using apple Create ML and Swift

Run with:

./OklahomaAI-CLI /path/to/Images

[!NOTE] Currently, image path MUST be an absolute path

[!NOTE] Image dir processing is not recursive

[!NOTE] Images in the target folder MUST be named *.JPG (case sensitive)


Output will be a file named "" in the Images dir, with this content:

``
[
  {
    "image" : "TOP_2023-12-02T223600_PICT3710_202312030600W4DUH.JPG",
    "classification" : "1.Deer",
    "confidence" : 0.9940010392107557
  },
  {
    "classification" : "1.Deer",
    "confidence" : 0.9999842919078755,
    "image" : "TOP_2023-12-02T221000_PICT3705_202312030600JGVXF.JPG"
  },
  ...
]
```
