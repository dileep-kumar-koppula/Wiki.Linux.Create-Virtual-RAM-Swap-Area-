# Managing Swap Space in Linux

When managing swap space in Linux, you may need to perform several operations. Below are the commands you can use, along with a brief explanation of each:

1. **Check current memory usage:**
   - `free -h`
   - This command displays the current memory usage, including swap space, in a human-readable format.

2. **Show active swap spaces:**
   - `swapon --show`
   - This command lists all active swap spaces currently in use.

3. **Disable the swap file:**
   - `sudo swapoff /swapfile`
   - This command turns off the specified swap file, making it inactive.

4. **Create a new swap file:**
   - `sudo fallocate -l 4G /swapfile`
   - This command allocates a new file of 4GB to be used as swap space.

5. **Set up the swap file:**
   - `sudo mkswap /swapfile`
   - This command formats the newly created file to be used as swap space.

6. **Enable the swap file:**
   - `sudo swapon /swapfile`
   - This command activates the swap file, making it available for use.

7. **Verify the new swap space:**
   - `swapon --show`
   - This command checks again to confirm that the new swap file is active.

8. **Check memory usage again:**
   - `free -h`
   - Finally, use this command again to see the updated memory and swap usage.
