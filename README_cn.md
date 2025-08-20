## 模型导出

```python
python export_ppyoloe.py \
    -w ppyoloe_plus_crn_t_auxhead_relu_300e_coco.pdparams \
    -c configs/ppyoloe/ppyoloe_plus_crn_t_auxhead_relu_300e_coco.yml \
    --simplify
```

```python
python3 export_ppyoloe.py \
    -w ppyoloe_crn_s_400e_coco.pdparams \
    -c configs/ppyoloe/ppyoloe_crn_s_400e_coco.yml \
    --simplify
```


```python
python3 export_picodet.py \
    -w picodet_l_640_coco_lcnet.pdparams \
    -c configs/picodet/picodet_l_640_coco_lcnet.yml\
    --simplify
```


```python
python3 export_picodet_pedestrian.py \
    -w picodet_s_320_lcnet_pedestrian.pdparams \
    -c configs/picodet/application/pedestrian_detection/picodet_s_320_lcnet_pedestrian.yml \
    --simplify
```

## 模型推理
```python
python3 onnx_infer.py
```