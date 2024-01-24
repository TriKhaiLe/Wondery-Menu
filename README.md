*MH Danh sách món ăn:
- lưu các món ăn được nhập vào với các thông tin: 
	string tên, 
	float giá tiền, 
	string hình ảnh (lưu ảnh trên drive, lưu url vào db, nếu dính tới bảo mật vd ngại lộ key drive thì sẽ chuyển lại lưu truyền thống), 
	string phân loại món ăn (user tự tạo các phân loại (vd: cơm, bún, ăn vặt,...); có thể thêm, xóa, sửa thông tin một phân loại ngay trên list lúc chọn phân loại), 
	list pair?<danh sách nguyên liệu, số lượng>, 
	string công thức chế biến, 
	string địa chỉ, 
	string sđt đặt hàng, 
	datetime lịch sử các thời điểm ăn, 
	bool isFavourite, 
	int mức độ no (1-5), 
	string đoạn cảm nhận
- hỗ trợ nút gọi ngay trên list item (làm mờ nút gọi nếu item nào sdt == null)
- hỗ trợ hiển thị các món ăn theo các collection, mỗi collection có các view theo từng phân loại món ăn, trong mỗi view hỗ trợ các kiểu lọc: chưa ăn lâu nhất; ds theo giá tiền; ds yêu thích;…
(có thể load thông tin item trước, load ảnh sau để giảm thời gian chờ). Sơ đồ minh họa:
![image](https://github.com/TriKhaiLe/Wondery-Menu/assets/108702049/3e034c20-4f61-4374-9000-595e6c8dce79)

- danh sách món ăn user tự nhập, 
- các user có thể share ds với nhau: 
+ user có thể set public hoặc private danh sách món ăn của mình
+ khi sang xem list của user khác, hỗ trợ option clone món ăn về list của mình

*MH Lịch sử ăn
- có thể đính kèm ảnh chụp + dòng status vào món ăn sắp thêm vào lịch sử
- tích hợp thống kê chi phí của lịch sử ăn uống
- user có thể set public hoặc private

*MH thông tin cá nhân:
- avatar, tên, số lượng món ăn, số lượt follow
- nút follow ở trang cá nhân: khi người được follow thêm món ăn thì có thông báo tới người follow, 
- icon chuông xem thông báo khi người khác thêm món ăn, khi ấn vào navigate tới món ăn đó của user vừa thêm

