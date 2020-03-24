# Read-RTSTRUCT-to-matlab
Read rtstruct set into matlab as binary mask

The “radiotherapy structure set” (RTSTRUCT) object of the DICOM standard is used for the transfer of patient structures and related data, between the devices found within and outside the radiotherapy department. It contains mainly the information for regions of interest (ROIs) for tumor and points of interest (e.g., dose reference points). Without the dicom image files, the RTSTRUCT.dcm file will be meaningless. 

To read the RTSTRUCT into matlab, make sure you download these five functions and add them to matlab searching path. Then put your single RTSTRUCT file and your dicom image files in the same folder (e.g. FolderA), and just run these 2 lines:


% Specify the path of the folder

directory='/Users/xxxx/Desktop/FolderA';


% Output into the same folder

files_out = scanDir(directory);

You should see the .mat file saved in the same folder. It could take a few minutes to get the output depending on the number of CT slices and structures.

Here is the link for the explanation:
https://www.mathworks.com/matlabcentral/answers/120098-how-to-read-dicom-rt-structure
