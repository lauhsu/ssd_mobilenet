# ssd_mobilenet
Forked from https://github.com/tensorflow/models

# Usage
1. Download data folder from \\diskstation\home\github\ssd_mobilenet
2. Download VOC2007 dataset and put in data folder
3. cd /opt/mobilessd/models/research
2. python object_detection/legacy/train.py  --pipeline_config_path="/opt/mobilessd/models/research/object_detection/samples/configs/ssd_mobilenet_v1_pets.config"   -train_dir="/opt/mobilessd/models/research/object_detection/data/"

# Issues
1. https://github.com/tensorflow/models/issues/1834
2. https://blog.csdn.net/xiji321/article/details/77163550?locationNum=4&fps=1
3. https://blog.csdn.net/Ivy_yijing1115/article/details/78915334
4. https://blog.csdn.net/huikey_buaa/article/details/79570179
5. 将VOC2007数据集转换为TFRecord格式 https://blog.csdn.net/weixin_37667519/article/details/79032870
   if len(xml)==0:
   python object_detection/dataset_tools/create_pascal_tf_record.py  --data_dir=/opt/mobilessd/models/research/object_detection/data--year=VOC2007  --output_path=/opt/mobilessd/models/research/object_detection/data/pascal.record
   
   
