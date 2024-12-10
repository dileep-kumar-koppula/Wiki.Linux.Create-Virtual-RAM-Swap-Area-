# Managing Swap Space in Linux

To manage swap space in Linux, you can use the following commands:

+ Check current memory usage
  ```bash
  free -h
  ```

+ Show active swap spaces
  ```bash
  swapon --show
  ```

+ Disable the swap file
  ```bash
  sudo swapoff /swapfile
  ```

+ Create a new swap file of 4GB. Here, I am creating 4 GB of RAM
  ```bash
  sudo fallocate -l 4G /swapfile
  ```

+ Set up the swap file
  ```bash
  sudo mkswap /swapfile
  ```

+ Enable the swap file
  ```bash
  sudo swapon /swapfile
  ```

+ Verify the new swap space
  ```bash
  swapon --show
  ```

+ Check memory usage again
  ```bash
  free -h
  ```
