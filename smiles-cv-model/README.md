# smilesRecognition
This model supports converting chemical image into SMILES and other chemical representations.


### Install Enviroment



```
conda env create --name chem_info_env --file utils/chem_info.yml
```



### Prediction

Put images which you want to predict under the folder */model/utils/input_img*

Run command under path *model/*

```
python one_input_pred.py | tee log.csv
```


### ensemble prediction(multi-model)

Change test path in ./src/config.py.

Run command 

```
python main.py --work_type ensemble_test
```



You can find the predicted images in folder *"/model/utils/pred_img"*