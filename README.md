# Training torchvision models on CIFAR10
To start training from scratch define a config.json file as specified in config_example.json. <br>
Set "model" to one of the model names supported by the models.model_choice(name) function (currently only "resnet_18", "resnet50" and "mobilenet_v2"). 
```
# start training from scratch
python train.py --config_file config.json
```
```
# resume training from checkpoint (number of epochs is required in this case!)
python train.py --load path_to_checkpoint --epochs num_epochs_to_train
```
