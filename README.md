---


---

<h1 id="session01_ex07-data-masking-và-de-masking">SESSION01_EX07: DATA MASKING VÀ DE-MASKING</h1>
<h2 id="phần-a.-masking-table-bảng-che-mờ-dữ-liệu">Phần A. Masking Table (Bảng che mờ dữ liệu)</h2>

<table>
<thead>
<tr>
<th>Thông tin PII thật</th>
<th>Nhãn Placeholder</th>
<th>Loại dữ liệu</th>
</tr>
</thead>
<tbody>
<tr>
<td>Phạm Minh C</td>
<td>[CUSTOMER_NAME]</td>
<td>Họ tên</td>
</tr>
<tr>
<td>0988.111.222</td>
<td>[PHONE]</td>
<td>Số điện thoại</td>
</tr>
<tr>
<td><a href="mailto:minhc@gmail.com">minhc@gmail.com</a></td>
<td>[EMAIL]</td>
<td>Email</td>
</tr>
<tr>
<td>Căn hộ 502 Chung cư Sunrise, Q7</td>
<td>[ADDRESS]</td>
<td>Địa chỉ</td>
</tr>
</tbody>
</table><h2 id="phần-b.-masked-input-dữ-liệu-đã-che-mờ">Phần B. Masked Input (Dữ liệu đã che mờ)</h2>
<p>“Tôi là [CUSTOMER_NAME] (SĐT: [PHONE], Email: [EMAIL], ở [ADDRESS]). Ngày 20/09 tôi mua 2kg thịt bò Wagyu giá 4.500.000 VNĐ tại MartX District 7 nhưng bị giao chậm 3 tiếng làm hỏng tiệc gia đình. Tôi yêu cầu bồi thường 100%!”</p>
<h2 id="phần-c.-prompt-gửi-ai">Phần C. Prompt gửi AI</h2>
<pre><code>Bạn là nhân viên chăm sóc khách hàng của MartX.

Hãy soạn thư xin lỗi khách hàng dựa trên nội dung khiếu nại đã cung cấp.

Yêu cầu:
- Thể hiện thái độ lịch sự, chân thành.
- Xin lỗi vì giao hàng chậm 3 tiếng.
- Thể hiện sự thông cảm với khách hàng.
- Đề xuất xem xét bồi thường 100%.
- Không tự ý hứa chắc chắn khi chưa được phê duyệt.
- Giữ nguyên các nhãn Placeholder.
- Không tự tạo thêm thông tin.
</code></pre>
<h2 id="phần-d.-văn-bản-de-masking-thư-sau-khi-khôi-phục-dữ-liệu">Phần D. Văn bản De-masking (Thư sau khi khôi phục dữ liệu)</h2>
<p><strong>Tiêu đề: Thư xin lỗi về sự cố giao hàng</strong></p>
<p>Kính gửi anh Phạm Minh C,</p>
<p>MartX chân thành xin lỗi anh vì đơn hàng thịt bò Wagyu ngày 20/09 bị giao chậm 3 tiếng, làm ảnh hưởng đến bữa tiệc gia đình của anh.</p>
<p>Chúng tôi rất tiếc về sự bất tiện này và sẽ kiểm tra sự việc, đồng thời xem xét yêu cầu bồi thường 100% của anh.</p>
<p>Thông tin khách hàng:</p>
<ul>
<li>
<p>Họ tên: Phạm Minh C</p>
</li>
<li>
<p>Số điện thoại: 0988.111.222</p>
</li>
<li>
<p>Email: <a href="mailto:minhc@gmail.com">minhc@gmail.com</a></p>
</li>
<li>
<p>Địa chỉ: Căn hộ 502 Chung cư Sunrise, Q7.</p>
</li>
</ul>
<p>MartX mong nhận được sự thông cảm từ anh và cam kết cải thiện chất lượng dịch vụ.</p>
<p>Trân trọng,</p>
<p><strong>Bộ phận Chăm sóc khách hàng MartX</strong></p>

