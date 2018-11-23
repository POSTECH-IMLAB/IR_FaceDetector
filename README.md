# IR_FaceDetector
Face Detector for IR Images
Created by: Jongmin Yoon, Daijin Kim from POSTECH, South Korea

Abstract

We propose a novel multi-view face detector that operates accurately and fast in challenging environments. It consists of four consecutive functional components: background rejector, pose classifier, pose-specific face detectors, and face validator. The background rejector removes non-face patches quickly, the pose classifier estimates poses of the surviving patches, one or more selected pose-specific face detectors according to their estimated pose labels determine that a given patch is a face by using winner take all (WTA) strategy, and the face validator checks whether the face-like patch is really a face. For achieving strong discrimination power with low computing overhead, we devise several types of order relation features (ORF) that encode the order relation among feature elements as a unique code. The devised ORFs are placed in functional components appropriately to ensure fast operation of the multi-view face detector. For accurate classification, we propose a doubly domain-partitioning (DDP) classifier that consists of a coarse domain-partitioning weak classifier followed by a fine bin-partitioning weighted linear discriminant analysis (wLDA) classifier. For fast classification, we devise a feature sharing method that shares identical features between the background rejector and the pose classifier, and among all classes in the pose classifier. We evaluated the proposed multi-view face detector using the FDDB, AFW, and PASCAL face datasets. The experimental results show that the proposed multi-view face detector outperforms other stateof- the-art methods in terms of detection accuracy and execution time.

# Testing
Testing with webcam:
test.exe webcam

Testing with videos:
test.exe <input_video> <result_file_name>

testing with images:
test.exe images

# Related Papers
Yoon, Jongmin, and Daijin Kim. "An accurate and real-time multi-view face detector using ORFs and doubly domain-partitioning classifier." Journal of Real-Time Image Processing: 1-16.
