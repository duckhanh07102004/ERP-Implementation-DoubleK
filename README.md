# ERP-Implementation-DoubleK

Phân tích, thiết kế, và ứng dụng giải pháp ERP cho DoubleK, chuỗi cửa hàng quần áo.

BỐI CẢNH DOANH NGHIỆP HIỆN TẠI

**Giới thiệu tổng quan**
Những năm gần đây, DoubleK đã nhanh chóng mở rộng mạng lưới lên hơn 10 chi nhánh tại Thành phố Hồ Chí Minh và tạo dựng được chỗ đứng trong thị trường thời trang Việt Nam. Nhờ vào chất lượng sản phẩm và giá cả cạnh tranh, DoubleK không chỉ thu hút được khách hàng từ các cửa hàng trực tiếp mà còn phát triển mạnh trên các nền tảng thương mại điện tử.
Tuy nhiên, sau 5 năm hoạt động, DoubleK bắt đầu đối mặt với những thách thức về hiệu quả vận hành và doanh thu không đáp ứng được chi phí ngày càng tăng. Qua phân tích nội bộ, ban lãnh đạo đã xác định các vấn đề chính bao gồm:
1.	Quy trình nhập hàng không tối ưu: Việc đặt hàng và kiểm soát hàng hóa từ nhà cung cấp còn bất cập, dẫn đến chi phí cao và hàng tồn không cần thiết.
2.	Thiếu đồng bộ hoá giữa các bộ phận: Doanh nghiệp thường gặp khó khăn trong việc đồng bộ hóa và tương tác giữa các bộ phận khác nhau. Sự phối hợp giữa bộ phận bán hàng, quản lý kho, kế toán và các cửa hàng chưa hiệu quả, gây chậm trễ đến toàn bộ hệ thống. Thiếu thông tin và giao tiếp kém giữa các bộ phận có thể dẫn đến sự mất mát thông tin, sự không nhất quán và khó khăn trong việc quản lý quy trình.
3.	Quản lý kho không hiệu quả: Việc kiểm soát hàng hóa nhập về và lưu trữ tại kho chưa được thực hiện tốt, dẫn đến tình trạng thừa hoặc thiếu sản phẩm, ảnh hưởng đến khả năng phục vụ khách hàng.
4.	Chất lượng sản phẩm không đồng đều: Do thiếu quy trình kiểm tra kỹ lưỡng khi nhập hàng, một số sản phẩm không đáp ứng kỳ vọng của khách hàng, ảnh hưởng đến uy tín thương hiệu.
5.	Khả năng đáp ứng nhu cầu thị trường kém linh hoạt: DoubleK chưa tối ưu hóa việc lựa chọn và thay đổi danh mục hàng hóa để phù hợp với xu hướng thời trang liên tục thay đổi.
6.	Khó khăn trong quản lý nguồn nhân lực: Doanh nghiệp có thể gặp khó khăn trong việc quản lý và tối ưu hóa nguồn nhân lực. Thiếu thông tin và công cụ để đánh giá và phát triển nhân viên có thể dẫn đến sự thiếu hụt kỹ năng và hiệu suất làm việc không đạt yêu cầu.
7.	Hạn chế trong việc tối ưu hóa chi phí nhập hàng: Việc không tận dụng các mối quan hệ hoặc lợi ích từ nhà cung cấp đã khiến chi phí nhập hàng cao hơn so với đối thủ cạnh tranh.
Đứng trước những thách thức này, DoubleK cần một chiến lược tái cấu trúc mạnh mẽ, tập trung vào tối ưu hóa quy trình nhập hàng, quản lý kho và nâng cao chất lượng sản phẩm để đảm bảo khả năng cạnh tranh và duy trì niềm tin từ khách hàng.

**Đặt vấn đề**

Vấn đề lớn nhất mà DoubleK đang gặp phải là sự thiếu liền mạch trong việc chia sẻ và xử lý thông tin giữa các phòng ban. Điều này khiến thông tin giữa các bộ phận như mua hàng, kho, bán hàng, và tài chính bị chậm trễ, gây ảnh hưởng trực tiếp đến khả năng đáp ứng nhu cầu của khách hàng và vận hành doanh nghiệp.
Để khắc phục tình trạng này, DoubleK đã quyết định triển khai hệ thống ERP, cụ thể là Odoo. Việc áp dụng ERP được kỳ vọng sẽ giúp cải thiện toàn diện quy trình vận hành, từ quản lý thông tin đến tối ưu hóa nguồn lực, mang lại sự minh bạch và đồng bộ giữa các phòng ban.

