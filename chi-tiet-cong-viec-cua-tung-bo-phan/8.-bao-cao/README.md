# 8. BÁO CÁO

Báo cáo được cài đặt tùy chỉnh theo từng yêu cầu riêng của công ty vận tải. Báo cáo được phân loại theo:

* Báo cáo tổng hợp
* Báo cáo Trucking
* Báo cáo kho- sửa chữa
* Báo cáo dầu

### **8.1 Báo cáo tổng hợp** <a href="#_22vxnjd" id="_22vxnjd"></a>

#### **8.1.1 Báo cáo Doanh thu chi phí theo xe (DTCP)** <a href="#_i17xr6" id="_i17xr6"></a>

Báo cáo Doanh thu chi phí theo xe là bảng tổng hợp thông tin lấy dữ liệu trong các bảng của mục: Điều hành, Kế toán, Sửa chữa, Nhiên liệu để tổng hợp chi phí theo từng xe. Gồm có:

* Báo cáo chi tiết: Chi tiết từng chuyến hàng theo xe, chi phí trên từng chuyến
* Báo cáo tổng hợp: Tổng hợp chi phí của xe trên tất cả các chuyến vận chuyển

**8.1.1.1 Mẫu 1- mẫu chung**

![](<../../.gitbook/assets/0 (1).png>)

_Màn hình Chi tiết Bc Doanh thu chi phí theo xe_

![](../../.gitbook/assets/1.png)

_Màn hình Tổng hợp Bc Doanh thu chi phí theo xe_

| Lượng giao/ Lượng nhận | Lượng lái xe giao / Lượng lái xe nhận                                                                         |
| ---------------------- | ------------------------------------------------------------------------------------------------------------- |
| Lượng hao hụt          | Lượng Giao - Nhận                                                                                             |
| DT vận tải bộ          | Cước thực thu trong Ql cước vc (= Định mức cước – Chiết khấu)                                                 |
| Lưu ca                 | Tổng tiền lưu ca trong Ql cước vc                                                                             |
| Nhiên liệu             | Tổng tiền nhiên liệu trong Ql chi phí vc (mặc định= (lượng dầu ĐM + Bổ sung) x Đơn giá định mức -lấy từ TTC)  |
| Chi phí đi đường       | Tổng tiền đường trong Ql chi phí vc                                                                           |
| Lương LX               | Lương khai báo trong bảng Nhân viên (k bao gồm phụ cấp, ...)                                                  |
| Sửa chữa               | Tổng chi phí các hóa đơn sửa chữa của xe trong tháng                                                          |
| Đăng kiểm & lưu thông  | (Phí đăng kiểm + dịch vụ) + Phí lưu thông đường bộ cho xe và mooc được gán cho xe                             |
| Bảo hiểm               | Bảo hiểm Trách nhiệm dân sự + Bảo hiểm vật chất                                                               |
| Ngân hàng              | Vay ngân hàng + Lãi ngân hàng                                                                                 |
| Định vị                | Phí định vị + Phí camera                                                                                      |
| Chi phí khác           | Các khoản phí thường niên còn lại                                                                             |
| Lợi nhuận              | (DTVT bộ + Lưu ca) - Chi phí xe                                                                               |

**8.1.1.2 Mẫu 2 – Dùng cho điều xe ghép**

![](../../.gitbook/assets/2.png)

![](<../../.gitbook/assets/3 (2).png>)

_Màn hình báo cáo DTCP theo xe_

| Ngày đi                                   | Ngày xe đi                                                                                                                                                                     |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Tuyến đường                               | Điểm đến trong KHĐX                                                                                                                                                            |
| <p>Vé/ Sửa rửa/ Dầu</p><p>Ăn/ Công an</p> | Thông tin tiền đường trong Điều xe ghép                                                                                                                                        |
| Bốc vác                                   | Tiền phát sinh, nhập trong Đx ghép- phần thông tin tiền đường                                                                                                                  |
| Bồi dưỡng                                 | Chi phí khác, nhập trong Đx ghép- phần thông tin tiền đường                                                                                                                    |
| Tổng DT                                   | = Cước thực thu + phát sinh (ô nhập bên cạnh Cách tính cước)                                                                                                                   |
| Tổng Chi phí                              | = Tổng CP                                                                                                                                                                      |
| Đền Hao hụt                               | = \[(lượng nhận - lượng giao)- (lượng nhận x %hao hụt)] x Giá đền bù                                                                                                           |
| Đền tiền hàng                             | <p>= Tiền hàng trong bảng lương lái xe (Chính là tiền đền bù gà yếu, chết)</p><p>= Đơn giá bù * Lái xe chịu (Nhập chi tiết trong Tiền hàng)</p>                                |
| Lợi nhuận \_ Dầu không theo chuyến        | Tổng lượng Dầu cấp theo xe trong tháng                                                                                                                                         |
| Lợi nhuận \_ Sửa xe k theo chuyến         | Tổng tiền các hóa đơn sửa chữa của xe trong tháng (theo ngày sửa)                                                                                                              |
| Phí khác                                  | Phí thường niên hàng tháng của xe                                                                                                                                              |
| Lợi nhuận xe                              | = Tổng DT - (Tổng chi phí + Đền hao hụt + Đề tiền hàng + Dầu k theo chuyến + Sửa xe k theo chuyến + Phí khác)                                                                  |
| % lái xe hưởng                            | Theo khai báo Lợi nhuận trong Đx ghép                                                                                                                                          |
| Vận chuyển                                | = (Cước + Phát sinh- Đền hao hụt - Đền tiền hàng) x % lx hưởng                                                                                                                 |
| Hao hụt                                   | = Đền hao hụt lô hàng                                                                                                                                                          |
| Dầu k theo chuyến                         | = Lợi nhuận \_ Dầu không theo chuyến                                                                                                                                           |
| Sửa k theo chuyến                         | <p>Tổng các hóa đơn sửa xe trong tháng tính theo CT sau</p><p>HĐ &#x3C;1 triệu: Tính toán bộ cho lái xe</p><p>HĐ > 1 triệu: Lái xe chịu = 1 triệu + (Hóa đơn - 1 triệu)/ 2</p> |
| VETC                                      | = Tổng VETC trong tháng (nhập tại Quản lý phí thường niên)                                                                                                                     |
| Lái xe \_ Lợi nhuận                       | = Tổng thu - (Tổng CP + VETC + Dầu k theo chuyến + Sửa xe k theo chuyến)                                                                                                       |
| Phí thường niên                           | = Tổng các phí thường niên của xe trong tháng (trừ VETC đã tính cho Lxe)                                                                                                       |
| Cước thu                                  | = (Cước + Phát sinh - Đền hao hụt - Đền tiền hàng)\* (100%- % lái xe hưởng)                                                                                                    |
| Hỗ trợ sửa xe                             | <p>HĐ > 1 triệu </p><p>= (Hóa đơn - 1 triệu)/ 2</p><p>= Sửa chữa k theo chuyến (Lợi nhuận) - Sửa chữa k theo chuyến (Lái xe) </p>                                              |
| Lợi nhuận                                 | = Cước thu - (Phí thường niên + Hỗ trợ sửa xe)                                                                                                                                 |

