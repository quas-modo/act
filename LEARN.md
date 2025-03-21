# Learning ACT
## generate data
To generated 50 episodes of scripted data, run:

    python3 record_sim_episodes.py \
    --task_name sim_transfer_cube_scripted \
    --dataset_dir /ssd/home/chenxinyi/data/act \
    --num_episodes 50

在`scripted_policy.py`中可以看到，其实是写死了双臂的运动轨迹去执行。比如在`PickAndTransferPolicy`中，右臂怎么抓、什么时候释放、什么时候移开，都是写好的。