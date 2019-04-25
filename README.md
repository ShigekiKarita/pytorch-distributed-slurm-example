# distributed MNIST Example

```bash
pip install -r requirements.txt
python main.py
# lauch 2 gpus x 2 nodes (= 4 gpus)
srun -N2 -p gpu --gres gpu:2 python main_distributed.py --dist-backend nccl --multiprocessing-distributed --dist-file dist_file
```