*
  *
    *
      1. **Báo cáo bộ phận thống kê**

![](<../../.gitbook/assets/4 (1).png>)

![](<../../.gitbook/assets/5 (2).png>)

![](<../../.gitbook/assets/6 (4).png>)_Màn hình Báo cáo bộ phận thống kê_

| Mã KH                         | Lấy từ cột Mã đối tác trong Quản lý đối tác - TTC             |
| ----------------------------- | ------------------------------------------------------------- |
| Khách hàng                    | Tên đầy đủ của khách hàng, link từ bảng Quản lý đối tác - TTC |
| Mã chuyến ghép                | Link từ cột Mã chuyến ghéo trong Điều xe                      |
| Tên hàng                      | Lấy từ Quản lý hàng hóa – TTC, link từ Qly lô hàng            |
| Số book/bill                  | Lấy theo số vận đơn/ booking trong Quản lý lô hàng            |
| Loại cont                     | Loại cont của chuyến                                          |
| Hàng nhập/xuất                | Loại hàng xuất/ nhập/ nội địa trong Quản lý lô hàng           |
| Điểm lấy hàng/đóng hàng       | Link từ Kế hoạch vận chuyển                                   |
| Điểm giao hàng/nhận hàng      | Link từ Kế hoạch vận chuyển                                   |
| Điểm hạ vỏ/lấy vỏ             | Link từ Kế hoạch vận chuyển                                   |
| Cảng xuất                     | Link từ Quản lý lô hàng                                       |
| Số cont                       | Số cont của chuyến xe                                         |
| Số seal                       |                                                               |
| Số tờ khai                    | Link từ Quản lý lô hàng                                       |
| Ngày xe chạy                  | Ngày vận chuyển trong Kế hoạch điều xe                        |
| Thời gian nhận hàng           | Link từ app mobile, sau khi lái xe tích nhận hàng             |
| Thời gian giao hàng           | Link từ app mobile, sau khi lái xe tích giao hàng             |
| Tổng thời gian giao nhận hàng | = Thời gian giao hàng – Thời gian nhận hàng                   |
| Số xe                         | Link từ Điều xe                                               |
| Tuyến đường                   |                                                               |
| Số phiếu dầu                  |                                                               |
| Dầu ĐM                        | Link từ cột ĐM dầu trong Quản lý chi phí vận chuyển           |
| Bù trừ dầu                    |                                                               |
| Dầu thực tế                   | Link từ Quản lý dầu cấp cho xe                                |
| Vé chuyến                     | Tiền vé trong Quản lý chi phí vận chuyển                      |
| Lương chuyến                  | Ca xe trong Quản lý chi phí vận chuyển                        |
| Đi đường                      |                                                               |
| Vé cao tốc                    | Vé cao tốc PS trong Quản lý chi phí vận chuyển                |
| CP phát sinh                  |                                                               |
| Tổng chi phí                  | Tiền đường trong Quản lý chi phí vận chuyển                   |
| Lưu ca                        | Tổng tiền lưu ca trong Ql cước vc                             |
| Ghi chú                       |                                                               |

#### **8.1.2 Báo cáo lô hàng** <a href="#_320vgez" id="_320vgez"></a>

Tổng hợp các chi phí làm hàng theo lô, bao gồm: chi phí hải quan, chi trả hộ, thu chi từ lái xe, cước vận chuyển, cược vỏ, lưu ca, …; Tính toán chênh lệch trong QTNB và QTKH.

Báo cáo lô hàng được tự động cập nhật khi người dùng có các thay đổi số liệu chi phí chuyến hàng ở các tác vụ khác: Cập nhật chi phí chi, trả hộ; Cập nhật thông tin lưu ca; Cập nhật thông tin cược vỏ, Cập nhật thu chi lái xe.

![](<../../.gitbook/assets/7 (2).png>)

_Màn hình Báo cáo lô hàng_

| Điều kiện hiển thị  | Tạo tạm ứng lô hàng từ Quản lý lô hàng đủ/ rút gọn                                                                                                                                                                         |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Nội dung chi phí    | <p>- Các chi phí trong tạm ứng lô hàng </p><p>- Cước các chuyến vận chuyển của lô (Thực tế theo cước thực thu, KH theo cước HĐ), Lưu ca của lô – Theo Ql cước vc và QTKH.</p><p>- Chi phí trong Quản lý thu chi lái xe</p> |
| Ngày thực hiện      | <p>- Chi phí tạm ứng - Ngày tạo tạm ứng </p><p>- Cước + lưu ca: Ngày điều xe</p><p>- Chi phí thu chi lái xe: Ngày nhập phí</p>                                                                                             |
| Ghi chú             | Ghi chú của Điều xe và tạm ứng lô hàng.                                                                                                                                                                                    |

