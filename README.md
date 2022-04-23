# gitskills
This repository is used to learn how to clone repo from remote host.
Git is a free software...
I do some change in local repo and pull it to remote online repo in main branch.
And I make some effort to make the issue start again.

iptables -t nat -A POSTROUTING -o wlp0s20f3 -s 192.168.1.0/24 -j MASQUERADE
iptables -A FORWARD -i usb0 -o wlp0s20f3 -m state --state RELATED,ESTABLISHED -j ACCEPT
iptables -A FORWARD -i usb0 -o wlp0s20f3 -j ACCEPT

echo "1" > /proc/sys/net/ipv4/ip_forward
iptables -t nat -A POSTROUTING -o wlp0s20f3 -s 192.168.1.0/24 -j MASQUERADE
iptables -A FORWARD -i usb0 -o wlp0s20f3 -m state --state RELATED,ESTABLISHED -j ACCEPT
iptables -A FORWARD -i usb0 -o wlp0s20f3 -j ACCEPT

# you must put these two stences in before ping
route add default gw 192.168.1.223 dev usb0
systemctl restart systemd-resolved.service

scp -r $HOME/projects/samples HwHiAiUser@192.168.1.2:/home/HwHiAiUser/projects/samples

cd $HOME/projects/samples/
export DDK_PATH=$HOME/Ascend/ascend-toolkit/latest/arm64-linux/
export NPU_HOST_LIB=$DDK_PATH/acllib/lib64/stub
cd $HOME/projects/samples/cplusplus/level1_single_api/5_200dk_peripheral/ascendcamera
cd build/intermediates/host/
make clean
cmake ../../../src -DCMAKE_CXX_COMPILER=aarch64-linux-gnu-g++ -DCMAKE_SKIP_RPATH=TRUE
export INSTALL_DIR=${HOME}/Ascend/ascend-toolkit/latest

how could git diff --cached work?
still don't have any change?
