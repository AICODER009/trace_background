# DEEPLABV3
All pre-trained models expect input images normalized in the same way, i.e. mini-batches of 3-channel RGB images of shape (N, 3, H, W), where N is the number of images, H and W are expected to be at least 224 pixels. The images have to be loaded in to a range of [0, 1] and then normalized using mean = [0.485, 0.456, 0.406] and std = [0.229, 0.224, 0.225].

The model returns an OrderedDict with two Tensors that are of the same height and width as the input Tensor, but with 21 classes. output['out'] contains the semantic masks, and output['aux'] contains the auxiliary loss values per-pixel. In inference mode, output['aux'] is not useful. So, output['out'] is of shape (N, 21, H, W). More documentation can be found here.

![image](https://github.com/AICODER009/trace_background/assets/133597851/94a85992-104d-4ee0-bbe1-1b3281378a17)

![image](https://github.com/AICODER009/trace_background/assets/133597851/066caada-be99-46b1-8416-d58188250229)