#### **8.1.3 Thanh toán khách hàng** <a href="#_1h65qms" id="_1h65qms"></a>

**8.1.3.1 Quyết toán chi hộ**

![](<../../.gitbook/assets/8 (8).png>)

| Điều kiện hiển thị        | Tìm kiếm theo ngày tạo lô/ ngày thanh toán, có tạm ứng                      |
| ------------------------- | --------------------------------------------------------------------------- |
| Ghi chú                   | Ghi chú QTKH (hoặc từ tạm ứng/ QTNB)                                        |
| Ngày TK                   |                                                                             |
| Bill/ Booking             | Lấy theo số vận đơn/ booking trong Quản lý lô hàng                          |
| Ngày tạo lô               | Ngày tạo lô hàng                                                            |
| Tờ khai hải quan/ số cont | Số tờ khai/ số cont được khai báo ở Qly lô hàng                             |
| Hàng, Loại cont           | Loại hàng xuất/ nhập/ nội địa; loại hàng cont 20, 40,... trong Ql lô hàng   |
| Trị giá hóa đơn           | theo Thành tiền trong QTKH                                                  |
| Mã lô                     | Mã lô được tạo tạI Qly lô hàng                                              |
| Nội dung                  | Các chi phí Chi trả hộ trong QTKH                                           |
| Ngày thanh toán           | Ngày tích thanh toán trong Tạm ứng lô hàng/ Quản lý tạm ứng- tab Thanh toán |
| Ngày hóa đơn              | Ngày hóa đơn trong Tạm ứng lô hàng/ Quản lý tạm ứng- tab Thanh toán         |
| Số hóa đơn                | Nhập tại cột hóa đơn ở Quyết toán theo KH                                   |
| Trị giá hóa đơn           | Là số thành tiền của các phí trong bảng                                     |

**8.1.3.2 Bảng kê thanh toán cước**

![](<../../.gitbook/assets/9 (7).png>)

| Ngày                   | Ngày điều xe, tìm kiếm phụ thuộc vào ngày điều xe, dữ liệu chạy theo Ql cước vc                                                                                                                        |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Diễn giải              | <p>Tuyến đường lấy theo điểm Mở rộng - Chi tiết </p><p>TH phát sinh chuyển điểm: thêm 1 dòng ghi điểm phát sinh </p>                                                                                   |
| Lượng giao, Lượng nhận | Lấy theo Ql cước vc. Lượng giao= Lượng lx giao, Lượng nhận= Lượng lx nhận                                                                                                                              |
| Chênh lệch             | = Lượng nhận - Lượng giao                                                                                                                                                                              |
| Đơn giá                | Đơn giá HĐ, theo Ql cước vc                                                                                                                                                                            |
| Tiền cước              | Cước HĐ                                                                                                                                                                                                |
| Phát sinh cước         | phát sinh cước HĐ khi chuyển điểm+ Lưu ca                                                                                                                                                              |
| Phí dịch vụ            | <p>Chạy từ phí dịch vụ thông quan trên QTKH: </p><p>Hàng cont: lấy đơn giá * Số lượng cont của chuyến (Đơn vị Cont 20, cont 40)</p><p>Hàng rời: Đơn giá * Trọng lượng nhận của chuyến (đơn vị tấn)</p> |
| Cộng                   | = Tiền cước + Phát sinh cước + Phí dịch vụ                                                                                                                                                             |
| Ghi chú                | Số cont từ điều xe                                                                                                                                                                                     |

**8.1.3.3 Bảng kê cước vận chuyển**

![](<../../.gitbook/assets/10 (2).png>)

| Ngày          | Ngày tạo lô                                                             |
| ------------- | ----------------------------------------------------------------------- |
| Tìm kiếm      | Ngày điều xe                                                            |
| Số xe         | theo Điều xe                                                            |
| Diễn giải     | Tuyến đường lấy theo điểm Mở rộng - Chi tiết                            |
| Số container  | Số cont từ điều xe                                                      |
| Loại lô hàng  | Loại hàng xuất/ nhập/ nội địa trong Ql lô hàng                          |
| Phí chi hộ    | =Tổng chị trả hộ (QTKH)/ số chuyến của lô (làm tròn đến hàng nghìn VNĐ) |
| Tiền VC       | = Thành tiền cước HĐ + Phát sinh cước HĐ (chưa bao gồm Lưu ca 9/11)     |
| Tổng          | = Phí chi hộ + Tiền vận chuyển                                          |
| Ghi chú       | Loại cont (20’, 40’...)                                                 |

**8.1.3.4 Bảng đối chiếu cước vận chuyển**

![](../../.gitbook/assets/11.png)

| Ngày                          | Ngày tạo/ sửa lô                                                        |
| ----------------------------- | ----------------------------------------------------------------------- |
| Số xe                         | Số xe đã chọn khi tạo điều xe                                           |
| Diễn giải                     | Tuyến đường trong điều xe (tuyến đầu tiên, không tính chuyển điểm)      |
| Mã lô                         | Mã lô đã tạo trong Qly lô hàng                                          |
| Bill                          | Lấy theo số vận đơn/ booking trong Quản lý lô hàng                      |
| Lượng giao                    | Lượng giao khi khai báo ở Điều xe                                       |
| Làm luật                      | Phí kẹp quá tải của Phí chi trả hộ theo thuyến - Qly chi phí vận chuyển |
| Chi phí phát sinh theo chuyến | bỏ                                                                      |
| Chi phí khác                  | bỏ                                                                      |
| Chi phí phát sinh tiền đường  | bỏ                                                                      |
| Tổng cước VC (chưa VAT)       | Cước TT - Qly cước VC                                                   |
| VAT                           |                                                                         |
| Tổng                          | bỏ                                                                      |
| Lượng nhận                    | Lượng nhận được khai báo khi điều xe                                    |
| Số cont                       | Số cont của chuyến xe                                                   |
| Cont/ Chuyến                  | (Các) loại cont của chuyến                                              |
| Tiền cước                     | Tiền cước HĐ                                                            |
| Phí nâng hàng                 |                                                                         |
| Phí hạ hàng                   |                                                                         |
| Phát sinh khác                | Phát sinh cước chuyển điểm + Lưu ca                                     |
| Cộng                          |                                                                         |
| Lưu ca                        |                                                                         |
| Phát sinh chuyển điểm         |                                                                         |
| Ghi chú                       | theo ghi chú của Điều xe                                                |

