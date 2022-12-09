# Running CompilerGym on SLURM

```
python launcher/slurm_launch.py --app=main_cg.py --time=10:00 -nc=80 -ng=2
```

# Running Custom trainer on SLURM

```
python launcher/slurm_launch.py --app=main.py --time=10:00 -nc=80 -ng=2
```

For Wandb support:
- Put your wandb key in /wandb_key.txt
- Uncomment "callbacks=[ WandbLoggerCallback..." from tune.run
- Set appropriate "project" parameter