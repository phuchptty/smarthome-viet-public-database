# Tác Giả

- Bài viết của bạn: [Bùi Sỹ Hải Đăng](https://www.facebook.com/www.quangminh.vn) và [yansign8x](https://miui.vn/forum/members/yansign8x.22571/) của [MIUI VN](http://miui.vn/)
- Bài viết trong group [Smarthome Việt](https://www.facebook.com/groups/784535325063755/permalink/1055647511285867/)
- Bài viết trên [MIUI VN](https://miui.vn/forum/threads/padavan-custom-firmware-qos-iptv-transmission-for-xioami-router-gen3-gen3g-mini-nano.24161/)

# Hướng Dẫn

  1. Up rom padavan theo hướng dẫn này: 
    Đọc kỹ phần "Với R3G" ở dưới bài nhé.
    Chú ý: Up firmware DEV này trước rồi mới up được SSH nhé. 

    2. Kích hoạt entware: https://bitbucket.org/…/rt-n…/wiki/EN/HowToConfigureEntware…
    
    3. Cài debian: https://github.com/…/w…/Installing-Debian-chroot-environment
    Tới đây để ý chút, bản debian chỉ có Python 3.4, mà 1 thành phần trong hass nó đòi Python 3.5 trở lên. Nên phải sửa lại chút để có Python 3.7
    Edit \opt\debian\etc\apt\sources.list, thay bằng đoạn này
    deb http://ftp.de.debian.org/debian testing main
    Sau đó apt-get update và làm tiếp.
    
    4. Install HASS: https://www.home-assistant.io/docs/installation/virtualenv/
    
    5. Thiết lập HASS chạy như service để auto start mỗi lần reboot.
