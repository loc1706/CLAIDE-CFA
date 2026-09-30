# CLAIDE-CFA – AgriPack: phản biện, mô hình định giá và báo cáo dạng CFA RC

Bài tập lớn học phần TTKN (định giá startup CTCP AgriPack). Người phản biện, lập mô hình và dàn báo cáo: Lộc.

## Sản phẩm (thư mục `deliverables/`)

| File | Nội dung |
|---|---|
| `AgriPack_CFA_Report.html` | Báo cáo dạng CFA Research Challenge (15 trang thân + 8 trang phụ lục A4, biểu đồ ở cột trái). Mục 1–3 giữ nguyên văn bài TTKN_2 của nhóm; Mục 4 (dự phóng), 5 (định giá), 8 (bonus: định giá khi chưa có doanh thu) và phụ lục viết từ mô hình. Mục 6–7 không thuộc phạm vi. Mở bằng trình duyệt; in PDF bằng Ctrl+P (A4, bật "Background graphics"). |
| `AgriPack_CFA_Report.pptx` | Chính báo cáo HTML ở trên chuyển sang PowerPoint: 23 slide khổ A4 dọc, mỗi slide một trang; chữ, bảng, biểu đồ chỉnh sửa được, mỗi biểu đồ là một group. |
| `AgriPack_Model_final.xlsx` | Mô hình dựng trên file Excel mẫu của giảng viên: Drivers → Pro Forma → 3 BCTC 2026E–2030E → Discount rate → DCF, VC Method, Multiples → Summary, Sensitivity, Checks. Nguồn và lý do của mỗi giả định ghi ngay ô bên cạnh (Drivers cột K, Discount rate cột C, Assumption cột E, VCM, Multiples cột K, Summary cột D/G/N). `Chart_Data` chứa dữ liệu của từng Fig. (Fig_01 … Fig_A15). |
| `AgriPack_CFA_Report.pdf` | Bản PDF xem trước của báo cáo HTML (cùng phiên bản). |
| `TTKN_1_Loc_phan_bien.docx` | Bản nháp đầu của nhóm kèm 93 comment phản biện của Lộc. |
| `AgriPack_Series_A_Thuyet_trinh.pptx` | Bản thuyết trình của phiên bản đầu (v1). **Không cập nhật** theo TTKN_2 vì Mục 6–7 (huy động vốn, pitching) ngoài phạm vi; số liệu trong file này đã cũ. |

## Kết quả chính (kịch bản cơ sở, t0 = 01/01/2026)

- Doanh thu 47,5 tỷ (2025A) → 170,3 tỷ (2030E), CAGR 29,1%; biên EBITDA 16,2% → 20,2%.
- BCKQKD theo chức năng (VAS): 70% tiền lương và 90% khấu hao vào giá vốn, 30% và 10% vào CPBH & QLDN, áp dụng cả 2023–2025; biên gộp 51,0% (2025A) → 44,8% (2028E) → 47,6% (2030E).
- Tỷ lệ tái đầu tư (CAPEX/doanh thu) 20% – 65% – 12% – 10% – 10% (2026–2030), so với trung vị 3,1% và P75 8,3% của 16 DN bao bì niêm yết; FCFF âm 2026–2028.
- WACC 13,6%: Rf 3,92% = bình quân lợi suất TPCP 10 năm 2016–2025, ERP Việt Nam 8,13%, total beta 1,48, Ke 15,9%, Kd 10%; g = 5%, RONIC 18%; tỷ lệ thất bại z = 40%.
- DCF 41,1 tỷ; VC Method 25,3 tỷ; Multiples 27,7 tỷ (EV/EBITDA, P/E 2025A, chiết khấu thanh khoản 30%). Pre-money bình quân 40/40/20: **32,1 tỷ** (khoảng 19,7–49,2 tỷ).
- Độ nhạy theo nhân tố vĩ mô – ngành (chạy lại toàn bộ mô hình): sản lượng ×0,8/×1,2 làm pre-money −24,3/+28,3 tỷ, trong khi lãi suất hay CRP ±1 điểm % chỉ làm pre-money thay đổi khoảng 5–7 tỷ. Kịch bản Bear: −16,1 tỷ; Bull: 73,6 tỷ; đầu tư lớn năm 2028: 26,3 tỷ.
- Nhu cầu vốn: 37,6 tỷ vốn cổ phần (2026) và 31,1 tỷ vay trung hạn (2027).

## Cần kiểm tra trước khi nộp

- Phần bù rủi ro quốc gia 3,9% là ước tính theo phương pháp Damodaran cho hạng Ba2; đối chiếu bảng CRP 01/2026.
- Rf: các quan sát 2016, 2017 và 2023 là lãi suất phát hành/trúng thầu (không phải lợi suất thứ cấp cuối năm).
- Đề bài ghi đầu tư lớn năm 2027, file Excel mẫu khóa 65% ở năm 2028; mô hình theo đề bài, phương án 2028 chạy bằng ô `Drivers!C4`.
- Tên nhà máy, khu công nghiệp và khách hàng trong sơ đồ chuỗi giá trị (Fig. A02) là giả định minh họa.
- Nội dung nhóm giữ nguyên văn, cần nhóm tự sửa: Nghị quyết 28/2022/NQ-HĐND (nên là Nghị định 08/2022/NĐ-CP, Điều 64); số liệu IMARC của thị trường bao bì phân hủy sinh học lặp lại đúng số của thị trường bao bì xanh (Mục 3.2); thị phần SAM F&B 4,3% (Mục 1) và 5,4% (Mục 2.1) chưa thống nhất; Tetra Pak được xếp vào doanh nghiệp nội địa; lỗi chính tả ("AgriPack mặt với", "BioWaps"/"BioWraps", "HAPIBO"/"HAPBIO"); năm tài liệu UNEP (2021 hay 2022); tiêu đề bài Wagner & Zanger (2023) cần đối chiếu theo DOI; câu nhắc "Phần 6" ở Mục 2.6.
