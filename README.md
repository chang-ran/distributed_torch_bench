# Distributed Torch Benchmarks 
## usage
worker0:
`torchrun --nproc_per_node 8 --master_addr <worker0 ip> --master_port 5678 --nnodes 2 --node_rank 0 -- run_bench.py -b 10G -n 20 -c all_reduce`
worker1:
`torchrun --nproc_per_node 8 --master_addr <worker0 ip> --master_port 5678 --nnodes 2 --node_rank 1 -- run_bench.py -b 10G -n 20 -c all_reduce`
