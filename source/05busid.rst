05busid 故障 gpu 显卡槽位
============================================

#. 执行命令 ``nvidia-smi`` ::

    Fri Aug 16 15:47:10 2024
    +-----------------------------------------------------------------------------------------+
    | NVIDIA-SMI 550.76                 Driver Version: 550.76         CUDA Version: 12.4     |
    |-----------------------------------------+------------------------+----------------------+
    | GPU  Name                 Persistence-M | Bus-Id          Disp.A | Volatile Uncorr. ECC |
    | Fan  Temp   Perf          Pwr:Usage/Cap |           Memory-Usage | GPU-Util  Compute M. |
    |                                         |                        |               MIG M. |
    |=========================================+========================+======================|
    |   0  NVIDIA GeForce RTX 4090 D      On  |   00000000:16:00.0 Off |                  Off |
    |  0%   45C    P8             25W /  425W |       2MiB /  24564MiB |      0%      Default |
    |                                         |                        |                  N/A |
    +-----------------------------------------+------------------------+----------------------+
    |   1  NVIDIA GeForce RTX 4090 D      On  |   00000000:34:00.0 Off |                  Off |
    |  0%   37C    P8             20W /  425W |       2MiB /  24564MiB |      0%      Default |
    |                                         |                        |                  N/A |
    +-----------------------------------------+------------------------+----------------------+
    |   2  NVIDIA GeForce RTX 4090 D      On  |   00000000:52:00.0 Off |                  Off |
    |  0%   40C    P8             17W /  425W |       2MiB /  24564MiB |      0%      Default |
    |                                         |                        |                  N/A |
    +-----------------------------------------+------------------------+----------------------+
    |   3  NVIDIA GeForce RTX 4090 D      On  |   00000000:CA:00.0 Off |                  Off |
    | 30%   44C    P2            223W /  425W |   16108MiB /  24564MiB |     99%      Default |
    |                                         |                        |                  N/A |
    +-----------------------------------------+------------------------+----------------------+

    +-----------------------------------------------------------------------------------------+
    | Processes:                                                                              |
    |  GPU   GI   CI        PID   Type   Process name                              GPU Memory |
    |        ID   ID                                                               Usage      |
    |=========================================================================================|
    |    3   N/A  N/A     15863      C   PWmat                                       16100MiB |
    +-----------------------------------------------------------------------------------------+

#. 以序号 :green:`3` 为例, 记录 3 号显卡 Bus-Id :green:`00000000:CA:00.0` ::

    dmidecode -t slot | grep -i -10 CA:00.0
    Handle 0x000D, DMI type 9, 17 bytes
    System Slot Information
    	Designation: CPU SLOT1 PCIe 5.0 X16
    	Type: x16 <OUT OF SPEC>
    	Current Usage: In Use
    	Length: Long
    	Characteristics:
    		3.3 V is provided
    		Opening is shared
    		PME signal is supported
    	Bus Address: 0000:ca:00.0

   3 号显卡对应服务器主板 PCI插槽槽位是 :blue:`Designation: CPU SLOT1 PCIe 5.0 X16`

-----

#. gpu 卡对应型号

pci.ids: https://github.com/pciutils/pciids/blob/master/pci.ids ::

    # lspci -nn | grep VGA
    # lspci | grep NVIDIA
    02:00.0 VGA compatible controller: NVIDIA Corporation Device 2204 (rev a1)   # 3090
    02:00.0 VGA compatible controller: NVIDIA Corporation Device 2208 (rev a1)   # 3080ti
    1a:00.0 3D controller: NVIDIA Corporation GP100GL [Tesla P100 SXM2 16GB] (rev a1)   # p100
    02:00.0 VGA compatible controller: NVIDIA Corporation GP102 [GeForce GTX 1080 Ti] (rev a1)   # 1080ti
    31:00.0 VGA compatible controller [0300]: NVIDIA Corporation Device [10de:2684]  # NVIDIA GeForce RTX 4090
