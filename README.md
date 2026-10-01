# CLAIDE-CFA – AgriPack: phản biện, mô hình định giá và báo cáo dạng CFA RC

Bài tập lớn học phần TTKN (định giá startup CTCP AgriPack). Người phản biện, lập mô hình và dàn báo cáo: Lộc.

## Sản phẩm (thư mục `deliverables/`)

| File | Nội dung |
|---|---|
| `AgriPack_CFA_Report.html` | Báo cáo dạng CFA Research Challenge (16 trang thân + 8 trang phụ lục A4, 59 Fig. ở phần thân và 15 Fig. phụ lục, biểu đồ ở cột trái). Mục 1–3 giữ nguyên văn bài TTKN_2 của nhóm; Mục 4 (dự phóng), 5 (định giá), 8 (bonus: định giá khi chưa có doanh thu) và phụ lục viết từ mô hình. Mục 6–7 không thuộc phạm vi. Mở bằng trình duyệt; in PDF bằng Ctrl+P (A4, bật "Background graphics"). |
| `AgriPack_CFA_Report.pptx` | Chính báo cáo HTML ở trên chuyển sang PowerPoint: 24 slide khổ A4 dọc, mỗi slide một trang; chữ, bảng, biểu đồ chỉnh sửa được, mỗi biểu đồ là một group. |
| `AgriPack_Model_final.xlsx` | Chính file model bạn gửi lại (AgriPack_Model_final_1.xlsx, giữ nguyên các chỗ đã sửa tay), đã áp các thay đổi mới. Mô hình dựng trên file Excel mẫu của giảng viên: Drivers → Pro Forma → 3 BCTC 2026E–2030E → Discount rate → DCF, VC Method, Multiples → Summary, Sensitivity, Checks. Nguồn và lý do của mỗi giả định ghi ngay ô bên cạnh (Drivers cột K, Discount rate cột C, Assumption cột E, VCM, Multiples cột K, Summary cột D/G/N). Sheet Multiples có khối kết quả như DCF và VCM (A44:E52: giá trị doanh nghiệp, pre-money, post-money, nhu cầu vốn, tỷ lệ cổ phần). Summary xếp ba phương pháp ở hàng 5–7 (DCF, VC Method, Multiples), pre-money khuyến nghị ở hàng 8. `Chart_Data` chứa dữ liệu của từng Fig. (Fig_01 … Fig_59, Fig_A01 … Fig_A15). |
| `AgriPack_CFA_Report.pdf` | Bản PDF xem trước của báo cáo HTML (cùng phiên bản). |
| `TTKN_1_Loc_phan_bien.docx` | Bản nháp đầu của nhóm kèm 93 comment phản biện của Lộc. |
| `AgriPack_Series_A_Thuyet_trinh.pptx` | Bản thuyết trình của phiên bản đầu (v1). **Không cập nhật** theo TTKN_2 vì Mục 6–7 (huy động vốn, pitching) ngoài phạm vi; số liệu trong file này đã cũ. |

## Kết quả chính (kịch bản cơ sở, t0 = 01/01/2026)

- Doanh thu 47,5 tỷ (2025A) → 170,3 tỷ (2030E), CAGR 29,1%; biên EBITDA 16,2% → 20,2%.
- BCKQKD theo chức năng (VAS): 70% tiền lương và 90% khấu hao vào giá vốn, 30% và 10% vào CPBH & QLDN, áp dụng cả 2023–2025; biên gộp 51,0% (2025A) → 44,8% (2028E) → 47,6% (2030E).
- Tỷ lệ tái đầu tư (CAPEX/doanh thu) 20% – 65% – 12% – 10% – 10% (2026–2030), so với trung vị 3,1% và P75 8,3% của 16 DN bao bì niêm yết; FCFF âm 2026–2028.
- WACC 13,6%: Rf 3,92% = bình quân lợi suất TPCP 10 năm 2016–2025, ERP Việt Nam 8,13%, beta tổng 1,48, Ke = Rf + β × (Rm − Rf) = 15,9%, Kd 10%; g = 5%.
- Giá trị cuối kỳ giữ công thức của file mẫu, FCFF 2031/(WACC − g); FCFF 2031 được chuẩn hóa với RONIC bằng ROIC 2030 của mô hình (13,9%), không thêm giả định mới.
- VC Method: z = 40% theo hướng dẫn của đề bài cho giai đoạn đầu tăng trưởng; p = (1 + r)/(1 − z)^(1/n) − 1 = 25,9% (công thức giáo trình).
- DCF 32,8 tỷ; VC Method 25,3 tỷ; Multiples 27,7 tỷ (EV/EBITDA, P/E 2025A, chiết khấu thanh khoản 30%; giá trị doanh nghiệp 26,4 tỷ, post-money 65,3 tỷ, nhà đầu tư mới nắm 57,6%). Pre-money bình quân 40/40/20: **28,8 tỷ** (khoảng 17,7–43,7 tỷ), gần bằng vốn chủ sở hữu sổ sách (30,0 tỷ).
- Độ nhạy theo nhân tố vĩ mô – ngành (chạy lại toàn bộ mô hình): sản lượng ×0,8/×1,2 làm pre-money −27,6/+32,3 tỷ, trong khi lãi suất hay CRP ±1 điểm % chỉ làm pre-money thay đổi khoảng 5–6 tỷ. Kịch bản xấu (Bear): −25,8 tỷ; tốt (Bull): 76,2 tỷ; đầu tư lớn năm 2028: 19,2 tỷ.
- Nhu cầu vốn: 37,6 tỷ vốn cổ phần (2026) và 31,1 tỷ vay trung hạn (2027).

## Cần kiểm tra trước khi nộp

- Phần bù rủi ro quốc gia 3,9% là ước tính theo phương pháp Damodaran cho hạng Ba2.
- Rf: các quan sát 2016, 2017 và 2023 là lãi suất phát hành/trúng thầu (không phải lợi suất thứ cấp cuối năm).
- Đề bài ghi đầu tư lớn năm 2027, file Excel mẫu khóa 65% ở năm 2028; mô hình theo đề bài, phương án 2028 chạy bằng ô `Drivers!C4`.
- Tên nhà máy, khu công nghiệp và khách hàng trong sơ đồ chuỗi giá trị (Fig. A02) là giả định minh họa.
- Đã sửa trong bài nhóm: Nghị quyết 28/2022/NQ-HĐND → Nghị định 08/2022/NĐ-CP (Điều 64); số IMARC bị lặp ở Mục 3.2 thay bằng số bao bì F&B phân hủy sinh học (33,93 → 51,45 triệu USD, CAGR 4,73%); thị phần SAM F&B thống nhất 4,3% (miền Trung – Nam ~5,8%); Tetra Pak là tập đoàn đa quốc gia; lỗi chính tả ("đối mặt", "BioWraps", "HAPBIO"); Mục 2.6 dẫn sang Mục 4, 5 thay vì "Phần 6". Còn lại cần nhóm tự kiểm tra: năm tài liệu UNEP (2021 hay 2022) và tiêu đề bài Wagner & Zanger (2023) theo DOI.
