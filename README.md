Nguồn #JapanTools V3.0
# Ngày 1/1/2020 0h00'000
#########################
### TỰ ĐỘNG NHẬN PROXIES ###
### QUY TRÌNH KIỂM TRA TRỰC TIẾP ###
### Http proxy / Https ###
### Sock4 / Sock5 Live ###
#########################
##################################################### #############################
## =============================== README.TXT ============== ================== ##
## ============ HƯỚNG DẪN SỬ DỤNG CÔNG CỤ HIỆU QUẢ NHẤT ================= ##
## * TRONG LOẠI PROXY: ##
## - Trong Máy chủ Khác, Chúng tôi sử dụng Proxy Http whit [ https://victim.com ] sẽ chết ###
## - Máy chủ khác, Chúng tôi sử dụng Proxy Https [ http://victim.com ] sẽ chết ###
## - Hoặc có thể chúng ta có thể sử dụng Proxy Http, Https, Socks4, Socks5 whit Victim ###
## - DANH SÁCH MỘT PROXY PHẢI ĐẦY ĐỦ, (PHẢI HƠN 100 PROXY TRONG DANH SÁCH) ##
## - BẠN PHẢI ĐƯỢC KIỂM TRA TOÀN BỘ VÀ NHẬN PROXY TRỰC TIẾP ĐỂ CÔNG CỤ LÀM VIỆC HIỆU QUẢ ####
## - NẾU DANH SÁCH PROXY ÍT HƠN 100 PROXY, IN CHỈ SỐ LỖI IN NGOÀI RANGE #
## - NÊN LOẠI BỎ PROXY DUPLICATE VÀ GIỮ PROXY CÓ THỜI GIAN NGOÀI = <1 #
## - DANH SÁCH PROXY TỪ NHIỀU NGUỒN MIỄN PHÍ KHÔNG THỂ CÓ VỚI PROXY VIP CỦA BẠN. ##
## - Thứ tự của Loại Proxy được ưu tiên sử dụng để có hiệu suất tốt nhất là: ##
## ---> Loại proxy SOCK4 - HTTP- SOCK5- HTTPS (SSL Proxy) <--- ##
## - NẾU CHỌN LOẠI PROXY HTTP-HTTPS SẼ LÀ GIẢ: ĐỊA CHỈ MAC VÀ IP ##
## SỰ KẾT HỢP GIỮA LOẠI PROXY VÀ PHƯƠNG PHÁP CÔNG CỤ ĐỂ VẬN HÀNH HIỆU QUẢ #
## - Thứ tự của CÔNG CỤ PHƯƠNG PHÁP được ưu tiên để có hiệu suất tốt nhất là: ##
## ---> Loại Phương thức [1] - [3] - [2] - [4] - [5] - [6] <--- ##
## - CÔNG CỤ TRONG PHƯƠNG PHÁP: ##
## + NẾU BẠN CHỌN [1] HttpFlood (Mặc định): ##
## ---> URL MỤC TIÊU: [ http://domain.com ] HOẶC [ http://192.168.1.127:80 ] ##
## ---> PHẢI CÓ CỔNG 80 HOẶC KHÔNG CÓ CỔNG TRONG MỤC TIÊU [ http://192.168.1.127 ] ##
## ---> LOẠI PROXY (Thứ tự ưu tiên): SOCK4 -SOCK5 -HTTP -HTTPS #
## + NẾU BẠN CHỌN [2] CloudFlare (Mặc định): ##
## ---> URL MỤC TIÊU: [ http://domain.com ] HOẶC [ http://192.168.1.127:80 ] ##
## ---> PHẢI CÓ CỔNG 80 HOẶC KHÔNG CÓ CỔNG TRONG MỤC TIÊU [ http://192.168.1.127 ] ##
## ---> LOẠI PROXY (Thứ tự ưu tiên): SOCK4 -SOCK5 -HTTP -HTTPS #
## ---> PHƯƠNG PHÁP CHỈ CÓ VỚI LOẠI URL CF ĐƠN GIẢN NHẤT (KHÔNG PHẢI UAM) #
## + NẾU BẠN CHỌN [3] HttpFlood (Sockets): ##
## ---> URL MỤC TIÊU: [ http://domain.com ] HOẶC [ http://192.168.1.127:80 ] ##
## ---> PHẢI CÓ CỔNG 80 HOẶC KHÔNG CÓ CỔNG TRONG MỤC TIÊU [ http://192.168.1.127 ] ##
## ---> LOẠI PROXY (Thứ tự ưu tiên): SOCK4 -SOCK5 -HTTP -HTTPS #
## ---> TẠO YÊU CẦU HƠN LOẠI KHÁC NẾU SỬ DỤNG LOẠI SOCK4 #
## + NẾU BẠN CHỌN [4] CloudFlare (Cookie): ##
## ---> URL MỤC TIÊU: [ http://domain.com ] HOẶC [ http://192.168.1.127:80 ] ##
## ---> PHẢI CÓ CỔNG 80 HOẶC KHÔNG CÓ CỔNG TRONG MỤC TIÊU [ http://192.168.1.127 ] ##
## ---> LOẠI PROXY (Thứ tự ưu tiên): SOCK4 -SOCK5 -HTTP -HTTPS #
## ---> CHỈ SỬ DỤNG CHO MỤC TIÊU NẤU ĂN VÀ CÓ MỤC TIÊU NẤU ĂN #
## + NẾU BẠN CHỌN [5] Tìm IP-CF (--- SSH) HOẶC [6] Kiểm tra IP-CF (--- DNS): ##
## ---> URL MỤC TIÊU: [ http://domain.com ] HOẶC [ http://192.168.1.127:80 ] ##
## ---> PHẢI CÓ CỔNG 80 HOẶC KHÔNG CÓ CỔNG TRONG MỤC TIÊU [ http://192.168.1.127 ] ##
## ---> LOẠI PROXY (Thứ tự ưu tiên): SOCK4 -SOCK5 -HTTP -HTTPS #
## ---> LỰA CHỌN CỦA BẠN ĐỂ LỰA CHỌN [5] VÀ [6] ##
## ------- ĐỂ CÔNG CỤ LÀM VIỆC TỐT NHẤT CẦN MÁY TÍNH VÀ MẠNG SỨC KHỎE, -------- #
## --- SỐNG NHIỀU PROXY, KIẾN THỨC SỬ DỤNG CÔNG CỤ VÀ HIỂU BIẾT VỀ MỤC TIÊU ---- #
## ---- NÊN SỬ DỤNG VPS MẠNH MẼ NHẤT. TÔI LUÔN CẬP NHẬT CÁC CÔNG CỤ MÃ NGUỒN .----- #
## ============== CÁC BẠN ĐÃ XEM VÀ SỬ DỤNG CÔNG CỤ !!! =================
## BẢN QUYỀN TRÊN P3TERJ4MES, MÃ NGUỒN CỦA P3TERJ4MES, CẤM BẢN SAO, #
## MUA HÀNG, CHỈNH SỬA MÃ DƯỚI MỌI HÌNH THỨC KHI CHƯA ĐƯỢC SỰ CHO PHÉP CỦA CHỦ SỞ HỮU HỢP PHÁP !!! #
## Bản quyền © 2015-2020 JAPANTOOLS. Thiết kế bởi P3TERJ4MES ##
## =============================== README.END ============== ================== ##
##################################################### #############################
