# DS_TASK_PS01
## Visual Search, Retrieval &amp; Detection 

A satellite image chip-based visual search task requires designing a system to find objects in multi-spectral satellite imagery based on sample image chips. The solution must support two input modes—image chip upload and bounding box selection—and produce a specific output format with bounding box coordinates, object name, file name, and similarity score, demonstrated in a Jupyter Notebook (Kaggle/Colab) on a mock dataset.

## Key Requirements: 
Accept ≤5 sample image chips or bounding box selection in any satellite image for object/feature representation.

Search for visually similar objects across a folder of multi-spectral TIFF images (with four bands: Blue, Green, Red, NIR).

## Output detections as:

(xmin ymin xmax ymax object_name target_image_filename similarity_score (space-delimited; use -1 for missing similarity score).

Submission must include a Jupyter Notebook that demonstrates the end-to-end solution, including result visualization and output file generation on the test dataset.

## Implementation Task Sections
Input Modes
Implement:

Recommended: 

Using CLI
(Optional: Upload capability for image chips by the user, Interactive bounding box tool for selecting objects within a displayed satellite image.)

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

## SUB-TASKS FOR EVALUATION

1. Data Input and Preprocessing
   
   1.1. Implement functionality to upload the desired object class.
   
   1.2. Implement interactive bounding box selection to capture object chips from given satellite imagery.

   1.3. Load and preprocess multi-spectral TIFF images (Blue, Green, Red, NIR bands) into a usable format for analysis.

3. Feature Extraction from Sample Chips

4. Satellite Image Dataset Processing

5. Visual Search and Similarity Matching
  
   4.1. Compute similarity scores between example chip features and candidate regions.

   4.2. Identify candidate regions exceeding a similarity threshold as potential matches.

5. Detection Output Generation

   5.1. For each matched region, extract bounding box coordinates [xmin, ymin, xmax, ymax].

   5.2. Record matched object name, source image filename, and similarity/confidence score.

   5.3. Format results as required: space-delimited text file without headers.

6. Visualization and Result Reporting
  
   6.1. Visualize input chips and drawn bounding boxes.

   6.2. Visualize matching candidate regions with bounding boxes on satellite images.

   6.3. Display similarity scores on visualizations for confirmation.

7. Jupyter Notebook Development
   
  Integrate each step into a cohesive, runnable notebook designed for Kaggle/Colab environment. Feel free to develope them locally or use kaggle/collab for computation requirements.

(optional: Include explanatory markdown cells for clarity.)

Demonstrate the full workflow on a provided mock dataset.

Export the final detection results in the required output format.

## Instruction for Submission

1. Send the link of 'Work Notebook/notebooks' in .ipynb format either by creating github repo or kaggle/collab to 'siddham@arms4ai.com' and 'nitish@arms4ai.com'. Make sure to set viewing permission to Public.
   
2. Last date of Submission is 06/10/2025 16:00:00 IST

Feel free to reach out to us in case there is any doubt regarding the task over the mentioned emails.
