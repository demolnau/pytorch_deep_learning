# Moving between CPU and GPU
Working with tensors, there is transferring data btw CPU and GPU
- output data will be generated on a GPU, but will require preprocessing that typically is only possible on a CPU
- some preprocessing libraries don't support tensors and expect NumPy array
- NumPy supports only data in the CPU

### Three ways to move from CPU to GPU
```
#1st way
Tensor.cuda()

#2nd way
Tensor.to("cuda")

#3rd way
Tensor.to("cuda:0")
```

### Moving from GPU to CPU
```
#1st way
Tensor.cpu()

#2nd way
Tensor.detach().cpu()
```