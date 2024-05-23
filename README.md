Sen1Floods11: a georeferenced dataset to train and test deep learning flood algorithms for Sentinel-1 (Example). This data was generated by Cloud to Street, a Public Benefit Corporation: https://www.cloudtostreet.info/. For questions about this dataset or code please email support@cloudtostreet.info. Please cite this data as:
Bonafilia, D., Tellman, B., Anderson, T., Issenberg, E. 2020. Sen1Floods11: a georeferenced dataset to train and test deep learning flood algorithms for Sentinel-1. The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops, 2020, pp. 210-211.


Dataset Access

The dataset is available for access through Google Cloud Storage bucket at: "gs://senfloods11/"

You can access the dataset bucket using the gsutil command line tool. If you would like to download the entire dataset (~14 GB) you can use gsutil rsync to clone the bucket to a local directory. The -m flag is recommended to speed downloads. The -r flag will download sub-directories and folder recursively. See the example below.

$ gsutil -m rsync -r gs://sen1floods11 /YOUR/LOCAL/DIRECTORY/HERE
If using an example notebook, you can download the dataset to the folder that notebooks expect it to be in by running


$ mkdir /home/files
$ gsutil -m rsync -r gs://sen1floods11 /home/files
