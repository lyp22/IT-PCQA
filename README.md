# IT-PCQA
If you use this code please cite the paper   

    "Qi Yang, Yipeng Liu, Siheng Chen, Yiling Xu, Jun Sun, "No-Reference Point Cloud Quality Assessment via Domain Adaptation," in CVPR, 2022."  
    
Bibtex:    
  
@InProceedings{yang2022ITPCQA,  
author = {Qi Yang and Yipeng Liu and Siheng Chen and Yiling Xu and Jun Sun},  
title = {No-Reference Point Cloud Quality Assessment via Domain Adaptation},  
booktitle = {Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},  
year = {2022}  
}
  
train.py is the main program. The explanations of some parameters are as below: 

parser.add_argument('--batch_size', type=int, default=16,
                        help='input batch size for training')  
parser.add_argument('--test_batch_size', type=int, default=16,
					help='input batch size for testing')  
parser.add_argument('--epochs', type=int, default=50, metavar='N',
					help='number of epochs to train')  
parser.add_argument('--lr', type=float, default=0.003, metavar='LR')  
parser.add_argument('--momentum', type=float, default=0.9, metavar='M',
					help='SGD momentum')  
parser.add_argument('--slabelscale', type=float, default=9.0,
					help='Maximum value of labels for source domain')  
parser.add_argument('--tlabelscale', type=float, default=9.0,
					help='Maximum value of labels for target domain')  
