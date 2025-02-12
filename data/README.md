# Prepare Datasets for P<sup>2</sup>SAM

Download the 
[NSCLC-Radiomics](https://www.cancerimagingarchive.net/collection/nsclc-radiomics/), 
[4D-Lung](https://www.cancerimagingarchive.net/collection/4d-lung/),
[Kvasir-SEG](https://datasets.simula.no/kvasir-seg/), 
[CVC-ClinicDB](https://polyp.grand-challenge.org/CVCClinicDB/), 
and [PerSeg](https://drive.google.com/file/d/18TbrwhZtAPY5dlaoEqkPa5h08G9Rjcio/view) 
datasets. 
Organize them as follows:

## NSCLC Datasets

**Raw Data**
```
data
├── lung_org/
│  ├── NSCLC-Radiomics/
│  │  ├── LUNG1-001/
│  │  ├── .../
│  │  └── LUNG1-422/
│  └── 4D-Lung
│     ├── 100_HM10395/
│     ├── .../
│     └── 119_HM10395/
```

**Processed Data (lung.ipynb)**
```
data
├── lung_pro/
│  ├── nsclc_radiomics/
│  │  ├── image/ LUNG*/ *.png
│  │  └── label/ LUNG*/ *.png
│  └── 4d_lung_multi_visits/
│     ├── image/ *_HM10395/ *.png
│     └── label/ *_HM10395/ *.png
```

## Endoscopy Datasets

**Raw Data**
```
data
├── endoscopy_org/
│  ├── Kvasir-SEG/
│  │  ├── images/ *.jpg
│  │  └── masks/ *.jpg
│  └──CVC-ClinicDB
│     ├── Ground Truth/ *.tif
│     └── Original/ *.tif
```

**Processed Data (endoscopy.ipynb)**
```
data
├── endoscopy_pro/
│  ├── kvasir_seg/
│  │  ├── image/ *.png
│  │  └── label/ *.png
│  └── cvc_clinicdb/
│     ├── image/ video*/ *.png
│     └── label/ video*/ *.png
```

## PerSeg
```
data/
├── perseg/
│   ├── Annotations/ objects/ *.png
│   └── Images/ objects/ *.jpg
```
