# TP_LVM


    1  cd
    2  lsblk
    3  pvcreate /dev/sdc /dev/sdd /dev/sde
    4  pvs
    5  vgcreate datos /dev/sdc /dev/sdd /dev/sde
    6  vgs
    7  lvcreate -L 1G -n www datos
    8  lvcreate -L 4G -n salvas datos
    9  lvs
   10  df -h
   11  lvresize -L 2G /dev/datos/www
   12  lvresize -l +100%FREE /dev/datos/www
   13  lvs
   14  history > history.txt

