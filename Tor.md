## Install Tor in Fedora

1. **Configure Tor Package Repository:**
   - Add the following content to `/etc/yum.repos.d/tor.repo`:
     ```
     [tor]
     name=Tor for Fedora $releasever - $basearch
     baseurl=https://rpm.torproject.org/fedora/$releasever/$basearch
     enabled=1
     gpgcheck=1
     gpgkey=https://rpm.torproject.org/fedora/public_gpg.key
     cost=100
     ```

2. **Install the Tor Package:**
   ```
   sudo dnf install tor
   ```

### Update, Start, and Stop Tor

1. **Update Tor:**
   ```
   sudo dnf upgrade tor
   ```

2. **Start Tor:**
   ```
   sudo systemctl start tor
   ```

3. **Stop Tor:**
   ```
   sudo systemctl stop tor
   ```

4. **Check the Status of Tor:**
   ```
   sudo systemctl status tor
   ```

5. **Enable Tor to Start at Boot:**
   ```
   sudo systemctl enable tor
   ```

6. **Disable Tor from Starting at Boot:**
   ```
   sudo systemctl disable tor
   ```

These steps will help you install and manage the Tor service on a Fedora system.