**8.1.3.5 Bảng kê chi tiết phí làm hàng**

![](../../.gitbook/assets/12.png)

| Ngày thực hiện                       | Ngày tạo/ sửa lô                                                                                          |
| ------------------------------------ | --------------------------------------------------------------------------------------------------------- |
| Bill                                 | Số vận đơn/ booking khai báo khi tạo lô                                                                   |
| Mã lô                                | Được tạo ra từ Qly lô hàng                                                                                |
| Loại lô hàng                         | Nhập/xuất/Nội địa                                                                                         |
| Phí dịch vụ giao nhận hàng nhập khẩu | = Tổng phí dịch vụ trong qtkh - (lưu ca + cước vận chuyển + phát sinh chuyển điểm + phát sinh lạch huyện) |
| Chi phí hải quan giám sát            | =Phí HQ giám sát ở Qly tạm ứng lô hàng                                                                    |
| Phát sinh vận chuyển                 | Tổng cước VC trong QTKH                                                                                   |
| Thuế GTGT dịch vụ                    | Tổng phí dịch vụ trong QTKH \* VAT (được khai báo khi tạo lô hàng)                                        |
| Thuế GTGT vận chuyển                 | Tổng Cước VC trong QTKH \* VAT                                                                            |
| VAT                                  | Phí VAT được khai báo khi tạo lô hàng                                                                     |
| Khách tạm ứng                        | Được khai báo cột Khách tạm ứng - Qly cước VC                                                             |
| Danh sách phí                        | Các phí thuộc mục Chi trả hộ của QTKH (số HĐ, ngày HĐ lấy từ QTNB sang)                                   |
| Tổng                                 | Tổng chi phí chi trả hộ                                                                                   |
| Lưu ca                               | tiền lưu ca được khai báo khi tạo Điều xe                                                                 |
| Phí phát sinh chuyển điểm            | Phí phát sinh khi có tuyến chuyển điểm được link từ cột Phát sinh chuyển điểm - Qly cước VC               |
| Tổng cộng                            | Tổng các phí trên bảng                                                                                    |
| Số cont                              | Số cont đã vận chuyển của lô                                                                              |
| Ghi chú                              | theo ghi chú của Điều xe                                                                                  |

#### **8.1.4 Báo cáo cước xe ngoài** <a href="#_415t9al" id="_415t9al"></a>

**8.1.4.1 Báo cáo cước xe ngoài**

Hiển thị thông tin chuyến hàng và cước phí tương ứng với những chuyến xe thuê ngoài.

![](../../.gitbook/assets/13.png)

_Màn hình báo cáo cước xe ngoài_

| Báo cáo cước xe ngoài  | <p>Báo cáo của các xe thuần xe ngoài (chỉ nằm trong nhóm Đơn vị vận tải - bảng </p><p>Đối tác)</p>                                     |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| Thu khách              | <p>Cước: Cước HĐ được tính trong Ql cước vc</p><p>Phát sinh: Lưu ca + Chi trả hộ theo chuyến, được tính trong Ql cước vc</p>           |
| Thuê ngoài             | <p>Cước: Cước thuê ngoài, được tính trong Ql cước vc</p><p>Phát sinh: cột Phát sinh cước thuê ngoài, được tính trong Ql cước vc </p>   |
| Chênh lệch             | = Thu khách - Thuê ngoài                                                                                                               |
| Trạng thái             | <p>Theo trạng thái trong Điều xe</p><p>Vận chuyển= chưa vc, đã nhận hàng, đã giao hàng, về bãi </p><p>Hủy. trễ= hủy chuyến, bị trễ</p> |
| Ghi chú                | Theo ghi chú điều xe                                                                                                                   |

**8.1.4.2 Báo cáo đối soát**

Báo cáo đối soát: Hiển thị thông tin chuyến hàng và cước phí tương ứng với những chuyến xe thuê ngoài của đơn vị vận tải vừa là nhà xe vừa là khách hàng. Sử dụng để đối soát cước giữa 2 đơn vị và hạch toán hàng tháng.

Báo cáo theo các xe là chủ xe ngoài (nằm trong nhóm Đơn vị vận tải và có thể cả nhóm KH,...). Đơn vị vận tải được chọn tìm kiếm đóng vai trò là cả Chủ xe và Khách hàng.

Mẫu hiển thị: Giống với Báo cáo cước xe ngoài.

*
  *
    1. **Báo cáo tổng hợp theo dõi bảo hiểm**

Báo cáo tổng hợp theo dõi bảo hiểm tổng hợp thông tin lấy dữ liệu từ Danh sách xe và mục Quản lý phí thường niên – Kế toán

![](<../../.gitbook/assets/14 (1).png>)

_Màn hình Báo cáo tổng hợp theo dõi bảo hiểm_

| Nhãn hiệu, Năm sản xuất, Tải trọng            | Lấy trong Danh sách xe                      |
| --------------------------------------------- | ------------------------------------------- |
| Tên đăng ký, Hạn ngân hàng, Ngày mua bảo hiểm | Vay ngân hàng/Lãi ngân hàng                 |
| BHTNDS                                        | Lấy trong Kế toán – Quản lý phí thường niên |
| BHVC                                          | Lấy trong Kế toán – Quản lý phí thường niên |

