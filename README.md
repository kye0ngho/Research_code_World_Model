# Research_code_World_Model


### 언어를 주고 안 주고 DMC_WALKER 

```bash

# 언어 on
sh xvfb_run.sh python3 dreamer.py \
  --configs dmc_vision \
  --task dmc_walker_walk \
  --logdir ./logdir_on/run1 \
  --lang_text "keep moving forward"
```

```bash

# 언어 off
sh xvfb_run.sh python3 dreamer.py \
  --configs dmc_vision \
  --task dmc_walker_walk \
  --logdir ./logdir_off/run1 \
  --lang_text ""
```


### 더 어려운 Task 를 위해 DMC_HUMANOID

```bash

# humanoid + 언어 on
sh xvfb_run.sh python3 dreamer.py \
  --configs dmc_vision \
  --task dmc_humanoid_walk \
  --logdir ./logdir_hubo_on/run1 \
  --lang_text "keep balance and move forward"
```

```bash
# humanoid + 언어 off
sh xvfb_run.sh python3 dreamer.py \
  --configs dmc_vision \
  --task dmc_humanoid_walk \
  --logdir ./logdir_hubo_off/run1 \
  --lang_text ""
```
