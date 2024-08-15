# notebookUbuntu
## resize LVM
sudo vgdisplay ubuntu-vg
Tìm dòng "Free PE / Size" để xem dung lượng trống còn lại trong Volume Group.
sudo lvextend -l +100%FREE /dev/ubuntu-vg/ubuntu-lv
Nếu bạn đang sử dụng hệ thống tập tin ext4
sudo resize2fs /dev/ubuntu-vg/ubuntu-lv
sudo xfs_growfs /
