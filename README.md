# distributed MNIST Example

```bash
pip install -r requirements.txt
python main.py
# using NFS and slurm job scheduler
srun -n2 -N2 -p gpu --gres gpu:2 python main_distributed.py --dist-backend nccl --multiprocessing-distributed --dist-file dist_file
```

