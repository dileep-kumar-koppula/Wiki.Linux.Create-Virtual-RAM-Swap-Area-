# Managing Swap Space in Linux

To manage swap space in Linux, you can use the following commands:

```bash
# Check current memory usage
free -h

# Show active swap spaces
swapon --show

# Disable the swap file
sudo swapoff /swapfile

# Create a new swap file of 4GB. Here, I am creating 4 GB of RAM
sudo fallocate -l 4G /swapfile

# Set up the swap file
sudo mkswap /swapfile

# Enable the swap file
sudo swapon /swapfile

# Verify the new swap space
swapon --show

# Check memory usage again
free -h
```
