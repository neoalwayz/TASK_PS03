# DS_TASK_PS01
## Visual Search, Retrieval &amp; Detection 

A satellite image chip-based visual search task requires designing a system to find objects in multi-spectral satellite imagery based on sample image chips. The solution must support two input modes—image chip upload and bounding box selection—and produce a specific output format with bounding box coordinates, object name, file name, and similarity score, demonstrated in a Jupyter Notebook (Kaggle/Colab) on a mock dataset.

Key Requirements: 
Accept ≤5 sample image chips or bounding box selection in any satellite image for object/feature representation.

Search for visually similar objects across a folder of multi-spectral TIFF images (with four bands: Blue, Green, Red, NIR).

Output detections as:

xmin ymin xmax ymax object_name target_image_filename similarity_score (space-delimited; use -1 for missing similarity score).

Submission must include a Jupyter Notebook that demonstrates the end-to-end solution, including result visualization and output file generation on the test dataset.

Implementation Task Sections
Input Modes
Implement:

Using CLI
(Optional: Upload capability for image chips by the user.)

Interactive bounding box tool for selecting objects within a displayed satellite image.

Multi-Spectral Image Search
Load all TIFF files from the dataset folder.

For each sample chip/bounding box, search all images for visually similar regions using a similarity metric (e.g., feature embeddings or template matching across the four bands).

Detection and Output Formatting
For each detection, extract bounding box coordinates in [xmin, ymin, xmax, ymax].

Record detected class (object_name), target image filename, and similarity score (use -1 if undefined).

Save results as a space-delimited text file without headers.

Visualization and Submission
Visualize both sample images and detections in the notebook.

Show matched bounding boxes on corresponding images.

Demonstrate the workflow on mock data, including sample output file.
