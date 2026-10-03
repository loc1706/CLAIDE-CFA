# CLAIDE-CFA – AgriPack: phản biện, mô hình định giá và báo cáo dạng CFA RC

Bài tập lớn học phần TTKN (định giá startup CTCP AgriPack). Người phản biện, lập mô hình và dàn báo cáo: Lộc.

## Sản phẩm (thư mục `deliverables/`)

| File | Nội dung |
|---|---|
| `AgriPack_CFA_Report.html` | **Chưa dựng lại theo model ngày 03/10/2026** (báo cáo vẫn dùng Rf bình quân 3,92% và pre-money 28,8 tỷ). Báo cáo dạng CFA Research Challenge (16 trang thân + 8 trang phụ lục A4, 59 Fig. ở phần thân và 15 Fig. phụ lục, biểu đồ ở cột trái). Mục 1–3 giữ nguyên văn bài TTKN_2 của nhóm; Mục 4 (dự phóng), 5 (định giá), 8 (bonus: định giá khi chưa có doanh thu) và phụ lục viết từ mô hình. Mục 6–7 không thuộc phạm vi. Mở bằng trình duyệt; in PDF bằng Ctrl+P (A4, bật "Background graphics"). |
| `AgriPack_CFA_Report.pptx` | Chính báo cáo HTML ở trên chuyển sang PowerPoint: 24 slide khổ A4 dọc, mỗi slide một trang; chữ, bảng, biểu đồ chỉnh sửa được, mỗi biểu đồ là một group. |
| `AgriPack_Model_final.xlsx` | Chính file model bạn gửi lại (AgriPack_Model_final_1.xlsx, giữ nguyên các chỗ đã sửa tay), đã áp các thay đổi mới. Sheet đầu `Trang bìa` gồm mô tả, mã màu, cấu trúc các tab và thông tin mô hình; toàn file dùng Calibri 12, tắt gridlines, ghi chú tô nền xanh nhạt, ô cần kiểm tra (Rf, CRP) chữ đỏ nền cam. Mô hình dựng trên file Excel mẫu của giảng viên: Drivers → Pro Forma → 3 BCTC 2026E–2030E → Discount rate → DCF, VC Method, Multiples → Summary, Sensitivity, Checks. Nguồn và lý do của mỗi giả định ghi ngay ô bên cạnh (Drivers cột K, Discount rate cột C, Assumption cột E, VCM, Multiples cột K, Summary cột D/G/N). Công thức chỉ dùng hàm cơ bản: phép cộng dùng SUM, ngoài ra chỉ có IF, MAX/MIN, CHOOSE, NPV, AVERAGE/MEDIAN, ROUND (ghi ở sheet Ghi chu, dòng 30). Sheet Multiples có khối kết quả như DCF và VCM (A44:E52: giá trị doanh nghiệp, pre-money, post-money, nhu cầu vốn, tỷ lệ cổ phần). Summary xếp ba phương pháp ở hàng 5–7 (DCF, VC Method, Multiples), pre-money khuyến nghị ở hàng 8. `Chart_Data` chứa dữ liệu của từng Fig. (Fig_01 … Fig_59, Fig_A01 … Fig_A15). |
| `AgriPack_CFA_Report.pdf` | Bản PDF xem trước của báo cáo HTML (cùng phiên bản). |
| `TTKN_1_Loc_phan_bien.docx` | Bản nháp đầu của nhóm kèm 93 comment phản biện của Lộc. |
| `AgriPack_Series_A_Thuyet_trinh.pptx` | Bản thuyết trình của phiên bản đầu (v1). **Không cập nhật** theo TTKN_2 vì Mục 6–7 (huy động vốn, pitching) ngoài phạm vi; số liệu trong file này đã cũ. |

## Kết quả chính (kịch bản cơ sở, t0 = 01/01/2026)

