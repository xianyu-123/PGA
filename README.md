# PGA
This is an alternative installation method for BiocManager::install("wenbostar/PGA"). 

Orign: https://github.com/wenbostar/PGA


tar -zxvf PGA405.tar.gz to a new folder, and then copy all the contents of the folder to the R directory of the virtual environment, such as /t9k/mnt/.conda/envs/testR/lib/R/.

```
python=3.7

conda install r-base=4.0.5

google drive (https://drive.google.com/file/d/1CmcU8kKJ6JnUbyygSKmMNljDaf6UHXwW/view?usp=drive_link)

tar -zxvf a.tar.gz -C /path/to/new_folder

cp -r /path/to/new_folder/* /t9k/mnt/.conda/envs/testR/lib/R/
