*MH Danh sách món ăn:
- lưu các món ăn được nhập vào với các thông tin: 
	string tên, 
	float giá tiền, 
	string hình ảnh (lưu ảnh trên drive, lưu url vào db, nếu dính tới bảo mật vd ngại lộ key drive thì sẽ chuyển lại lưu truyền thống), 
	string phân loại món ăn (user tự tạo các phân loại (vd: cơm, bún, ăn vặt,...); có thể thêm, xóa, sửa thông tin một phân loại ngay trên list lúc chọn phân loại), 
	list pair?<danh sách nguyên liệu, số lượng>, 
	string công thức chế biến, 
	list pair?<danh sách dinh dưỡng, số lượng> (vd calo: 100 kcal), string tung độ, string hoành độ
	string địa chỉ, 
	string sđt đặt hàng, 
	datetime lịch sử các thời điểm ăn, 
	bool isFavourite, 
	int mức độ no (1-5), 
	string đoạn cảm nhận
- hỗ trợ ấn nút gọi nếu có món ăn có sdt đặt hàng (item nào ko có sdt thì nút làm mờ nút gọi)
- nút Thêm vào giỏ đi chợ: danh sách nghiên liệu nấu ăn được thêm tự động vào MH giỏ đi chợ
- hỗ trợ hiển thị các món ăn theo các view lớn theo từng phân loại món ăn, trong mỗi view hỗ trợ các kiểu lọc: chưa ăn lâu nhất; ds theo giá tiền; ds yêu thích;…
(có thể load thông tin item trước, load ảnh sau để giảm thời gian chờ)
 
- danh sách món ăn user tự nhập, 
- các user có thể share ds với nhau: 
+ nút follow ở trang cá nhân: khi người được follow thêm món ăn thì có thông báo tới người follow, 
+ user có thể set public hoặc private danh sách món ăn của mình

*MH Lịch sử ăn
- có thể đính kèm ảnh chụp + dòng status vào món ăn sắp thêm vào lịch sử
- tích hợp thống kê chi phí của lịch sử ăn uống
- user có thể set public hoặc private

*MH giỏ đi chợ: danh sách các thứ cần mua (tương tự todo list)
- danh sách nghiên liệu nấu ăn được thêm tự động khi user chọn món trong MH danh sách và chọn option Thêm vào giỏ đi chợ
- tích hợp tính chi phí

*MH thống kê các chất dinh dưỡng đã tiêu thụ (vd calo, đạm)
- thống kê theo ngày/tuần/tháng/năm các chất dinh dưỡng đã tiêu thụ dựa trên lịch sử ăn uống