*
  *
    1. **Bảng kê chi tiết vận tải**

![](../../.gitbook/assets/15.png)

_Màn hình Bảng kê chi tiết vận tải_

| Thời gian tìm kiếm                     | Ngày vận chuyển                                               |
| -------------------------------------- | ------------------------------------------------------------- |
| Khách hàng                             | Lấy từ cột Mã đối tác trong Quản lý đối tác - TTC             |
| Hãng tàu                               | Lấy từ Quản lý hãng tàu trong TTC và link từ Qly lô hàng      |
| Ngày chạy                              | Ngày vận chuyển                                               |
| Xe chạy                                | Link từ Điều xe                                               |
| Tuyến đường                            |                                                               |
| Tên hàng                               | Lấy từ Quản lý hàng hóa – TTC, link từ Qly lô hàng            |
| BL - INVOICE NO                        | Số vận đơn/số booking trong Qly lô hàng                       |
| Tờ khai                                | Số tờ khai trong Qly lô hàng                                  |
| Ngày TK                                | Ngày làm tờ khai trong Qly lô hàng                            |
| Luồng TK                               |                                                               |
| Số cont                                | Số cont của chuyến xe                                         |
| Loại cont                              | (Các) loại cont của chuyến                                    |
| SL                                     | Số lượng cont của chuyến                                      |
| X/N                                    | Loại lô hàng trong Qly lô hàng                                |
| <p>Cước vận chuyển</p><p>Tổng cộng</p> | <p>Link từ chi phí trong QTKH</p><p>= cột Phát sinh + VAT</p> |
| <p>Chi trả hộ</p><p>Tổng tiền</p>      | Link từ chi phí trong QTNB                                    |
| Hóa đơn                                |                                                               |

### **8.2 Báo cáo trucking** <a href="#_vgdtq7" id="_vgdtq7"></a>

#### **8.2.1 Báo cáo cước phí** <a href="#_3fg1ce0" id="_3fg1ce0"></a>

**8.2.1.1 Báo cáo cước phí theo khách hàng**

Báo cáo theo Khách hàng: Tổng hợp các nội dung liên quan đến thu chi cho khách có phát sinh vận chuyển trong tháng. Cho phép lọc theo khách hàng và theo tháng.

![](<../../.gitbook/assets/16 (6).png>)

_Màn hình Bc cước phí theo khách hàng_

| Chủ xe                                              | Lấy theo tên viết tắt, riêng xe trong thì chia theo phòng ban                                                       |
| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Điểm bắt đầu - Địa điểm giao hàng                   | Lấy theo Điểm đi - Điểm đến trong Điều xe, chiều xe đi đầu tiên                                                     |
| Ngày giao, số cont, loại cont, số vỏ rỗng, số kiện  | Lấy theo dữ liệu trong điều xe                                                                                      |
| Lượng giao - nhận                                   | Có thể lấy trong khai báo khi điều xe hoặc trong Ql cước vc                                                         |
| Khoảng cách                                         | Tổng các chiều đi (không lấy chiều về cuối cùng)                                                                    |
| Cước nội bộ                                         | Ql cước vc, Chênh lệch = Thực thu - Thuê ngoài                                                                      |
| Cước HĐ                                             | Ql cước vc, Chênh lệch cước= Cước HĐ - Cước thực thu                                                                |
| Phát sinh chuyển điểm                               | Cước HĐ nhập trong ô chuyển điểm của Ql cước vc                                                                     |
| Tiền dầu                                            | = số lít dầu định mức x Đơn giá, trong Ql cước vc                                                                   |
| Tiền đường, Chi trả hộ theo chuyến                  | Ql cước vc                                                                                                          |
| Tổng chi hộ                                         | = Tổng chi trả hộ theo chuyến                                                                                       |
| Tổng thu                                            | = Cước thực thu + Lưu ca                                                                                            |
| Tổng chi                                            | = Cước thuê ngoài + Tiền dầu + Tiền đường                                                                           |
| Lợi nhuận                                           | <p>= Tổng thu - Tổng chi</p><p>(Note: Chi phí phát sinh chuyển điểm đc tách riêng, k tính lẫn vào các chi phí) </p> |

**8.2.1.2 Báo cáo cước phí theo chủ xe**

![](<../../.gitbook/assets/17 (1).png>)

_Màn hình Bc cước phí theo chủ xe_

| Ngày tìm kiếm             | Theo ngày giao hàng                                                           |
| ------------------------- | ----------------------------------------------------------------------------- |
| Cước Thực thu             | Cước thực thu + Phát sinh chuyển điểm thực thu                                |
| Cước thuê ngoài           | Cước thuê ngoài + Phát sinh + phát sinh chuyển điểm (Tổng thành tiền cước TN) |
| Cước HĐ                   | Cước HĐ (không cộng phát sinh chuyển điểm)                                    |
| Môi giới                  | = Cước hợp đồng - Cước thực thu                                               |
| Tổng cước vận tải theo lô | = Tổng cước thực thu của cả lô (tổng các chuyển)                              |

**8.2.1.3 Bảng kê cước vận chuyển**

Liệt kê chi phí vận chuyển trong tháng theo từng xe.

![](<../../.gitbook/assets/18 (5).png>)

_Màn hình Bảng kê cước vận chuyển_

| Ngày tờ khai           | Ngày làm tờ khai, nhập khi tạo lô hàng                                 |
| ---------------------- | ---------------------------------------------------------------------- |
| Tuyến vận chuyển       | Chiều đầu tiên của chuyến vận chuyển trong Ql cước vc                  |
| Chi trả hộ             | Tổng tiền chi trả hộ theo QTNB                                         |
| Cước                   | Tổng tiền cước thực thu theo QTNB                                      |
| Phát sinh              | Phát sinh cước chuyển điểm + Lưu ca                                    |
| Tổng cộng              | = Chi trả hộ + Cước + Phát sinh                                        |
| Số tiền nhận của KH    | Người dùng nhập tay trực tiếp                                          |
| Người nhận tiền của KH | Lựa chọn trong danh sách nhân viên (đã khai báo trong TTC – Nhân viên) |
| Chênh lệch thanh toán  | = Tổng cộng – Số tiền nhận của KH                                      |

