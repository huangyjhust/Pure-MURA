# PureMURA
A pre-operative sub-set of MURA dataset(https://stanfordmlgroup.github.io/competitions/mura/).

The dataset is avaliable at https://drive.google.com/open?id=140YHuHvjGxUJfvu2vsaKY4H4MR6tJDd

I noticed that, ~50% of the positive samples are with fracture indicators(steel plates, manual marks or in plaster). These indicators ruin CNN's understanding of fractures, thus CNNs easily identify fractures from seeing these indicators. However, a clinically valuable fracture recognition system should be capable of recognizing fractures from pre-operative samples rather than post-operative samples. 

Therefore, I mannually divided MURA dataset into two subsets, the subset with fracture indicators or pre-operative subset without indicators. By training models with the pre-operative subset, classification should be based on visual clues of fractures, not the indicators. Some post-operative samples may remain in the pre-operative dataset due to mistakes of mannual labour, but they are minority after all.

Below are a few fracture samples from PureMURA/train_AllPlate/

![Fig.1.](https://github.com/huangyjhust/PureMURA/blob/master/samples/1_Plaster.png)
![Fig.3.](https://github.com/huangyjhust/PureMURA/blob/master/samples/2_Plate.png)
![Fig.4.](https://github.com/huangyjhust/PureMURA/blob/master/samples/3_Mark.png)

Below are a few fracture samples from PureMURA/train_NoPlate/

![Fig.0.](https://github.com/huangyjhust/PureMURA/blob/master/samples/1_NoPlate.png)
![Fig.2.](https://github.com/huangyjhust/PureMURA/blob/master/samples/2_NoPlate.png)
![Fig.5.](https://github.com/huangyjhust/PureMURA/blob/master/samples/3_NoPlate.png)
