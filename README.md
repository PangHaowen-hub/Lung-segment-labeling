# 肺段标注
### step1 分割气道树和动静脉

### step2 生成raw

分割得到 CT3_clean_hu.nii.gz、CT3_av.nii.gz、CT3_airway.nii.gz

使用nnU-Net分割肺叶得到CT3_lobe_mask.nii.gz

运行nii2raw.py将这四个文件结合写为raw格式

### step3 使用mimics分割