Dưới đây là các bộ phận chính liên quan đến quy trình cốt lõi của DoubleK và sự thay đổi sau khi triển khai ERP:

Bộ phận Cung ứng

Phòng Thu mua: Quản lý thông tin nhà cung cấp và đơn đặt hàng hiệu quả hơn, giúp đảm bảo nguồn hàng ổn định.

Phòng Kho: Theo dõi lượng tồn kho chính xác, giảm thiểu hàng thừa hoặc thiếu.

Phòng Logistics: Tối ưu hóa quy trình vận chuyển và giao nhận hàng hóa đến các chi nhánh.

Bộ phận Kinh doanh

Phòng Bán hàng (Sales): Tích hợp dữ liệu đơn hàng từ các chi nhánh và kênh trực tuyến, cải thiện tốc độ xử lý đơn hàng.

Phòng Marketing: Quản lý các chiến dịch marketing, theo dõi hiệu quả và tương tác khách hàng trên một nền tảng tập trung.

Bộ phận Tài chính – Kế toán

Tích hợp quản lý doanh thu, chi phí và báo cáo tài chính theo thời gian thực, tăng tính minh bạch và chính xác trong việc ra quyết định.

Bộ phận Nhân sự

Quản lý thông tin nhân viên, lịch làm việc và hiệu suất làm việc dễ dàng hơn.

Việc triển khai ERP giúp DoubleK không chỉ cải thiện hiệu suất nội bộ mà còn nâng cao chất lượng phục vụ khách hàng, tạo tiền đề để mở rộng và phát triển bền vững trong tương lai

**Quy trình nghiệp vụ trước khi áp dụng ERP**

Quy trình tổng quát

