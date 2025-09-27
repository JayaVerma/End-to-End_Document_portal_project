### to activate the env

```
conda activate /Users/jayaverma/Desktop/LLMOps-study/document/env
```

🔧 Fix 1 – Manually Fix PATH Priority
Since /Users/jayaverma/Desktop/LLMOps-study/document/env/bin appears after /usr/local/bin, we need to prepend it.

Run:
``` 
#temporary fix
export PATH="/Users/jayaverma/Desktop/LLMOps-study/document/env/bin:$PATH"
which python
python --version

# permanent fix
# Add this to your ~/.zshrc before Conda’s init:

# Force Conda env to take priority
export PATH="/Users/jayaverma/Desktop/LLMOps-study/document/env/bin:$PATH"
source ~/.zshrc
```