#### **8.2.2 Báo cáo vận chuyển** <a href="#_1ulbmlt" id="_1ulbmlt"></a>

Tổng hợp các thông tin liên quan đến chuyến hàng và xe điều cho chuyến. Lưu trữ các chứng từ hóa đơn do Lái xe gửi lên từ điện thoại. Cho phép người dùng tìm kiếm theo tháng và theo các thông số: mã lô, số cont, số xe hoặc khách hàng.

**Báo cáo vận chuyển**

![](<../../.gitbook/assets/19 (5).png>)

| Số vận đơn        | Số vận đơn/ số booking khai báo từ lô hàng                                   |
| ----------------- | ---------------------------------------------------------------------------- |
| Thực giao         | Lượng KH giao (lái xe nhận)                                                  |
| Thực nhận         | Lượng KH nhận (lái xe giao)                                                  |
| Chênh lệch        | = Thực nhận – Thực giao                                                      |
| Chi phí phát sinh | Phát sinh chi lái xe (nhập từ app hoặc trong Quản lý thu chi lái xe-phí chi) |
| Thu phát sinh     | Phát sinh lái xe thu (nhập từ app hoặc trong Quản lý thu chi lái xe-phí thu) |
| Thuê ngoài        | Cước thuê ngoài trong Ql cước vc                                             |
| Thực thu          | Cước thực thu trong Ql cước vc                                               |
| Hợp đồng          | Cước HĐ trong Ql cước vc                                                     |
| Ảnh chứng từ      | Ảnh từ mobile gửi lên                                                        |
| Ghi chú           | Ghi chú của điều xe/ đx gộp cước                                             |

**8.2.2.2 Báo cáo Vendor**

![](<../../.gitbook/assets/20 (4).png>)

| Ngày             | Ngày giao hàng                                                                         |
| ---------------- | -------------------------------------------------------------------------------------- |
| Địa điểm         | Điểm địa                                                                               |
| Lượng nhận       | Lượng LX nhận (theo Ql cước vc)                                                        |
| Lượng giao       | Lượng LX giao (theo Ql cước vc)                                                        |
| Hao hụt          | Lượng giao - nhận                                                                      |
| Hao hụt cho phép | từ Quản lý lô hàng → form thêm mới lô→ tab mở rộng                                     |
| Đền HH           | = hao hụt- HH cho phép (HH cho phép = % HH cho phép \* lượng LX nhận)                  |
| Đơn giá          | từ Quản lý lô hàng → form thêm mới lô→ tab mở rộng                                     |
| Thành tiền       | = Đền HH x đơn giá                                                                     |
| Đơn giá          | Đơn giá thực thu (trong Ql cước vc)                                                    |
| Thành tiền       | Lượng giao/ nhận (khai báo từ điều xe xem tính theo lượng nào) x Đơn giá TT            |
| Thực lĩnh        | = Thành tiền - Thành tiền (đền hao hụt)                                                |
| Ghi chú          | Ghi chú của lô hàng                                                                    |
| Tổng             | Tổng tiền (có làm tròn đến hàng nghìn đồng)                                            |
| VAT              | mặc định VAT 10%                                                                       |
| Tổng cộng        | = Thành tiền/ thực lĩnh + 10% Thành tiền/ thực lĩnh (có làm tròn đến hàng nghìn đồng)  |

*
  *
    1. **Báo cáo vận chuyển**

| Số thứ tự         | Sắp xếp đúng theo thứ tự danh sách xe lấy từ Thông tin chung -> Danh sách xe                |
| ----------------- | ------------------------------------------------------------------------------------------- |
| Số xe             | Lấy theo Thông tin chung -> Danh sách xe                                                    |
| Chuyến Hà Nội     | Số lượng chuyến có điểm đi/ đến = địa chỉ mở rộng – Hà Nội (địa chỉ default, không có xóa)  |
| Chuyến Yên Bái    | Số lượng chuyến có điểm đi/ đến = địa chỉ mở rộng – Yên Bái (địa chỉ default, không có xóa) |
| Chuyến ngắn       | Đếm số lượng chuyến ngắn từ app mobile gửi lên                                              |
| Kẹp               | = Số chuyến – (Chuyến Yên Bái + Chuyến ngắn)                                                |
| Số chuyến         | Tổng số chuyến đếm theo khoảng thời gian lọc                                                |
| Dầu theo định mức | Tổng định mức dầu của các chuyến đường dài ở mục Điều xe                                    |
| Dầu đã cấp        | Tổng lượng dầu cấp của từng xe trong khoảng thời gian tìm kiếm                              |
| Dầu chênh         | = Dầu theo ĐM – Dầu đã cấp                                                                  |
| Tổng tiền vé      | = Tổng tiền cột vé đã nhập trong Điều xe theo khoảng thời gian tìm kiếm                     |
| Tổng tiền lương   | = Tổng tiền cột lương chuyến đã nhập trong Điều xe theo khoảng thời gian tìm kiếm           |
| Tổng tiền luật    | = Tổng tiền cột tiền luật đã nhập trong Điều xe theo khoảng thời gian tìm kiếm              |
| Phí phát sinh     | = Tổng tiền cột Phí phát sinh đã nhập trong Điều xe theo khoảng thời gian tìm kiếm          |
| Hủy / Chậm chuyến | Tổng số lượng chuyến vận chuyển của xe ở trạng thái Hủy/ Trễ (trạng thái trong Điều xe)     |

*
  *
    1. **Báo cáo sản lượng hiện trường**

Tìm kiếm dữ liệu theo tên nhân viên làm hàng

