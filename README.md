# tlc_plate_analyser and rf calculator
Digitise thin layer chromatography plactes and automatically measures the rf values of tlc plates
Rf_calculator.ipynb ©Michelle Chong, April 2021, Release 1.0
*Code written for university project*

Dependencies: numpy v1.18.5, matplotlib	v3.2.2, opencv/cv2 v4.0.2

---

Before running the code:
Make sure the Rf_calculator.ipynb code and "display_image2_after.jpg" and "display_image2_after_analysed.jpg" are in the same file.
Make sure the test files are also in the same file.

---

In jupyter:
Run the code Rf_calculator.ipynb in the same file directory as test image files.

When prompted for a filename name, try "image.tiff".
The output is printed out, showing the orginial input file and the analysed plate.
A image file called "image_analysed.jpg" is saved in the same file directory.
To check the accuracy of the Rf values calculated, check Test_files_with_Rf.pdf

To test different test files, re-run the input cell and enter a different test filename.
For example: "coloured_spots.png", "image1.jpg"
The output is printed out and the name of the saved image file will be displayed in the output.
The image files are saved in the same file directory as the code and test files.

---

Description of test files provided:
"image.tiff", "image1.jpg", "coloured_spots.png" are files that work successfully in different image formats.

"image4_before.jpg" is a plate with oval spots that lead to inaccurate circle detection so Rf values are inaccurate.
"image4_after.jpg" is a plate with circles around the oval spots, leading to more accurate Rf values.

"column_1" files are examples of column chromatography TLCs with many spots.
"column_1.jpg" is a compressed image file.
"full_column_1.jpg" is a full quality image.

"image0.jpg", "blank.jpg", "no_spots.jpg", "only_bl.jpg" and "only_sf.jpg" are meant to break the code.
Error messages should appear.

"image0.jpg" has no plate.
"blank.jpg" is a empty plate.
"no_spots.jpg" has the pencil lines visible but no spots.
"only_bl.jpg" only have baseline visible .
"only_sf.jpg" only have solvent front visible.