- Doanh thu 47,5 tỷ (2025A) → 170,3 tỷ (2030E), CAGR 29,1%; biên EBITDA 16,2% → 20,2%.
- BCKQKD theo chức năng (VAS): 70% tiền lương và 90% khấu hao vào giá vốn, 30% và 10% vào CPBH & QLDN, áp dụng cả 2023–2025; biên gộp 51,0% (2025A) → 44,8% (2028E) → 47,6% (2030E).
- Tỷ lệ tái đầu tư (CAPEX/doanh thu) 20% – 65% – 12% – 10% – 10% (2026–2030), so với trung vị 3,1% và P75 8,3% của 16 DN bao bì niêm yết; FCFF âm 2026–2028.
- WACC 14,1%: Rf 4,588% = lợi suất TPCP kỳ hạn 10 năm ngày 01/10/2026, ERP Việt Nam 8,13%, beta điều chỉnh 1,48, Ke = Rf + β × (Rm − Rf) = 16,6%, Kd 10%; g = 5%.
- Giá trị cuối kỳ giữ công thức của file mẫu, FCFF 2031/(WACC − g); FCFF 2031 được chuẩn hóa với RONIC bằng ROIC 2030 của mô hình (13,9%), không thêm giả định mới.
- VC Method: z = 40% theo hướng dẫn của đề bài cho giai đoạn đầu tăng trưởng; p = (1 + r)/(1 − z)^(1/n) − 1 = 26,4% (công thức giáo trình).
- DCF 28,4 tỷ; VC Method 24,0 tỷ; Multiples 27,7 tỷ (EV/EBITDA, P/E 2025A, chiết khấu thanh khoản 30%; giá trị doanh nghiệp 26,4 tỷ, post-money 65,3 tỷ, nhà đầu tư mới nắm 57,6%). Pre-money bình quân 40/40/20: **26,5 tỷ** (khoảng 15,8–40,4 tỷ), khoảng 0,88 lần vốn chủ sở hữu sổ sách (30,0 tỷ); nhà đầu tư mới nắm 58,7%.
- Độ nhạy theo nhân tố vĩ mô – ngành (chạy lại toàn bộ mô hình): sản lượng ×0,8/×1,2 làm pre-money −26,2/+30,6 tỷ, trong khi lãi suất hay CRP ±1 điểm % chỉ làm pre-money thay đổi khoảng 4–5 tỷ. Kịch bản xấu (Bear): −25,4 tỷ; tốt (Bull): 71,7 tỷ.
- Nhu cầu vốn: 37,6 tỷ vốn cổ phần (2026) và 31,1 tỷ vay trung hạn (2027).

## Cần kiểm tra trước khi nộp

- Phần bù rủi ro quốc gia 3,9% là ước tính theo phương pháp Damodaran cho hạng Ba2.
- Rf 4,588% (TPCP 10 năm ngày 01/10/2026) lấy từ Trading Economics qua kết quả tìm kiếm (4,5879% ngày 02/10/2026, tăng 0,0002 điểm % so với phiên 01/10); cần đối chiếu đường cong lợi suất HNX/VBMA ngày 01/10/2026.
- Tên nhà máy, khu công nghiệp và khách hàng trong sơ đồ chuỗi giá trị (Fig. A02) là giả định minh họa.
- Đã sửa trong bài nhóm: Nghị quyết 28/2022/NQ-HĐND → Nghị định 08/2022/NĐ-CP (Điều 64); số IMARC bị lặp ở Mục 3.2 thay bằng số bao bì F&B phân hủy sinh học (33,93 → 51,45 triệu USD, CAGR 4,73%); thị phần SAM F&B thống nhất 4,3% (miền Trung – Nam ~5,8%); Tetra Pak là tập đoàn đa quốc gia; lỗi chính tả ("đối mặt", "BioWraps", "HAPBIO"); Mục 2.6 dẫn sang Mục 4, 5 thay vì "Phần 6". Còn lại cần nhóm tự kiểm tra: năm tài liệu UNEP (2021 hay 2022) và tiêu đề bài Wagner & Zanger (2023) theo DOI.