*
  *
    *
      1. _**Báo cáo sản lượng hàng xuất**_

| Khách hàng | Thông tin khách hàng đã nhập trong QL lô hàng đủ/ rút gọn theo khoảng thời gian tìm kiếm |
| ---------- | ---------------------------------------------------------------------------------------- |
| Số book    | Lấy thông tin từ Số booking ở Ql lô hàng                                                 |
| Số cont    | Từ cột số cont hàng ở mục Điều xe                                                        |
| Loại cont  | Từ cột loại cont hàng ở mục Điều xe                                                      |
| Ngày ứng   | Lấy thông tin từ Kế toán -> QTNB -> -> hiển thị ở cột Ngày tạm ứng                       |
| Ngày chạy  | Lấy từ Ngày vận chuyển ở Điều hành -> Kế hoạch vận chuyển                                |
| Số xe      | Lấy theo Thông tin chung -> Danh sách xe                                                 |

*
  *
    *
      1. _**Báo cáo sản lượng hàng nhập**_

| Khách hàng         | Thông tin khách hàng đã nhập trong QL lô hàng đủ/ rút gọn theo khoảng thời gian tìm kiếm |
| ------------------ | ---------------------------------------------------------------------------------------- |
| Số bill            | Lấy từ thông tin Mã vận đơn trong QL lô hàng                                             |
| Số lượng cont/bill | Từ cột số cont hàng ở mục Điều xe                                                        |
| Loại cont          | Từ cột loại cont hàng ở mục Điều xe                                                      |
| Ngày ứng           | Lấy thông tin từ Kế toán -> QTNB -> -> hiển thị ở cột Ngày tạm ứng                       |

#### **8.2.5 Báo cáo chi tiết giao hàng** <a href="#_18vjpp8" id="_18vjpp8"></a>

Báo cáo chi tiết giao hàng theo từng lô trong tháng.



_Báo cáo chi tiết giao hàng cont_



_Báo cáo chi tiết giao hàng rời_

| Mục đích                     | Kiểm soát lượng hàng giao theo lô tại mỗi điểm, tổng lượng đã giao và còn tồn (cần giao) |
| ---------------------------- | ---------------------------------------------------------------------------------------- |
| Tìm kiếm                     | Theo trả hàng, mã lô                                                                     |
| Điểm giao                    | Điểm đến trong chiều xe đi (trong Điều xe)                                               |
| VC                           | Chủ xe (tên viết tắt)                                                                    |
| Số lượng                     | Hàng cont, số lượng cont                                                                 |
| Tổng hàng cần giao theo điểm | Hàng cont, Tổng số lượng cont của lô hàng có cùng điểm giao                              |
| Lượng LX nhận/ giao          | Hàng rời, theo Ql cước vc                                                                |
| Chênh lệch                   | Hàng rời, = Lượng nhận - giao                                                            |
| Ghi chú                      | Ghi chú của lô hàng                                                                      |
| Tổng hàng đã giao            | Số lượng giao                                                                            |
| Tổng hàng cần giao           | Số lượng khai báo khi tạo lô (Ql lô hàng)                                                |
| Còn lại                      | = Tổng cần giao - Tổng đã giao                                                           |

### **8.3 Báo cáo kho - sửa chữa** <a href="#_3sv78d1" id="_3sv78d1"></a>

#### **8.3.1 Báo cáo sửa chữa** <a href="#_280hiku" id="_280hiku"></a>

_Màn hình Báo cáo sửa chữa_

| Chủ xe            | Phòng ban                                                                           |
| ----------------- | ----------------------------------------------------------------------------------- |
| Mã tạm ứng        | Mã tạm ứng sửa chữa (do người dùng chọn, theo Kế toán→ Quản lý sửa chữa)            |
| Phân loại         | Chọn loại vật tư                                                                    |
| Nội dung thay thế | Nội dung của hóa đơn sửa chữa                                                       |
| Tên phụ tùng      | Tên vật tư                                                                          |
| Chi tiết          | Nội dung chi tiết trong hóa đơn sửa chữa- nội dung hỏng                             |
| Mã nhân viên      | Theo mã nhân viên của Mã tạm ứng (không phải người phụ trách khai trong hóa đơn)    |
| Số serial         | Chỉ có với những vật tư có ch tiết, quản lý số serial - và là số serial thay mới.   |

#### **8.3.2 Báo cáo lốp** <a href="#_n5rssn" id="_n5rssn"></a>

Báo cáo được kết xuất dữ liệu từ các hóa đơn khai báo sửa chữa cho xe, với loại vật tư là Lốp. Báo cáo tổng hợp tình trạng thay và sử dụng lốp của từng xe trong công ty vận tải, đưa ra cản báo đến hạn thay lốp, giúp bộ phận sửa chữa theo dõi và lên kế hoạch kiểm tra, thay thế.

_Màn hình báo cáo sử dụng lốp_

| Ngày thay                        | Ngày hỏng                                                                                               |
| -------------------------------- | ------------------------------------------------------------------------------------------------------- |
| Loại lốp                         | Tên phụ tùng                                                                                            |
| Số lốp                           | Số serial mới                                                                                           |
| Km tại thời điểm thay            | Chỉ số km nhập trong chi tiết sửa chữa                                                                  |
| Số km di chuyển lốp của hiện tại | Theo dữ liệu điều xe                                                                                    |
| Ngày nhập liệu                   | Ngày nhập chỉ số km trong điều xe                                                                       |
| Số ngày sử dụng lốp đến hiện tại | = Ngày Hôm nay - Ngày thay                                                                              |
| Tgian bảo hành lốp               | Ghi trong chi tiết sửa chữa                                                                             |
| Tình trạng                       | <p>Tính theo số ngày sử dụng và tgian sử dụng</p><p>Theo dỡi cả trên bảng Sửa chữa- Quản lý quá hạn</p> |
| Thông số tái sử dụng lốp         | Theo khai báo chi tiết vật tư lốp khi nhập kho                                                          |