Sơ đồ quy trình

 ![image](https://github.com/user-attachments/assets/b4785069-db02-4fa7-8b06-696813af120a)

Mô tả quy trình

Quy trình tổng quát của cửa hàng bán lẻ bao gồm 6 bước chính, bắt đầu với quy trình mua hàng. Tại đây, cửa hàng xác định nhu cầu hàng hóa dựa trên tồn kho hiện tại hoặc kế hoạch kinh doanh, sau đó tìm nhà cung cấp phù hợp, thương lượng giá cả, và đặt hàng. Sau khi hàng được giao, nhân viên kiểm tra chất lượng, số lượng, nhập kho và cập nhật dữ liệu tồn kho. Tiếp theo là quản lý kho, nơi cửa hàng tổ chức lưu trữ, kiểm kê định kỳ để đảm bảo số liệu khớp thực tế, và theo dõi cảnh báo hàng tồn kho thấp. Quy trình bán hàng bao gồm việc tiếp nhận khách hàng tại cửa hàng hoặc trực tuyến, tư vấn, xử lý giao dịch, và cập nhật tồn kho. Sau bán hàng, cửa hàng thực hiện chăm sóc khách hàng, bao gồm tiếp nhận phản hồi, xử lý khiếu nại, và hỗ trợ đổi trả hàng nếu cần. Quản lý tài chính là một phần quan trọng để theo dõi doanh thu, chi phí, quản lý dòng tiền và thanh toán. Cuối cùng, cửa hàng tiến hành báo cáo và phân tích với mục tiêu tổng hợp số liệu, đánh giá hiệu quả hoạt động, và hỗ trợ ra quyết định chiến lược nhằm tối ưu hóa kinh doanh.

Quy trình quản lý chuỗi cung ứng

Sơ đồ quy trình

![image](https://github.com/user-attachments/assets/54b412f2-ef77-4d42-987d-e5df15dda92d)

Mô tả quy trình

Quy trình nhận và xử lý đơn hàng của nhà cung cấp bao gồm các bước chính như sau. Đầu tiên, nhà cung cấp nhận đơn hàng từ khách hàng, thường thông qua hình thức thủ công như ghi chép hoặc qua điện thoại. Sau đó, nhà cung cấp tạo đơn hàng trong hệ thống. Khi đơn hàng được xác nhận, nhà cung cấp tiến hành giao hàng Tiếp theo, nhân viên cửa hàng kiểm tra số lượng và chất lượng hàng hóa sau khi nhận hàng. Trong trường hợp không đủ hàng, nhà cung cấp phải thông báo tình trạng này .Cuối cùng, nhà cung cấp cần gửi yêu cầu bổ sung hàng hóa nếu thiếu.

Các vấn đề gặp phải trong quy trình

Các vấn đề gặp phải trong quy trình nhận và xử lý đơn hàng:

1.	Sai sót trong truyền đạt thông tin:

Thông tin đơn hàng thường được ghi nhận thủ công hoặc qua điện thoại, dễ xảy ra lỗi như ghi sai số lượng, sản phẩm, hoặc thông tin khách hàng.

2.	Tốn thời gian trong việc tạo đơn hàng:

Quy trình nhập liệu thủ công và xác nhận lại thông tin mất nhiều thời gian, làm chậm tiến độ xử lý đơn hàng.

3.	Theo dõi giao hàng không hiệu quả:

Việc giám sát giao hàng bằng phương pháp thủ công dẫn đến nguy cơ giao hàng không đúng hẹn, ảnh hưởng đến sự hài lòng của khách hàng.

4.	Kiểm tra hàng hóa không đầy đủ:

Kiểm tra số lượng và chất lượng hàng hóa không được thực hiện kịp thời hoặc chi tiết, có thể dẫn đến việc phát hiện lỗi muộn, gây khó khăn trong xử lý.

5.	Thông báo thiếu hàng chậm trễ:

Khi không đủ hàng, nhà cung cấp thường báo cáo tình trạng không kịp thời, làm gián đoạn kế hoạch kinh doanh của khách hàng.

6.	Quy trình bổ sung hàng hóa kéo dài:

Việc gửi yêu cầu và chờ phản hồi từ các bên liên quan làm tăng thời gian hoàn tất đơn hàng, ảnh hưởng đến khả năng đáp ứng nhu cầu thị trường.

Những vấn đề trên không chỉ làm giảm hiệu quả vận hành mà còn ảnh hưởng tiêu cực đến trải nghiệm của khách hàng và hiệu suất kinh doanh tổng thể.

Quy trình bán hàng

Sơ đồ quy trình

![image](https://github.com/user-attachments/assets/b4bd6fc4-e9af-4d79-bd03-631bdbfd4f10)

Mô tả quy trình

Quy trình mua sắm trực tuyến bắt đầu khi khách hàng truy cập website để bắt đầu trải nghiệm mua sắm. Trong bước chọn sản phẩm, khách hàng tìm kiếm và chọn sản phẩm mong muốn nhưng có thể gặp khó khăn trong việc tìm kiếm thông tin nếu hệ thống không hỗ trợ tốt chức năng lọc hoặc tìm kiếm. Tiếp theo, khách hàng đặt hàng bằng cách nhập thông tin đơn hàng, nhưng quá trình này có thể kéo dài nếu thông tin không đầy đủ hoặc giao diện phức tạp. Đơn hàng sau đó cần xác nhận từ nhân viên, dẫn đến sự chậm trễ nếu thiếu sự tự động hóa. Trong bước thanh toán, tình trạng thanh toán có thể không được cập nhật ngay lập tức, khiến khách hàng cảm thấy không chắc chắn về giao dịch của mình. Khi đến giai đoạn giao hàng, việc theo dõi và xử lý giao hàng có thể không hiệu quả nếu hệ thống thiếu công cụ tự động quản lý. Cuối cùng, trong hỗ trợ sau bán hàng, khách hàng có thể gặp khó khăn khi liên hệ hỗ trợ hoặc không nhận được phản hồi kịp thời.

Các vấn dề gặp phải trong quy trình

1.	Khó khăn trong tìm kiếm sản phẩm: Hệ thống không tối ưu hóa tìm kiếm và sắp xếp, gây trở ngại cho khách hàng.

2.	Quá trình đặt hàng kéo dài: Thiếu hỗ trợ tự động hoàn thành thông tin hoặc giao diện không thân thiện làm tăng thời gian đặt hàng.

3.	Chậm trễ trong xác nhận đơn hàng: Quy trình xác nhận thủ công làm giảm tốc độ xử lý và gây bất tiện cho khách hàng.

4.	Không chắc chắn về thanh toán: Tình trạng giao dịch không được cập nhật kịp thời gây lo lắng cho khách hàng.

5.	Theo dõi giao hàng không hiệu quả: Không có hệ thống theo dõi đơn hàng tự động khiến khách hàng không biết tình trạng giao hàng.

6.	Hỗ trợ sau bán hàng kém: Khách hàng khó liên hệ hỗ trợ hoặc không nhận được phản hồi nhanh, ảnh hưởng đến trải nghiệm.

Những vấn đề này làm giảm trải nghiệm người dùng, ảnh hưởng tiêu cực đến uy tín và doanh thu của doanh nghiệp.

Quy trình quản lý kế toán-tài chính
 
Quy trình quản lý kế toán-tài chính trước khi áp dụng ERP

Mô tả quy trình

Quy trình xử lý hóa đơn bắt đầu khi khách hàng nhận hóa đơn và thực hiện thanh toán khi nhận hàng hoặc chuyển khoản. Hóa đơn sau đó được gửi đến bộ phận kế toán qua email hoặc các phương tiện truyền thông khác. Tiếp theo, nhân viên kế toán kiểm tra thông tin trên hóa đơn để đảm bảo tính chính xác. Sau đó, kế toán thực hiện đối chiếu thanh toán giữa khoản thanh toán từ khách hàng và hóa đơn. Sau khi hoàn tất đối chiếu, nhân viên lưu hóa đơn vào hệ thống lưu trữ. Cuối cùng, vào cuối tháng, nhân viên kế toán lập báo cáo tài chính dựa trên các thông tin từ hóa đơn.

Các vấn đề gặp phải trong quy trình

1.	Gửi hóa đơn thiếu tính hệ thống: Hóa đơn được truyền qua các phương tiện không tập trung, dễ thất lạc và khó kiểm soát.

2.	Đối chiếu thủ công mất thời gian: Việc kiểm tra và đối chiếu hóa đơn với thanh toán không được tự động hóa, dễ gây nhầm lẫn và sai sót.

3.	Lưu trữ không hiệu quả: Phương pháp lưu trữ thủ công khiến việc truy xuất hóa đơn tốn thời gian và không đáng tin cậy.

4.	Lập báo cáo tài chính phức tạp: Quá trình này phụ thuộc vào dữ liệu thủ công, mất nhiều thời gian và có nguy cơ sai lệch, ảnh hưởng đến độ chính xác của báo cáo.

Những vấn đề này không chỉ làm giảm hiệu suất làm việc của bộ phận kế toán mà còn tiềm ẩn nguy cơ ảnh hưởng đến hoạt động tài chính của doanh nghiệp.
Quy trình trả hàng
Sơ đồ quy trình
 

Mô tả quy trình
Quy trình trả hàng bắt đầu khi khách hàng mang sản phẩm đến cửa hàng và gửi yêu cầu trả hàng cùng hóa đơn hoặc bằng chứng mua hàng. Nhân viên cửa hàng sau đó tiến hành kiểm tra hóa đơn để xác minh tính hợp lệ. Nếu hóa đơn không hợp lệ, quy trình kết thúc với việc thông báo từ chối yêu cầu cho khách hàng. Nếu hóa đơn hợp lệ, nhân viên tiếp tục kiểm tra sản phẩm trả lại để đánh giá tình trạng sản phẩm (độ mới, lỗi, v.v.) và đối chiếu với chính sách trả hàng. Nếu sản phẩm không đáp ứng chính sách, khách hàng cũng được thông báo từ chối yêu cầu. Trong trường hợp yêu cầu trả hàng cần sự phê duyệt đặc biệt, quản lý cửa hàng sẽ tham gia để xem xét và quyết định. Nếu tất cả yêu cầu đều được đáp ứng, nhân viên cửa hàng xử lý hoàn tiền hoặc đổi sản phẩm tùy theo mong muốn của khách hàng. Quy trình kết thúc sau khi hoàn tất các thủ tục trả hàng.
3.5.3 Các vấn đề gặp phải trong quy trình
1.	Xác minh hóa đơn thủ công: Việc kiểm tra hóa đơn hoặc bằng chứng mua hàng bằng tay dễ xảy ra sai sót hoặc kéo dài thời gian xử lý.
2.	Kiểm tra sản phẩm không rõ ràng: Tiêu chí đánh giá sản phẩm có thể không đồng nhất, dẫn đến các quyết định không minh bạch và gây bất mãn cho khách hàng.
3.	Chính sách trả hàng phức tạp: Nếu chính sách không rõ ràng hoặc thiếu thông tin công khai, khách hàng dễ cảm thấy bị thiệt thòi khi yêu cầu bị từ chối.
4.	Phê duyệt thủ công: Trong trường hợp cần sự phê duyệt từ quản lý, quy trình có thể bị chậm trễ nếu quản lý không có mặt hoặc thiếu thông tin.
5.	Xử lý tài chính thủ công: Hoàn tiền hoặc đổi sản phẩm được thực hiện thủ công, dễ xảy ra sai sót và thiếu minh bạch.
6.	Thiếu thông tin theo dõi: Toàn bộ quá trình không được ghi nhận một cách hệ thống, gây khó khăn trong việc xử lý các tranh chấp hoặc kiểm tra sau này.
Những vấn đề này không chỉ làm chậm quy trình trả hàng mà còn có thể ảnh hưởng đến sự hài lòng của khách hàng và uy tín của cửa hàng.
3.6. Quy trình tuyển dụng
3.6.1 Sơ đồ quy trình
 
3.6.1 Quy trình tuyển dụng trước khi áp dụng ERP
3.6.2 Mô tả quy trình
Quy trình tuyển dụng bắt đầu khi bộ phận yêu cầu tuyển dụng đề xuất nhu cầu và cung cấp thông tin chi tiết như mô tả công việc và số lượng cần tuyển. Nhân sự tiếp nhận yêu cầu, sau đó trình lên quản lý cấp cao để kiểm tra và phê duyệt nhằm đảm bảo phù hợp với ngân sách và nhu cầu. Nếu được phê duyệt, nhân sự tiến hành soạn thảo và đăng tin tuyển dụng trên các kênh phù hợp. Sau khi thu thập hồ sơ, nhân sự sàng lọc để lựa chọn ứng viên đáp ứng yêu cầu cơ bản, đồng thời gửi thông báo từ chối cho hồ sơ không đạt. Ứng viên đạt yêu cầu sẽ được mời tham gia phỏng vấn do nhân sự tổ chức, với sự tham gia đánh giá của quản lý trực tiếp. Kết quả phỏng vấn quyết định ứng viên có được chuyển sang giai đoạn thử việc hay không. Trong thời gian thử việc, ứng viên thực hiện các nhiệm vụ theo yêu cầu và được quản lý trực tiếp đánh giá hiệu suất. Nếu ứng viên đạt yêu cầu, quy trình tiếp tục với việc ký hợp đồng chính thức. Ngược lại, ứng viên sẽ nhận được thông báo chấm dứt thử việc. Quy trình kết thúc khi ứng viên ký hợp đồng chính thức hoặc từ chối lời mời làm việc.
3.6.3 Các vấn đề trong quy trình
1.	Thời gian phê duyệt kéo dài: Quá trình duyệt yêu cầu tuyển dụng từ quản lý cấp cao có thể chậm trễ, ảnh hưởng đến thời gian triển khai tuyển dụng.
2.	Sàng lọc hồ sơ chưa hiệu quả: Khối lượng lớn hồ sơ ứng viên đôi khi khiến nhân sự khó đảm bảo độ chính xác, dẫn đến bỏ sót ứng viên tiềm năng hoặc chọn sai người không phù hợp.
3.	Quản lý thông tin chưa đồng bộ: Thông tin từ các bước như phê duyệt, sàng lọc, và đánh giá có thể không được chia sẻ kịp thời giữa các bên liên quan, gây khó khăn trong việc phối hợp.
4.	Quy trình phỏng vấn thiếu nhất quán: Đôi khi không có tiêu chí đánh giá rõ ràng hoặc sự không đồng nhất giữa quản lý trực tiếp và nhân sự trong việc nhận xét ứng viên.
5.	Giai đoạn thử việc chưa tối ưu: Việc đánh giá hiệu suất trong thời gian thử việc có thể không rõ ràng hoặc thiếu sự hướng dẫn cụ thể, dẫn đến quyết định tuyển dụng không chính xác.
6.	Ứng viên từ chối lời mời: Nếu không xử lý tốt các bước tương tác với ứng viên, có thể dẫn đến việc họ từ chối cơ hội sau khi được chọn.
 
CHƯƠNG 4 BỐI CẢNH DOANH NGHIỆP SAU KHI ÁP DỤNG ERP
4.1. Quy trình quản lý chuỗi cung ứng
4.1.1 Sơ đồ quy trình
 
4.1.1 Quy trình quản lý chuỗi cung ứng sau khi triển khai ERP
4.1.2 Mô tả quy trình
Quy trình xử lý đơn hàng bắt đầu khi nhà cung cấp nhận đơn đặt hàng từ khách hàng thông qua hệ thống ERP, đảm bảo ghi nhận thông tin tự động để giảm sai sót và tăng tốc độ xử lý. Tiếp theo, hệ thống kiểm tra tính khả dụng của hàng hóa và xác nhận đơn hàng một cách nhanh chóng, chính xác. Đơn hàng sau đó được gửi đến quản lý để phê duyệt thông qua tính năng phê duyệt trực tuyến, giúp rút ngắn thời gian chờ đợi. Sau khi phê duyệt, nhà cung cấp chuẩn bị và giao hàng, với quá trình được giám sát qua hệ thống ERP để đảm bảo thời gian giao hàng chính xác. Khi hàng hóa được nhận, nhân viên kiểm tra số lượng và chất lượng, đồng thời cập nhật kết quả kiểm tra vào hệ thống để phát hiện vấn đề kịp thời. Thông tin về tình trạng đơn hàng được đồng bộ hóa tự động, đảm bảo các bộ phận liên quan đều nắm rõ trạng thái. Cuối cùng, hệ thống gửi thông báo tự động đến các bên liên quan.
4.2. Quy trình bán hàng
4.2.1 Sơ đồ quy trình
 
4.2.1 Quy trình bán hàng sau khi triển khai ERP
4.2.2 Mô tả quy trình
Quy trình mua sắm trực tuyến qua hệ thống ERP bắt đầu khi khách hàng truy cập website với giao diện thân thiện, được tối ưu hóa để tìm kiếm và chọn sản phẩm dễ dàng. Hệ thống cung cấp bộ lọc thông minh và gợi ý sản phẩm dựa trên hành vi của khách hàng, với thông tin chi tiết, hình ảnh chất lượng và đánh giá rõ ràng. Sau khi chọn sản phẩm, khách hàng thực hiện đặt hàng. Hệ thống ERP tự động kiểm tra tính đầy đủ của thông tin, thông báo ngay nếu có thiếu sót, và tích hợp các phương thức thanh toán đa dạng. Tình trạng thanh toán được cập nhật ngay lập tức, và khách hàng nhận thông báo qua email hoặc trên trang web.
Khi đơn hàng được thanh toán, hệ thống ERP kích hoạt quy trình xác nhận tự động, giúp nhân viên giảm thời gian xử lý và đảm bảo khách hàng nhận được thông tin xác nhận ngay lập tức. Giai đoạn giao hàng được quản lý và theo dõi chặt chẽ qua hệ thống ERP, cho phép khách hàng cập nhật trạng thái đơn hàng trực tuyến và nhận thông báo về thời gian giao hàng dự kiến. Sau khi giao hàng, hệ thống hỗ trợ dịch vụ sau bán hàng qua nhiều kênh như chat trực tuyến, email hoặc điện thoại, giúp giải quyết các vấn đề phát sinh nhanh chóng và hiệu quả.

4.3. Quy trình quản lý kế toán-tài chính
4.3.1 Sơ đồ quy trình
 
4.3.1 Quy trình quản lý kế toán-tài chính sau khi triển khai ERP
4.3.2 Mô tả quy trình
Quy trình quản lý hóa đơn sau khi triển khai hệ thống ERP bắt đầu khi khách hàng thanh toán thông qua hình thức thanh toán khi nhận hàng hoặc chuyển khoản. Ngay sau khi thanh toán được thực hiện, hóa đơn sẽ được tự động gửi vào hệ thống ERP, loại bỏ sự phụ thuộc vào nhập liệu thủ công và giảm thiểu sai sót. Hệ thống ERP ghi nhận và lưu trữ thông tin hóa đơn một cách hiệu quả, cho phép nhân viên kế toán dễ dàng truy cập và kiểm tra thông tin khi cần.
Hệ thống cũng tự động đối chiếu thanh toán từ khách hàng với các hóa đơn đã ghi nhận, giúp quy trình đối chiếu diễn ra nhanh chóng, chính xác và giảm thiểu rủi ro sai sót. Các hóa đơn sau đó được lưu trữ tự động trong hệ thống, đảm bảo dữ liệu được tổ chức chặt chẽ và thuận tiện cho việc tra cứu sau này. Định kỳ, hệ thống ERP tự động tổng hợp và tạo báo cáo tài chính dựa trên các dữ liệu đã ghi nhận, giúp doanh nghiệp tiết kiệm thời gian và nâng cao hiệu quả quản lý tài chính.

4.4. Quy trình trả hàng
4.4.1 Sơ đồ quy trình
 
4.4.1 Quy trình trả hàng sau khi triển khai ERP
4.4.2 Mô tả quy trình
Quy trình xử lý trả hàng bắt đầu khi khách hàng mang sản phẩm đến cửa hàng và cung cấp thông tin giao dịch như hóa đơn, số điện thoại hoặc mã đơn hàng. Nhân viên sử dụng module Sales hoặc POS (Point of Sale) của Odoo để tra cứu lịch sử mua hàng và kiểm tra hóa đơn cùng các điều kiện trả hàng dựa trên chính sách được cấu hình sẵn trong hệ thống. Sau đó, nhân viên tiến hành kiểm tra sản phẩm trả lại theo các tiêu chí như tình trạng sản phẩm và thời gian trả hàng, với kết quả được ghi nhận trực tiếp trên Odoo.
Nếu cần phê duyệt từ quản lý, yêu cầu sẽ được gửi qua module Approvals, cho phép quản lý phê duyệt hoặc từ chối trực tiếp trên hệ thống, giảm thiểu thời gian chờ. Sau khi phê duyệt, nhân viên cập nhật trạng thái sản phẩm trả về kho thông qua module Inventory và thực hiện hoàn tiền hoặc đổi hàng qua module Accounting hoặc POS, đảm bảo tất cả thông tin được tự động ghi nhận. Cuối cùng, hệ thống tự động gửi email hoặc SMS thông báo cho khách hàng về trạng thái xử lý trả hàng. Ngoài ra, các dữ liệu liên quan đến trả hàng được phân tích qua module Reporting hoặc BI để đánh giá nguyên nhân, tỷ lệ trả hàng và các vấn đề liên quan, hỗ trợ cải thiện quy trình và dịch vụ.
4.5. Quy trình tuyển dụng
4.5.1 Sơ đồ quy trình
 
4.5.1 Quy trình tuyển dụng sau khi triển khai ERP
4.5.2 Mô tả quy trình
Quy trình tuyển dụng qua Odoo bắt đầu khi bộ phận yêu cầu gửi đề xuất tuyển dụng bằng module Recruitment, kèm theo mô tả công việc và số lượng cần tuyển. Yêu cầu này được quản lý cấp cao phê duyệt trực tiếp trên hệ thống sau khi nhận thông báo tự động. Nếu được duyệt, module Recruitment tự động đăng tin tuyển dụng trên các kênh tích hợp như website công ty, LinkedIn, hoặc các trang tuyển dụng. Hồ sơ ứng viên sau đó được gửi trực tiếp vào hệ thống Odoo, nơi nhân sự sàng lọc và đánh giá để chọn ra những ứng viên phù hợp.
Nhân sự sử dụng Odoo để lên lịch phỏng vấn, thông báo đến ứng viên và ban phỏng vấn, đồng thời ghi nhận kết quả đánh giá của quản lý trực tiếp trong hệ thống. Các ứng viên đạt yêu cầu sẽ được chuyển sang giai đoạn thử việc, nơi quản lý trực tiếp theo dõi và nhập nhận xét về kết quả thử việc vào hệ thống thông qua module HR. Nếu thử việc đạt yêu cầu, quy trình tiếp tục với việc chuẩn bị hợp đồng chính thức. Module Recruitment hỗ trợ tạo hợp đồng tự động, gửi qua email hoặc hệ thống để ứng viên ký số, hoàn tất quá trình tuyển dụng một cách nhanh chóng và hiệu quả.










