تغییر مسیر کش APT 
mkdir -p /tmp/apt-cache
echo 'Dir::Cache::archives "/tmp/apt-cache";' > /etc/apt/apt.conf.d/99customcache
apt-get update && apt-get install -y nano && apt-get clean
