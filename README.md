## 依赖库安装

```bash
pip install -r requirements-gpu.txt
```

## 数据集下载

```bash
cd ./script
./get_coco_dataset_2017.sh
```

## 训练命令

```bash
python train.py --weights ./data/yolov4.weights
```

## 验证命令

```bash
python evaluate.py --weights ./data/yolov4.weights
cd mAP/extra
python remove_space.py
cd ..
python main.py --output results_yolov4_tf
```

## 测试命令

源代码仓代码存在Bug，近期正在尝试修改

## 与标杆对比

无

