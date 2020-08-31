## Project1 :Improving Unsupervised Face Translationbetween Images and Videos

The image dataset CelebA can be downloaded from http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html. For the corresponding video dataset, Trailor faces from YouTube

Small image datatset(sample) is given in the folder: IDCycleGAN\test_image_128 as well as the index file is in the same folder: index_file_img_test_128
Video dataset(sample) given in the folder: IDCycleGAN\videos with index file: train_data.txt

1. Traning IdCycleGAN-model1

python `main_train_lau_best_models.py --experiment_name=idcyclegan_128alignhq_model1 --mode=idcyclegan_model1 --batch_size=16 --crop_size_img=128 --learning_rate=0.00028 --recover_model=False --sample_every=25 --save_model_every=1000 --num_epochs=50000`


2. Training IdCycleGAN-model2

python `main_train_lau_best_models.py --experiment_name=idcyclegan_128alignhq_model2 --mode=idcyclegan_model2 --batch_size=16 --crop_size_img=128 --learning_rate=0.00028 --recover_model=False --sample_every=25 --save_model_every=1000 --num_epochs=50000`


3. Training IdCycleGAN-model3

python `main_train_lau_best_models.py --experiment_name=idcyclegan_128alignhq_model3 --mode=idcyclegan_model3 --batch_size=16 --crop_size_img=128 --learning_rate=0.00028 --recover_model=False --sample_every=25 --save_model_every=10 --num_epochs=50python main_train_lau_best_models.py --experiment_name=idcyclegan_128alignhq_model3_stride4 --mode=idcyclegan_model3 --batch_size=16 --crop_size_img=128 --learning_rate=0.00028 --recover_model=False --sample_every=25 --save_model_every=1000 --num_epochs=50000`

Packages needed:
- tensorflow
- numpy
- random
- scipy
- scikit
- Pillow
- ffmpeg( conda install -c conda-forge ffmpeg)