#### **8.3.3 Báo cáo bảo dưỡng** <a href="#_375fbgg" id="_375fbgg"></a>

_Màn hình Báo cáo bảo dưỡng_

| Phạm vi                                         | <p>Khi sửa chữa, khai báo loại vật tư là Bảo dưỡng </p><p>Tgian hiển thị: 1 năm </p> |
| ----------------------------------------------- | ------------------------------------------------------------------------------------ |
| <p>Nội dung bảo dưỡng</p><p>Ngày: </p><p>Km</p> | <p>Ngày sửa ghi trên hóa đơn </p><p>Chỉ số km khai báo trong chi tiết sửa chữa </p>  |
| Theo km cũ                                      | = Km tháng mới - Km tháng cũ                                                         |
| Theo số ngày cũ                                 | = Ngày thay mới - ngày thay cũ                                                       |
| Số ngày đến hiện tại                            | = Ngày Hôm nay - Ngày thay                                                           |
| Cảnh báo                                        | Cảnh báo quá hạn (Dựa vào ngày quá hạn trong chi tiết sửa chữa)                      |

#### **8.3.4 Tồn kho** <a href="#_1maplo9" id="_1maplo9"></a>

Là bảng tổng hợp các thông tin về kho vật tư, phụ tùng của bộ phận Sửa chữa, bao gồm: số liệu nhập, xuất, tồn, đơn giá, xuất xứ, nhà cung cấp của tùng loại phụ tùng.

Thông tin tồn kho được tổng hợp từ bảng nhập phụ tùng, xuất kho trong mục Sửa chữa. Lượng tồn bằng lượng nhập trừ xuất.

_Màn hình Báo cáo tồn kho_

| Tồn đầu    | = Tồn của tháng trước                          |
| ---------- | ---------------------------------------------- |
| Nhập       | Tổng nhập trong tháng                          |
| Xuất       | Tổng xuất kho trong tháng (K bao gồm sửa chữa) |
| Tồn        | = Tồn đầu + Nhập - Xuất – Bù kiểm              |
| Đơn giá    | Đơn giá nhập                                   |
| Thành tiền | = Đơn giá x Tồn                                |

#### **8.3.5 Báo cáo thanh toán vật tư nhập** <a href="#_46ad4c2" id="_46ad4c2"></a>

_Màn hình Báo cáo thanh toán nhập vật tư và sửa chữa_

| Ngày              | Ngày sửa/ Ngày nhập kho (do người dùng khai báo, k phải ngày tạo) |
| ----------------- | ----------------------------------------------------------------- |
| Chủ xe            | <p>Sửa chữa: Theo nhóm xe</p><p>Nhập kho= K</p>                   |
| Phương tiện       | Số xe khai báo sửa chữa/ Kho                                      |
| Nội dung thay thế | Nội dung hỏng trong chi tiết hóa đơn sửa chữa                     |
| Thành tiền        | Tiền sửa chữa/ Tiền nhập kho                                      |
| Ghi chú           | Sửa chữa/ nhập kho                                                |

### **8.4 Báo cáo dầu** <a href="#_2lfnejv" id="_2lfnejv"></a>

#### **8.4.1 Báo cáo sử dụng nhiên liệu** <a href="#_10kxoro" id="_10kxoro"></a>

Tổng hợp thông tin tồn/cấp/ sử dụng nhiên liệu theo xe.

* Dầu theo định mức: Tính theo lượng đã cài đặt trong thông tin chung/ quản lý cước vc/ quản lý định mức dầu.
* Dầu đổ thực tế: Lấy theo lượng dầu cấp trong Quản lý cấp dầu cho xe.

_Màn hình Báo cáo sử dụng nhiên liệu theo xe_

| Dầu theo định mức | Lấy theo số liệu từ Ql cước vc                                                 |
| ----------------- | ------------------------------------------------------------------------------ |
| Dầu đổ thực tế    | Lấy theo số liệu trong Quản lý cấp dầu cho xe                                  |
| Dầu tồn           | = Lượng còn dư của tháng trước                                                 |
| Dầu chạy          | Tổng số lít dầu theo định mức                                                  |
| Dầu đổ            | Tổng số lít dầu đổ thực tế                                                     |
| Bù kiểm           | Người dùng nhập tay trực tiếp                                                  |
| Lượng còn dư      | = (Dầu tồn + Dầu chạy + Bù kiểm)- Dầu đổ (Lượng tồn còn được đổ cho tháng sau) |

#### **8.4.2 Báo cáo tồn dầu** <a href="#kix.2vgjiljteq0k" id="kix.2vgjiljteq0k"></a>

Tổng hợp lượng dầu nhập, xuất, tồn của kho trong và lượng dầu xe đổ ngoài. Lượng dầu tồn được tính bằng lượng nhập trừ lượng hao hụt và lượng dầu xuất trên các cây dầu của công ty, không tính dầu đổ ngoài.

_Màn hình báo cáo tồn dầu_

| Điều kiện                | Có phát sinh cấp dầu trong tháng                                              |
| ------------------------ | ----------------------------------------------------------------------------- |
| Kỳ trước chuyển sang     | Tổng tồn dầu tháng trước                                                      |
| Ngày tháng               | <p>Ngày nhập- Quản lý nhập dầu</p><p>Ngày cấp- Quản lý cấp dầu cho xe</p>     |
| Nhập dầu                 | Theo Ql nhập nhiên liệu                                                       |
| Lượng hao hụt            | theo dữ liệu khi nhập dầu                                                     |
| Dầu xuất                 | <p>NCC dầu: Tách cột</p><p>Dầu đổ ngoài: hiển thị chung tại cột Dầu ngoài</p> |
| Tồn                      | = Nhập dầu - Dầu xuất                                                         |
| Tổng số trên cây dầu bơm | Chỉ số cây dầu trong Ql cấp dầu cho xe                                        |
