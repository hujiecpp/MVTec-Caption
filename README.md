# README

## **Building the MVTec Caption Dataset**

This document describes how to build the **MVTec Caption Dataset**.
The MVTec Caption Dataset is constructed in two parts, requiring the separate construction of the **MVTEC-AD-Caption** and **MVTEC-LOCO-Caption** datasets.

### **（1）MVTEC-AD-Caption**

1. Download the MVTEC-AD dataset from [https://www.mvtec.com/company/research/datasets/mvtec-ad](https://www.mvtec.com/company/research/datasets/mvtec-ad)
2. Run tools/Construct_MVTEC-AD-Caption.py to build the MVTEC-AD-Caption part of the dataset.

```python
python tools/Construct_MVTEC-AD-Caption.py
```

### **（2）MVTEC-LOCO-Caption**

1. Download the **MVTec LOCO AD** dataset from [https://www.mvtec.com/company/research/datasets/mvtec-loco](https://www.mvtec.com/company/research/datasets/mvtec-loco)
2. Run tools/Construct_MVTEC-LOCO-Caption.py to build the MVTEC-LOCO-Caption part of the dataset.

```python
python tools/Construct_MVTEC-LOCO-Caption.py
```

### **Dataset Structure**

**Expected Structure for MVTEC-AD-Caption**

```text
datasets/
	mvtec_anomaly_detection/
	  bottle/
	    ground_truth/
	    prompt/
	    test/
	    train/
	  cable/
	    ground_truth/
	    prompt/
	    test/
	    train/
	  ...
	  zipper/
	    ground_truth/
	    prompt/
	    test/
	    train/
```

**Expected Structure for MVTEC-LOCO-Caption**

```text
datasets/
	mvtec_loco_anomaly_detection/
	  breakfast_box/
	    ground_truth/
	    ground_truth_merge_mask/
		prompt/
		test/
	    train/
	  juice_bottle/
	    ground_truth/
	    ground_truth_merge_mask/
		prompt/
		test/
	    train/
	  ...
	  splicing_connectors/
	    ground_truth/
	    ground_truth_merge_mask/
		prompt/
		test/
	    train/
```