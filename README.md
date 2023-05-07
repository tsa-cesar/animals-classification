# Projeto Final - Modelos Preditivos Conexionistas

### Thaís Santos Albuquerque

|**Tipo de Projeto**|**Modelo Selecionado**|**Linguagem**|
|--|--|--|
|Classificação de Imagens<br>|YOLOv5-Classify|PyTorch|

## Performance

O modelo treinado possui performance de **87.9%**.

### Output do bloco de treinamento

<details>
  <summary>Click to expand!</summary>
  
  ```text
    albumentations: RandomResizedCrop(p=1.0, height=640, width=640, scale=(0.08, 1.0), ratio=(0.75, 1.3333333333333333), interpolation=1), HorizontalFlip(p=0.5), ColorJitter(p=0.5, brightness=[0.6, 1.4], contrast=[0.6, 1.4], saturation=[0.6, 1.4], hue=[0, 0]), Normalize(p=1.0, mean=(0.485, 0.456, 0.406), std=(0.229, 0.224, 0.225), max_pixel_value=255.0), ToTensorV2(always_apply=True, p=1.0, transpose_mask=False)
Downloading https://github.com/ultralytics/yolov5/releases/download/v7.0/yolov5s-cls.pt to yolov5s-cls.pt...
100% 10.5M/10.5M [00:00<00:00, 114MB/s]
    Model summary: 149 layers, 4177604 parameters, 4177604 gradients, 10.5 GFLOPs
optimizer: Adam(lr=0.001) with parameter groups 32 weight(decay=0.0), 33 weight(decay=5e-05), 33 bias
Image sizes 640 train, 640 test
Using 1 dataloader workers
Logging results to runs/train-cls/exp
Starting yolov5s-cls.pt training on Images-4 dataset with 4 classes for 200 epochs...

     Epoch   GPU_mem  train_loss   test_loss    top1_acc    top5_acc
     1/200     9.43G        1.35        1.38           0           1: 100% 8/8 [00:09<00:00,  1.24s/it]
     2/200     9.43G         1.1        1.35           0           1: 100% 8/8 [00:09<00:00,  1.20s/it]
     3/200     9.43G        1.03        1.27       0.333           1: 100% 8/8 [00:10<00:00,  1.37s/it]
     4/200     9.43G       0.962        1.21       0.545           1: 100% 8/8 [00:11<00:00,  1.39s/it]
     5/200     9.43G       0.974        1.35           0           1: 100% 8/8 [00:09<00:00,  1.19s/it]
     6/200     9.43G       0.959        1.58      0.0303           1: 100% 8/8 [00:10<00:00,  1.35s/it]
     7/200     9.43G       0.927         1.6       0.242           1: 100% 8/8 [00:11<00:00,  1.38s/it]
     8/200     9.43G       0.939        1.53       0.455           1: 100% 8/8 [00:10<00:00,  1.32s/it]
     9/200     9.43G       0.926        1.55       0.545           1: 100% 8/8 [00:09<00:00,  1.22s/it]
    10/200     9.43G       0.972         1.9           0           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    11/200     9.43G       0.894        1.61       0.333           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    12/200     9.43G       0.903         1.4       0.485           1: 100% 8/8 [00:09<00:00,  1.17s/it]
    13/200     9.43G       0.858        1.32       0.394           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    14/200     9.43G       0.926        1.08       0.727           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    15/200     9.43G       0.885        1.29       0.455           1: 100% 8/8 [00:10<00:00,  1.29s/it]
    16/200     9.43G       0.835         1.6       0.394           1: 100% 8/8 [00:10<00:00,  1.32s/it]
    17/200     9.43G       0.878        1.46       0.364           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    18/200     9.43G       0.893        1.53       0.364           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    19/200     9.43G       0.822        1.39       0.424           1: 100% 8/8 [00:09<00:00,  1.18s/it]
    20/200     9.43G       0.888        1.12       0.515           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    21/200     9.43G       0.894        1.22       0.606           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    22/200     9.43G        0.86        1.49       0.424           1: 100% 8/8 [00:10<00:00,  1.31s/it]
    23/200     9.43G       0.846        1.16       0.606           1: 100% 8/8 [00:09<00:00,  1.25s/it]
    24/200     9.43G       0.824        1.65       0.424           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    25/200     9.43G       0.897        1.49       0.394           1: 100% 8/8 [00:10<00:00,  1.36s/it]
    26/200     9.43G       0.851        1.71       0.182           1: 100% 8/8 [00:09<00:00,  1.25s/it]
    27/200     9.43G       0.841        1.96       0.273           1: 100% 8/8 [00:10<00:00,  1.35s/it]
    28/200     9.43G       0.815        1.21       0.636           1: 100% 8/8 [00:10<00:00,  1.33s/it]
    29/200     9.43G       0.867        2.83       0.333           1: 100% 8/8 [00:10<00:00,  1.37s/it]
    30/200     9.43G       0.825        1.25       0.576           1: 100% 8/8 [00:09<00:00,  1.21s/it]
    31/200     9.43G       0.818         1.4       0.515           1: 100% 8/8 [00:10<00:00,  1.37s/it]
    32/200     9.43G       0.835        1.56       0.485           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    33/200     9.43G       0.812        1.65       0.455           1: 100% 8/8 [00:10<00:00,  1.25s/it]
    34/200     9.43G       0.852        1.27       0.545           1: 100% 8/8 [00:10<00:00,  1.33s/it]
    35/200     9.43G        0.81        1.76       0.455           1: 100% 8/8 [00:11<00:00,  1.42s/it]
    36/200     9.43G       0.793        1.27       0.576           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    37/200     9.43G       0.807        1.43       0.667           1: 100% 8/8 [00:09<00:00,  1.21s/it]
    38/200     9.43G       0.807        1.64       0.424           1: 100% 8/8 [00:11<00:00,  1.41s/it]
    39/200     9.43G       0.806        1.21       0.667           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    40/200     9.43G       0.731        1.54       0.364           1: 100% 8/8 [00:10<00:00,  1.35s/it]
    41/200     9.43G       0.785        1.75       0.515           1: 100% 8/8 [00:10<00:00,  1.25s/it]
    42/200     9.43G        0.81        1.22       0.515           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    43/200     9.43G       0.789        1.69       0.242           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    44/200     9.43G       0.796        1.78       0.273           1: 100% 8/8 [00:09<00:00,  1.25s/it]
    45/200     9.43G       0.825        1.64       0.333           1: 100% 8/8 [00:10<00:00,  1.33s/it]
    46/200     9.43G       0.786        1.85       0.303           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    47/200     9.43G       0.775        1.79       0.333           1: 100% 8/8 [00:11<00:00,  1.41s/it]
    48/200     9.43G       0.748        1.75       0.455           1: 100% 8/8 [00:09<00:00,  1.19s/it]
    49/200     9.43G       0.767         1.1       0.727           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    50/200     9.43G       0.715        1.12       0.788           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    51/200     9.43G       0.688        1.46       0.485           1: 100% 8/8 [00:10<00:00,  1.30s/it]
    52/200     9.43G        0.68       0.748       0.909           1: 100% 8/8 [00:10<00:00,  1.28s/it]
    53/200     9.43G       0.696        1.02       0.848           1: 100% 8/8 [00:10<00:00,  1.36s/it]
    54/200     9.43G       0.684       0.782       0.848           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    55/200     9.43G       0.658           1       0.697           1: 100% 8/8 [00:09<00:00,  1.23s/it]
    56/200     9.43G        0.71       0.886       0.758           1: 100% 8/8 [00:10<00:00,  1.36s/it]
    57/200     9.43G        0.73        1.03       0.758           1: 100% 8/8 [00:10<00:00,  1.37s/it]
    58/200     9.43G       0.714           1       0.727           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    59/200     9.43G       0.684       0.828       0.879           1: 100% 8/8 [00:09<00:00,  1.22s/it]
    60/200     9.43G       0.643        1.67       0.455           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    61/200     9.43G       0.611        1.45       0.515           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    62/200     9.43G       0.627        1.33       0.667           1: 100% 8/8 [00:10<00:00,  1.27s/it]
    63/200     9.43G       0.656           2       0.242           1: 100% 8/8 [00:10<00:00,  1.31s/it]
    64/200     9.43G       0.639        1.09       0.667           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    65/200     9.43G       0.638        1.38       0.636           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    66/200     9.43G       0.593        1.27       0.697           1: 100% 8/8 [00:09<00:00,  1.21s/it]
    67/200     9.43G       0.622         1.6       0.545           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    68/200     9.43G       0.671        2.33       0.152           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    69/200     9.43G       0.622        1.54       0.485           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    70/200     9.43G        0.63        1.62       0.485           1: 100% 8/8 [00:09<00:00,  1.23s/it]
    71/200     9.43G       0.604        1.47       0.576           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    72/200     9.43G       0.592        1.43       0.515           1: 100% 8/8 [00:11<00:00,  1.41s/it]
    73/200     9.43G       0.601        1.23       0.667           1: 100% 8/8 [00:09<00:00,  1.25s/it]
    74/200     9.43G       0.589        1.08       0.727           1: 100% 8/8 [00:10<00:00,  1.35s/it]
    75/200     9.43G       0.601        1.17       0.667           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    76/200     9.43G       0.589        1.95       0.333           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    77/200     9.43G       0.578        1.61       0.424           1: 100% 8/8 [00:09<00:00,  1.19s/it]
    78/200     9.43G       0.595        1.73       0.303           1: 100% 8/8 [00:10<00:00,  1.37s/it]
    79/200     9.43G       0.585        1.38       0.485           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    80/200     9.43G       0.637        1.27       0.667           1: 100% 8/8 [00:10<00:00,  1.34s/it]
    81/200     9.43G       0.579        1.51       0.455           1: 100% 8/8 [00:10<00:00,  1.28s/it]
    82/200     9.43G       0.574        1.33       0.576           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    83/200     9.43G       0.577        1.87       0.333           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    84/200     9.43G       0.537        1.62       0.424           1: 100% 8/8 [00:09<00:00,  1.22s/it]
    85/200     9.43G       0.561        1.62       0.394           1: 100% 8/8 [00:10<00:00,  1.35s/it]
    86/200     9.43G       0.578        1.37       0.515           1: 100% 8/8 [00:11<00:00,  1.40s/it]
    87/200     9.43G       0.548        1.13       0.697           1: 100% 8/8 [00:10<00:00,  1.36s/it]
    88/200     9.43G       0.599        1.11       0.697           1: 100% 8/8 [00:09<00:00,  1.23s/it]
    89/200     9.43G       0.545        1.12       0.697           1: 100% 8/8 [00:11<00:00,  1.41s/it]
    90/200     9.43G       0.566        1.53       0.455           1: 100% 8/8 [00:11<00:00,  1.38s/it]
    91/200     9.43G       0.571        2.15       0.333           1: 100% 8/8 [00:10<00:00,  1.29s/it]
    92/200     9.43G       0.549        1.15       0.697           1: 100% 8/8 [00:10<00:00,  1.27s/it]
    93/200     9.43G        0.57        1.68       0.515           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    94/200     9.43G       0.523        1.58       0.394           1: 100% 8/8 [00:11<00:00,  1.42s/it]
    95/200     9.43G       0.551        1.59       0.455           1: 100% 8/8 [00:09<00:00,  1.21s/it]
    96/200     9.43G       0.553        1.52       0.576           1: 100% 8/8 [00:10<00:00,  1.36s/it]
    97/200     9.43G       0.561        1.45       0.515           1: 100% 8/8 [00:11<00:00,  1.39s/it]
    98/200     9.43G       0.597        1.65       0.485           1: 100% 8/8 [00:10<00:00,  1.36s/it]
    99/200     9.43G       0.596        1.47       0.727           1: 100% 8/8 [00:09<00:00,  1.19s/it]
   100/200     9.43G       0.593        1.27       0.758           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   101/200     9.43G       0.537        1.44       0.515           1: 100% 8/8 [00:11<00:00,  1.38s/it]
   102/200     9.43G       0.545        1.65       0.485           1: 100% 8/8 [00:09<00:00,  1.25s/it]
   103/200     9.43G       0.516        1.81       0.455           1: 100% 8/8 [00:10<00:00,  1.35s/it]
   104/200     9.43G        0.56         1.7       0.364           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   105/200     9.43G       0.558        1.43       0.576           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   106/200     9.43G       0.563        1.65       0.515           1: 100% 8/8 [00:09<00:00,  1.19s/it]
   107/200     9.43G       0.586        1.71       0.394           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   108/200     9.43G       0.535        1.05       0.667           1: 100% 8/8 [00:11<00:00,  1.41s/it]
   109/200     9.43G       0.588        1.16       0.667           1: 100% 8/8 [00:09<00:00,  1.25s/it]
   110/200     9.43G       0.547        1.35       0.636           1: 100% 8/8 [00:10<00:00,  1.29s/it]
   111/200     9.43G       0.519        1.43       0.545           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   112/200     9.43G       0.545        1.52       0.424           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   113/200     9.43G       0.528         2.1       0.212           1: 100% 8/8 [00:09<00:00,  1.20s/it]
   114/200     9.43G        0.56        1.48       0.576           1: 100% 8/8 [00:11<00:00,  1.38s/it]
   115/200     9.43G       0.552        1.44       0.606           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   116/200     9.43G       0.541        1.42       0.576           1: 100% 8/8 [00:10<00:00,  1.33s/it]
   117/200     9.43G       0.593        1.46       0.455           1: 100% 8/8 [00:10<00:00,  1.26s/it]
   118/200     9.43G       0.563       0.997       0.697           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   119/200     9.43G       0.569        2.06       0.394           1: 100% 8/8 [00:11<00:00,  1.41s/it]
   120/200     9.43G       0.539        2.09       0.303           1: 100% 8/8 [00:09<00:00,  1.21s/it]
   121/200     9.43G       0.552        1.41       0.576           1: 100% 8/8 [00:10<00:00,  1.35s/it]
   122/200     9.43G       0.498         1.2       0.606           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   123/200     9.43G       0.526       0.983       0.727           1: 100% 8/8 [00:10<00:00,  1.33s/it]
   124/200     9.43G        0.54         1.4       0.424           1: 100% 8/8 [00:09<00:00,  1.22s/it]
   125/200     9.43G       0.531        1.32       0.576           1: 100% 8/8 [00:11<00:00,  1.41s/it]
   126/200     9.43G       0.535        1.48       0.576           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   127/200     9.43G       0.483        1.21       0.697           1: 100% 8/8 [00:09<00:00,  1.23s/it]
   128/200     9.43G       0.545        1.63       0.424           1: 100% 8/8 [00:10<00:00,  1.35s/it]
   129/200     9.43G        0.54        1.73       0.303           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   130/200     9.43G       0.553         1.8       0.303           1: 100% 8/8 [00:11<00:00,  1.38s/it]
   131/200     9.43G       0.504        1.76       0.364           1: 100% 8/8 [00:09<00:00,  1.20s/it]
   132/200     9.43G       0.492        1.48       0.515           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   133/200     9.43G       0.536        1.36       0.515           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   134/200     9.43G       0.536         1.6       0.485           1: 100% 8/8 [00:10<00:00,  1.27s/it]
   135/200     9.43G       0.504        1.66       0.485           1: 100% 8/8 [00:10<00:00,  1.30s/it]
   136/200     9.43G       0.524         1.5       0.485           1: 100% 8/8 [00:11<00:00,  1.42s/it]
   137/200     9.43G       0.511        1.43       0.485           1: 100% 8/8 [00:11<00:00,  1.38s/it]
   138/200     9.43G       0.537        1.03       0.697           1: 100% 8/8 [00:09<00:00,  1.18s/it]
   139/200     9.43G       0.487        1.27       0.576           1: 100% 8/8 [00:11<00:00,  1.42s/it]
   140/200     9.43G       0.502        1.47       0.455           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   141/200     9.43G       0.477        1.21       0.636           1: 100% 8/8 [00:11<00:00,  1.38s/it]
   142/200     9.43G       0.502        1.08       0.697           1: 100% 8/8 [00:09<00:00,  1.24s/it]
   143/200     9.43G       0.491        1.54       0.515           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   144/200     9.43G       0.527        1.48       0.515           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   145/200     9.43G         0.5        1.54       0.485           1: 100% 8/8 [00:10<00:00,  1.27s/it]
   146/200     9.43G       0.466        1.53       0.515           1: 100% 8/8 [00:10<00:00,  1.27s/it]
   147/200     9.43G       0.498        1.43       0.545           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   148/200     9.43G       0.523        1.32       0.636           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   149/200     9.43G       0.496        1.49       0.515           1: 100% 8/8 [00:09<00:00,  1.20s/it]
   150/200     9.43G       0.468        1.28       0.636           1: 100% 8/8 [00:10<00:00,  1.36s/it]
   151/200     9.43G       0.504        1.99       0.333           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   152/200     9.43G       0.507        1.41       0.576           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   153/200     9.43G       0.471         1.6       0.455           1: 100% 8/8 [00:09<00:00,  1.19s/it]
   154/200     9.43G       0.507        1.44       0.515           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   155/200     9.43G       0.511         1.7       0.364           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   156/200     9.43G        0.51         1.6       0.424           1: 100% 8/8 [00:10<00:00,  1.25s/it]
   157/200     9.43G       0.479        1.38       0.606           1: 100% 8/8 [00:10<00:00,  1.30s/it]
   158/200     9.43G       0.495        1.32       0.636           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   159/200     9.43G       0.482        1.16       0.667           1: 100% 8/8 [00:11<00:00,  1.42s/it]
   160/200     9.43G       0.492        1.16       0.697           1: 100% 8/8 [00:09<00:00,  1.18s/it]
   161/200     9.43G       0.475        1.21       0.606           1: 100% 8/8 [00:11<00:00,  1.38s/it]
   162/200     9.43G       0.453        1.13       0.727           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   163/200     9.43G       0.469         1.3       0.576           1: 100% 8/8 [00:10<00:00,  1.30s/it]
   164/200     9.43G        0.46         1.5       0.455           1: 100% 8/8 [00:10<00:00,  1.29s/it]
   165/200     9.43G        0.48        1.37       0.606           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   166/200     9.43G       0.488        1.25       0.606           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   167/200     9.43G       0.475        1.17       0.606           1: 100% 8/8 [00:09<00:00,  1.20s/it]
   168/200     9.43G       0.462        1.09       0.697           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   169/200     9.43G        0.47        1.34       0.545           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   170/200     9.43G       0.477        1.24       0.636           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   171/200     9.43G       0.457         1.3       0.606           1: 100% 8/8 [00:09<00:00,  1.22s/it]
   172/200     9.43G       0.462        1.11       0.697           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   173/200     9.43G        0.49        1.21       0.606           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   174/200     9.43G       0.473        1.35       0.515           1: 100% 8/8 [00:10<00:00,  1.28s/it]
   175/200     9.43G       0.453        1.25       0.636           1: 100% 8/8 [00:10<00:00,  1.29s/it]
   176/200     9.43G        0.48        1.34       0.606           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   177/200     9.43G       0.513         1.4       0.515           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   178/200     9.43G       0.467        1.46       0.424           1: 100% 8/8 [00:09<00:00,  1.18s/it]
   179/200     9.43G        0.47        1.39       0.545           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   180/200     9.43G       0.464        1.25       0.606           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   181/200     9.43G       0.469        1.27       0.576           1: 100% 8/8 [00:10<00:00,  1.29s/it]
   182/200     9.43G        0.46        1.37       0.515           1: 100% 8/8 [00:10<00:00,  1.27s/it]
   183/200     9.43G       0.489        1.23       0.667           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   184/200     9.43G       0.471        1.23       0.667           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   185/200     9.43G       0.435        1.36       0.545           1: 100% 8/8 [00:09<00:00,  1.21s/it]
   186/200     9.43G       0.463        1.48       0.515           1: 100% 8/8 [00:11<00:00,  1.38s/it]
   187/200     9.43G       0.448        1.47       0.485           1: 100% 8/8 [00:11<00:00,  1.42s/it]
   188/200     9.43G       0.487        1.27       0.606           1: 100% 8/8 [00:10<00:00,  1.36s/it]
   189/200     9.43G       0.479        1.29       0.576           1: 100% 8/8 [00:09<00:00,  1.19s/it]
   190/200     9.43G       0.452         1.4       0.515           1: 100% 8/8 [00:11<00:00,  1.40s/it]
   191/200     9.43G       0.451        1.41       0.515           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   192/200     9.43G       0.492         1.3       0.636           1: 100% 8/8 [00:10<00:00,  1.29s/it]
   193/200     9.43G       0.455        1.36       0.576           1: 100% 8/8 [00:10<00:00,  1.29s/it]
   194/200     9.43G       0.468        1.33       0.545           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   195/200     9.43G       0.452        1.25       0.606           1: 100% 8/8 [00:11<00:00,  1.39s/it]
   196/200     9.43G       0.475        1.19       0.667           1: 100% 8/8 [00:09<00:00,  1.20s/it]
   197/200     9.43G       0.437        1.21       0.636           1: 100% 8/8 [00:10<00:00,  1.37s/it]
   198/200     9.43G       0.455        1.21       0.667           1: 100% 8/8 [00:11<00:00,  1.41s/it]
   199/200     9.43G       0.459        1.23       0.636           1: 100% 8/8 [00:10<00:00,  1.36s/it]
   200/200     9.43G       0.459        1.26       0.606           1: 100% 8/8 [00:09<00:00,  1.23s/it]

Training complete (0.603 hours)
Results saved to runs/train-cls/exp
Predict:         python classify/predict.py --weights runs/train-cls/exp/weights/best.pt --source im.jpg
Validate:        python classify/val.py --weights runs/train-cls/exp/weights/best.pt --data /content/datasets/Images-4
Export:          python export.py --weights runs/train-cls/exp/weights/best.pt --include onnx
PyTorch Hub:     model = torch.hub.load('ultralytics/yolov5', 'custom', 'runs/train-cls/exp/weights/best.pt')
Visualize:       https://netron.app
  ```
</details>

### Evidências do treinamento

Gráfico de acurária:
![W B Chart 07_05_2023, 13 27 43(1)](https://user-images.githubusercontent.com/131788893/236690333-4eee543c-b243-4b4d-90fb-0b8515879c61.png)

Gráficos de perda:
![W B Chart 07_05_2023, 13 28 06(1)](https://user-images.githubusercontent.com/131788893/236690353-0707cdee-5da1-4594-80a2-2153563ba42b.png)
![W B Chart 07_05_2023, 13 28 24(1)](https://user-images.githubusercontent.com/131788893/236690365-37fb0da2-522f-4b90-af46-79a1a1e8b5f8.png)

## Roboflow

Nessa seção deve colocar o link para acessar o dataset no Roboflow

[Roboflow Dataset](https://universe.roboflow.com/classification/images-hzj5q)

## HuggingFace

Nessa seção você deve publicar o link para o HuggingFace
