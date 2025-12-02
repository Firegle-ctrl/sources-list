## 自动使用 Debian 13 Trixie 源

```sh
# 备份原有源列表文件
sudo cp /etc/apt/sources.list /etc/apt/sources.list.bak

# 下载新的 Debian 13 Trixie 源列表（需确保已安装 wget，或使用 PowerShell 时的 wget/Invoke-WebRequest）
wget "https://raw.githubusercontent.com/Firegle-ctrl/apt-sources-list/main/debian13trixie" -O Debian13Trixie.txt

# 替换系统源列表为新文件
sudo cp Debian13Trixie.txt /etc/apt/sources.list
```
