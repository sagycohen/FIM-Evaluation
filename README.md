# FIMevaluation
Framework for the evaluation of Flood Inundation Map (FIM) using a remote sensing derived benchmark FIM. The framework includes preprocessing of the benchmark layer and calculation of evaluation metrics.

Two ArcGIS Pro Notebooks (using ArcPy).
Overview:
1. Pre-processing Benchmark FIM (FIMGapFiller_BenchmarkProcessing.ipynb):
  1.1 Remove small ‘flooding’ clusters
  1.2 Enhancing the Remote Sensing FIM (GapFill/Region Growth)
  1.3 Removing Permanent Water Bodies (PWB)
  1.4 Matching Benchmark and Model FIMs (extent, resolution, and alignment)
  1.5 Prepare the final benchmark layer – classify gap-filled and PWB as NoData

2. Calculating Evaluation Metrics (ModelEval.ipynb):
  2.1 Re-classify benchmark [0,2] and predicted [1,2] FIM
  2.2 Generate a match classification raster (TP,  TN,  FP,  FN)
  2.3 Calculate evaluation metrics (CSI, TPR, FAR, F1, ACC)
