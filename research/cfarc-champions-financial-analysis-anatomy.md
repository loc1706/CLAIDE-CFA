# Giải phẫu cách các bài vô địch CFA Institute Research Challenge (CFARC) phân tích tài chính

> **Phạm vi:** 8 báo cáo viết (written report) vô địch toàn cầu 2019 → 2026, tải trực tiếp từ trang [Past Champions của CFA Institute](https://www.cfainstitute.org/insights/events/research-challenge/past-champions), trích text và đọc kỹ các phần *Investment Summary*, *Financial Analysis*, *Valuation*, *Investment Risks* và *Appendix*.
> **Mục tiêu:** chỉ ra **họ làm gì, làm theo thứ tự nào, vì sao cách đó thắng**, rồi rút thành checklist và template để áp dụng cho một báo cáo kiểu DGW (Digiworld) như mẫu bạn gửi.
>
> *Ghi chú:* số liệu dưới đây lấy từ text trích ra từ PDF. Một số con số chỉ nằm trong biểu đồ dạng ảnh nên không trích được; những chỗ đó mình mô tả định tính.

---

## 0. TL;DR: 10 điều làm nên bài vô địch

1. **Phân tích tài chính dùng để *chứng minh thesis*, không để kể lại lịch sử.** Mỗi bảng hay biểu đồ đều trả lời một câu hỏi của thesis. Ví dụ Waterloo 2026: *“Thesis #2: Inorganic growth has masked subpar organic execution”*, rồi họ tách hẳn doanh thu organic và M&A để chứng minh.
2. **Bảng DuPont + ROIC + Liquidity + Leverage gần như là “form chuẩn”**: 2024, 2025, 2026 dùng *cùng một bảng* gồm 5 năm lịch sử và 5 năm dự phóng.
3. **ROIC so với WACC là trục chính** để kết luận công ty tạo hay phá giá trị (Cargojet 2024, Qantas 2023, Lightspeed 2026).
4. **Dự phóng theo driver (driver-based) gắn với KPI ngành**: ASK×RASK cho hàng không, deliveries×giá cho bất động sản, customers×ARPU và GPV×take-rate cho SaaS/payments, MW×giá/MW cho tuabin gió, NIM/AIEA cho ngân hàng. Không ai dự phóng bằng một tỷ lệ tăng trưởng chung chung, trừ khi giải thích được vì sao dữ liệu không cho phép làm khác (Cargojet).
5. **Có ít nhất 2 phương pháp terminal value và luôn đối chiếu chéo**: dùng terminal growth thì ra *implied exit multiple*, dùng exit multiple thì ra *implied growth*. Họ cũng nêu *% giá trị nằm ở terminal value*.
6. **Mọi giả định chi phí vốn đều được tam giác hoá** bằng nhiều cách tính beta, CoE và Kd, rồi **chọn phương án bảo thủ có giải thích**.
7. **Reverse DCF** (2023, 2024, 2026) cho thấy thị trường đang ngầm định điều gì, và đó chính là *variant perception*.
8. **Kiểm định độ vững nhiều tầng**: bảng độ nhạy 2 chiều, bull/base/bear, Monte Carlo (10k đến 1 triệu lần lặp), valuation waterfall, Brownian motion và VaR.
9. **Mỗi rủi ro đều được lượng hoá tác động lên giá mục tiêu**, ví dụ *“5% decline in revenue → −28.5% share price”*, kèm biện pháp giảm thiểu (mitigant).
10. **Có primary research thật**: phỏng vấn chuyên gia, khảo sát khách hàng (n=97), đọc 1.766 khiếu nại BBB, 645 review nhân viên. Đây là thứ làm số liệu tài chính có “hồn” và khó bắt chước.

---

## 1. Bộ mẫu: 8 bài vô địch

| Năm | Trường | Công ty (ngành) | Khuyến nghị | TP / Upside | Phương pháp chính & trọng số |
|---|---|---|---|---|---|
| 2026 | Univ. of Waterloo | Lightspeed Commerce – LSPD (PoS/Payments SaaS) | **SELL** | $10 / −21% | **Levered DCF 10 năm (FCFE)**: 50% terminal growth, 50% exit P/E. Comps 0% |
| 2025 | Kozminski Univ. | Dom Development – DOM (BĐS nhà ở Ba Lan) | BUY | PLN 260 / +22% | **DCF FCFF 100%**; SOTP, DDM, Comps dùng để kiểm chứng |
| 2024 | Univ. of Waterloo | Cargojet – CJT (hàng không vận tải) | BUY | $150 / +23% | DCF 5 năm 80% (40% TG, 40% exit EV/EBITDA) + Comps EV/NTM EBITDA 20% |
| 2023 | Univ. of Sydney | Qantas – QAN (hàng không) | BUY | A$6.41 / +22.3% | DCF FCFF 2 giai đoạn 70% + Relative EV/EBITDA 30% |
| 2022 | Northern Illinois Univ. | Motorola Solutions – MSI (thiết bị/phần mềm an ninh công) | BUY | $287 / **+6.5%** | DCF FCFF; Monte Carlo, DDM, Relative dùng để kiểm chứng |
| 2021 | BI Norwegian BS | Vestas – VWS (tuabin gió) | BUY | DKK 1480 / +21% | DCF FCFF; Monte Carlo, kịch bản, Relative |
| 2020 | Univ. of Sydney | Commonwealth Bank – CBA (ngân hàng) | **SELL** | A$70.08 / −12.2% | **RIM 30% + DDM 10% + Relative 60%** (có giá trị franking credit) |
| 2019 | Ateneo de Manila | D&L Industries – DNL (hoá chất đặc biệt, Philippines) | BUY | Php 13.30 / +27.8% | DCF (WACC 9%, g 3.5%); Relative P/E, PEG, P/S; SOTP ở phụ lục |

**Quan sát nhanh:**
- **2 trong 8 bài là SELL.** Ban giám khảo không thưởng cho “upside lớn”. MSI 2022 thắng với upside chỉ **6.5%**. Thứ được thưởng là **chất lượng lập luận và tính nhất quán giữa thesis, số liệu và định giá**.
- Không có “phương pháp vô địch” cố định. Phương pháp được **chọn theo bản chất doanh nghiệp**: ngân hàng dùng RIM/DDM/P/BV, công ty chưa có lãi ổn định dùng levered DCF + P/E exit, bất động sản theo dự án dùng SOTP, công ty chia cổ tức đều dùng DDM để đối chiếu.

---

## 2. Nguyên lý xương sống: chuỗi Thesis → Driver → Số liệu → Định giá → Rủi ro

Mọi bài vô địch đều đi theo một chuỗi khép kín. Đây là điểm quan trọng nhất cần hiểu:

```
 Investment Thesis (2–3 luận điểm)
        │  mỗi thesis chỉ ra 1–2 DRIVER tài chính cụ thể
        ▼
 Financial Analysis (lịch sử)  ──► chứng minh driver đang/đã vận động như thesis nói
        ▼
 Forecast (driver-based)       ──► driver được đưa thẳng vào mô hình
        ▼
 Valuation (DCF + kiểm chứng)  ──► giá trị phản ánh driver
        ▼
 Reverse DCF / Consensus gap   ──► thị trường đang định giá driver đó thế nào? (variant view)
        ▼
 Risk & Sensitivity            ──► nếu driver sai X% thì giá mục tiêu đổi Y%
```

**Ví dụ minh hoạ toàn chuỗi (Waterloo 2026, Lightspeed – SELL):**

| Thesis | Driver tài chính | Bằng chứng trong Financial Analysis | Đưa vào mô hình | Rủi ro / độ nhạy |
|---|---|---|---|---|
| #1 Động cơ tăng trưởng bị giới hạn cấu trúc | Tăng trưởng locations, sales efficiency | Guidance 10–15%/năm trong khi lịch sử FY21–25 chỉ ~4% CAGR. **SaaS magic number ~0.10** so với Toast 0.44 (ngưỡng hiệu quả > 0.75) | Doanh thu subscription = customers × ARPU theo vùng; tăng trưởng giảm dần | R1: chiến lược thành công. Tăng location growth +2% thì TP chỉ +$0.4 |
| #2 M&A che giấu tăng trưởng hữu cơ yếu | Organic vs inorganic growth; chất lượng tài sản M&A | Mua ở 12.5x EV/Revenue so với precedent 4–6x; **$1.3B impairment**; implied multiple còn 5.4x. Revenue CAGR 118% trước Ecwid, 24% sau | Không giả định M&A; tăng trưởng hữu cơ | Đối chiếu KPI thực tế với mục tiêu CMD 2022: ARPU $490 vs ~$650; GPV/GTV 37.1% vs ~50% |
| #3 Payments làm biên lợi nhuận đi xuống | Take rate, payment gross margin | Payment GM 27% so với Square 41%, Shopify 38%; take rate giảm từ 0.82% xuống 0.44% | Doanh thu transaction = GPV × conversion; GM transaction giảm dần | R3: payments có đòn bẩy hoạt động. Được giảm thiểu bằng phân tích cấu trúc chi phí bên thứ ba (Stripe) |

Kết quả là **ROE dự phóng chỉ 0.4% đến 1.7%** và ROIC ~5% (thấp hơn CoE 12.8%), dẫn tới SELL. Mọi con số đều khớp với nhau.

---

## 3. Giải phẫu phần Financial Analysis: 7 lớp phân tích

### Lớp 1: “Financial snapshot” ở trang 1

Trang đầu luôn có sidebar gồm:
- **Company statistics**: giá, vốn hoá, số cổ phiếu, 52w high/low, một multiple định giá (EV/NTM Revenue hoặc EV/NTM EBITDA).
- **Valuation results**: bảng từng phương pháp, trọng số, giá trị và TP.
- **Financial data**: 3–4 năm (Revenue, Growth, EBITDA, EBITDA margin).
- **Biểu đồ giá 5 năm có chú thích sự kiện.** Ví dụ LSPD đánh dấu thời điểm *short seller report*; DOM có “Stock Price Performance Annotated with Key Events”.

Mục đích là giám khảo đọc 30 giây đã nắm được câu chuyện tài chính.

### Lớp 2: Phân tích lịch sử có “làm sạch” (normalization & decomposition)

Bài thắng **không dùng số báo cáo thô**. Họ bóc tách để thấy bản chất:

| Kỹ thuật | Bài | Cách làm |
|---|---|---|
| **Tách organic và M&A** | LSPD 2026 (Appendix 13) | Ước doanh thu các công ty bị mua từ press release, giả định chúng tăng cùng tốc độ với LSPD rồi trừ ra. Kết quả: hơn 50% tăng trưởng 5 năm đến từ M&A |
| **Underlying và statutory** | QAN 2023 | Biên EBITDA statutory tăng 17.7% → 19.3% (FY16–19) nhưng *underlying* lại **giảm 270bps** do one-off gains (bán tài sản, hoàn nhập impairment) và giá nhiên liệu |
| **Loại bỏ giai đoạn bất thường** | CJT 2024, QAN 2023 | COVID được coi là “perfect storm”. Margin và ROIC giai đoạn COVID không được ngoại suy |
| **Phân rã ROIC = NOPAT margin × Invested capital turnover** | CJT 2024 (Appendix 8) | 10 năm lịch sử: NOPAT margin ổn nhưng IC turnover giảm 1.9x → 0.7x do capex tăng trưởng. Từ đó suy ra ROIC sẽ bật lên khi capex dừng |
| **Phân rã ROE ngân hàng** | CBA 2020 | ROE 18.4% → 12.7% (FY15–19) được giải thích bằng đòn bẩy giảm 17.0x → 14.3x (CET1 tăng theo APRA) cộng cash NPAT margin −300bps |
| **Nhóm doanh thu theo phân khúc khách hàng** | LSPD 2026 | Tỷ trọng GTV của merchant trên/dưới $500k theo quý. Mix shift lên khách lớn làm take rate giảm |

### Lớp 3: Bảng DuPont mở rộng, “form chuẩn” của bài vô địch

Waterloo 2024, Kozminski 2025 và Waterloo 2026 dùng **gần như y hệt một bảng**, đặt ở đầu phần Financial Analysis, gồm lịch sử và 5 năm dự phóng:

```
                         2021A 2022A 2023A 2024A 2025A | 2026P 2027P 2028P 2029P 2030P
DuPont Analysis
  Gross Margin
  EBITDA Margin
  Net Profit Margin
  Asset Turnover
  Return on Assets
  Financial Leverage (A/E)
  Return on Equity
  Return on Invested Capital
Liquidity
  Current Ratio
  Quick Ratio
Debt Ratios
  Interest Coverage Ratio
  Debt / EBITDA
```

Ateneo 2019 dùng **DuPont 5 bước** (Gross margin → Operating margin → **Interest burden** → **Tax burden** → Net margin → Asset turnover → Leverage → ROE), thêm **Operating Efficiency** (Inventory turnover, Operating cycle, **Cash Conversion Cycle**) và **Shareholder indicators** (EPS, EPS growth).

**Điểm mấu chốt về cách *viết* quanh bảng.** Bảng chỉ là bằng chứng. Phần chữ bên cạnh chia thành 4–6 đoạn, mỗi đoạn có tiêu đề là **một kết luận**, không phải một chủ đề:
- CJT 2024: *“Margins stabilize above pre-COVID levels”*, *“Increasing returns for investors”*, *“Improving credit profile”*.
- DOM 2025: *“FROM BLUEPRINTS TO BILLIONS”* (doanh thu), *“DEFYING COST SURGES WITH PREMIUM STRATEGY”* (biên), *“HIGHER EARNINGS, HIGHER PAYOUTS”* (cổ tức), *“FUELING GROWTH WITH SMART CAPITAL”* (NWC), *“LEVERAGING STABILITY”* (nợ).
- LSPD 2026: *“Short-term top-line growth with new initiative”*, *“Margins stabilize, except for transaction-related segment”*, *“Continued cash flow challenges”*.

### Lớp 4: ROIC vs WACC, trục kết luận tạo hay phá giá trị

| Bài | Cách dùng |
|---|---|
| CJT 2024 | Biểu đồ *Historical ROIC vs WACC*: trừ giai đoạn COVID, ROIC luôn dưới WACC. Thesis #3 là “inflection point”: capex/EBITDA giảm từ 187% (2022) thì ROIC dự phóng tăng lên 12.8% (2028E), vượt WACC 8.2%. Có cả **ROIC forecast theo Bear/Base/Bull** |
| QAN 2023 | Pre-COVID ROIC 13.7%–20.9% > WACC ~10% nên “consistent shareholder value creation”. Dự phóng **ROIC hội tụ về WACC và ROE hội tụ về CoE** ở cuối kỳ, đây là điều kiện để vào terminal |
| LSPD 2026 | ROIC ~5% (base) < CoE 12.8%, kèm ROIC theo 3 kịch bản Base/Bear/Bull, cả 3 đều dưới CoE (cao nhất ~9.3%). Họ còn phê phán buyback: *“returning cash… without value creation represents a misuse of funds”* |
| DOM 2025 | ROIC lịch sử ~20–30% được dùng để **hiệu chỉnh RONIC** (15%) trong công thức terminal growth (xem mục 5.3) |
| Vestas 2021 | ROIC 19% so với peer 5%, ROE 22% so với 4% (2019) để chứng minh lợi thế cạnh tranh |

### Lớp 5: KPI và unit economics đặc thù ngành (phần “ăn điểm” nhất)

Bài vô địch **luôn đào xuống KPI vận hành** thay vì dừng ở các tỷ lệ chung:

| Ngành | KPI được phân tích | Bài |
|---|---|---|
| Hàng không chở khách | ASK, RPK, **Load factor**, Yield, **RASK, CASK (ex-fuel)**, spread RASK–CASK (“unit profitability”), fuel cost/ASK, hedging, refining spread | QAN 2023 |
| Hàng không cargo | **Revenue per lb capacity**, fleet capacity (lbs), **direct cost per block hour** (ex-fuel, ex-D&A), % chi phí cố định (85%) cho thấy operating leverage | CJT 2024 |
| SaaS / Payments | **ARPU, GTV, GPV, GPV/GTV penetration, take rate**, payment gross margin, **SaaS magic number**, CAC ngầm định của bên mua lại ($11,178 so với ~$1,600) | LSPD 2026 |
| Bất động sản | **Units sold/delivered, land bank (units), stock-to-sales (số quý cần để bán hết hàng tồn)**, giá trung bình/căn, deferred revenue/doanh thu năm sau, inventory/doanh thu năm sau (1.33–1.34x) | DOM 2025 |
| Ngân hàng | **NIM bridge**, AIEA, replicating portfolio, BBSW/OIS spread, **Cost-to-income & Jaws**, loan loss rate, 90+ arrears, collective provisions/credit RWA, **CET1, LCR, Leverage ratio**, payout ratio | CBA 2020 |
| Tuabin gió | MW delivered, **giá bán/MW** (onshore €0.73m, offshore €1.45m → €1.14m), GW under service, LCOE, R&D/doanh thu | Vestas 2021 |
| Hoá chất / B2B | Tỷ trọng sản phẩm biên cao (HMSP), **capacity utilization**, maintenance vs growth capex, effective tax (ưu đãi PEZA/BOI) | DNL 2019 |

**Bài học:** đổi KPI chung (growth, margin) thành **KPI mà ban lãnh đạo và nhà đầu tư ngành đó thực sự theo dõi**, rồi đưa chính các KPI này vào mô hình dự phóng.

### Lớp 6: Chất lượng lợi nhuận, “red flags” kế toán và tín nhiệm

| Công cụ | Bài | Cách dùng |
|---|---|---|
| **Piotroski F-score** | MSI 2022 | MSI 7 so với peer trung bình 6, nên “high investment value” |
| **Beneish M-score** | MSI 2022 | −2.75 so với peer −2.61, nên “most valid earnings”, ít khả năng thao túng |
| **Altman Z-score** | MSI 2022 | 2.79, thấp hơn đối thủ, được thừa nhận thẳng là điểm yếu (“increased but still unlikely risk of bankruptcy”) |
| **Impairment & implied multiple** | LSPD 2026 | Lấy giá trị sau impairment chia doanh thu M&A ra implied 5.4x so với lúc mua 12.5x. Nếu định giá lại theo 1.05x hiện tại thì cần thêm ~$800M impairment |
| **Đổi định nghĩa KPI** | LSPD 2026 | Phát hiện ARPU bị định nghĩa lại và một số chỉ số ngừng công bố trước CMD 2025. Bảng “Targets vs Results” đối chiếu từng mục tiêu |
| **Credit metrics kiểu S&P** | QAN 2023 | FFO/Net debt, DSCR, ICR; rating Baa2/BB+; maturity profile trái phiếu; khung đòn bẩy mục tiêu của chính công ty (Net debt 2.0–2.5x adjusted EBIT, với “10% ROIC EBIT”) |
| **Bond YTM / debt schedule** | MSI 2022, DOM 2025 | Lịch đáo hạn nợ, BBB−, xác suất vỡ nợ 5 năm (Bloomberg) |

### Lớp 7: Phân bổ vốn (capital allocation) và dòng tiền

- **Capex/EBITDA so với peers** (CJT: 187% năm 2022, cao hơn Atlas và ATSG) để chứng minh giai đoạn đầu tư đã qua đỉnh.
- **Mô hình hoá chính sách chia cổ tức sát thực tế**:
  - DOM: cổ tức = **40% LN năm nay + 60% LN năm trước** (đúng thông lệ của công ty).
  - MSI: OCF chia theo ưu tiên của ban lãnh đạo: Capex 20%, M&A 37.5%, cổ tức 30%, buyback 12.5% (“Assumed Managerial Cash Flow Priorities”).
  - QAN: payout hội tụ về trung bình FY15–19 của Air NZ và Singapore Airlines (51.8%).
- **Buyback được đánh giá về giá trị, không chỉ mô tả**: CBA có “Buyback EPS Impact Bridge” cho thấy buyback không lấp được hố EPS ~5% do thoái vốn. LSPD: buyback là “undisciplined use of capital”.
- **Vốn lưu động phân tích theo bản chất ngành**: DOM có NWC chủ yếu là hàng tồn kho (căn hộ đang xây) trừ đi deferred revenue (50–60% doanh thu), tức khách hàng tài trợ vốn cho doanh nghiệp. Vestas có NWC âm (nhận tiền trước của khách, chiếm dụng nhà cung cấp). QAN có A$1.2b COVID credits trong RRIA.

---

## 4. Dự phóng (Forecast): luôn driver-based và có lý do cho từng lựa chọn

### 4.1 Cách xây doanh thu

| Bài | Công thức doanh thu |
|---|---|
| QAN 2023 | **Flying revenue = ASK × RASK**, RASK = Load factor × Yield. Loyalty = marketing (earn, ~43%) + redemption (burn, ~57%). Freight = AFTK × RAFTK (gắn CPI). ASK FY23–24 bám guidance theo % FY19 |
| DOM 2025 | **Revenue = deliveries × average transaction price**. Deliveries dựng từ pipeline từng dự án (Annex 32, dữ liệu từ 2012); giá/m² theo từng vùng (Warsaw, Tricity, Wroclaw, Cracow) |
| LSPD 2026 | **Subscription = customers × software ARPU** (theo vùng; customers tăng theo dân số + chiếm thị phần từ legacy). **Transaction = GPV × conversion rate lịch sử** (GPV tăng theo lạm phát). Hardware theo % tăng trưởng |
| Vestas 2021 | **Onshore/Offshore = MW delivered × giá/MW**, theo 4 vùng; Service = GW under service (19 năm hợp đồng) |
| MSI 2022 | **Hồi quy** doanh thu từng segment theo các driver kinh tế (chi tiêu an ninh công, IT spending, LTE nodes, body cams…), cộng hiệu ứng M&A có độ trễ 2 năm |
| DNL 2019 | Mỗi segment chia local và export; local theo dự báo ngành Philippines, export theo APAC (Euromonitor); thêm 5% tài khoản mới; điều chỉnh theo giá CNO/CPO và USDPHP |
| CBA 2020 | Tăng trưởng cho vay theo system credit growth; yield từng loại cho vay và tiền gửi theo spread so với BBSW, dẫn tới NIM |
| CJT 2024 | % tăng trưởng theo segment, **kèm giải thích vì sao** (công ty công bố ít nên dựng theo volume/rate sẽ không tin cậy): Domestic 6.6% CAGR (thấp hơn tăng trưởng TMĐT Canada 8%), ACMI 12% (gắn DHL), Charter về mức trước COVID |

> **Nguyên tắc:** nếu không dựng được driver vì thiếu dữ liệu, **phải nói rõ lý do** và neo % tăng trưởng vào một biến ngoại sinh có thể kiểm chứng (CJT neo vào tăng trưởng TMĐT Canada).

### 4.2 Cách xây chi phí và biên lợi nhuận
- **Tách chi phí cố định và biến đổi** (CJT: 85% direct cost cố định, tạo operating leverage; QAN: chi phí biến đổi tăng từ 30% lên 40%+ sau COVID).
- **Chi phí theo đơn vị**: QAN index phần biến đổi của từng OPEX qua CASK; DNL hồi quy biên segment commodity theo giá dầu dừa và dầu cọ chuẩn hoá.
- **Giả định bảo thủ có định lượng**: QAN giả định A$172m lợi ích tái cấu trúc bị lạm phát (2.5%/năm) bào mòn; DOM giả định gross margin giảm 32% → 27% (2030E).

### 4.3 Độ dài kỳ dự phóng: luôn có lý do

| Bài | Kỳ | Lý do nêu ra |
|---|---|---|
| CBA 2020 | **3 năm** | Doanh nghiệp trưởng thành; giảm sai số dự phóng dài hạn |
| CJT 2024 | 5 năm | Capex hoàn tất 2025, sau đó ổn định |
| QAN 2023, Vestas 2021, DOM 2025 | 6 năm | Cần đủ thời gian để thoát COVID và ramp-up capex đội bay; FCF hội tụ về g; **ROIC → WACC, ROE → CoE** |
| LSPD 2026 | **10 năm** | Công ty đang chuyển từ lỗ sang lãi nên cần đường đi dài tới steady-state margin |

---

## 5. Định giá: chi tiết kỹ thuật làm nên khác biệt

### 5.1 Chọn phương pháp theo bản chất doanh nghiệp

| Tình huống | Lựa chọn của bài vô địch |
|---|---|
| Ngân hàng (CBA) | **Equity-side**: RIM + DDM + P/E, P/BV. Lý do: “debt is raw material” nên EV/EBITDA vô nghĩa. Có **P/BV vs ROE regression** (theo thời gian và cross-section ngân hàng toàn cầu > $500bn tài sản) |
| Công ty mới có lãi, cấu trúc khác peers (LSPD) | **Levered DCF (FCFE) chiết khấu bằng CoE**, terminal theo exit P/E; **Comps 0%** vì payments stack khác biệt |
| Dự án BĐS (DOM) | DCF + **SOTP** theo dự án (giá trị pipeline đến 2027 trừ chi phí, cộng terminal, cộng giá trị land bank theo giao dịch đất tương đương) |
| Công ty chia cổ tức đều (DOM, MSI, CBA) | **DDM** để kiểm chứng (DOM: payout 80%, g 2% = ROE dài hạn × retention theo Damodaran) |
| Công ty có moat, khác biệt so với peers (CJT) | DCF 80%, Comps chỉ 20%. Không dùng FCF multiple vì FCF lịch sử âm |
| Thiếu peer nội địa (DNL, QAN) | DNL so với consumer names nội địa + hoá chất APAC; QAN chia peers thành **3 rổ địa lý** (Âu, Bắc Mỹ, APAC) |

### 5.2 Chi phí vốn: tam giác hoá rồi chọn phương án bảo thủ

| Thành phần | Kỹ thuật cụ thể |
|---|---|
| **Beta** | DOM: lấy **max của 3 cách** (hồi quy 5 năm với WIG, bottom-up theo peers, Damodaran sector) ra 0.62. CJT: re-lever beta peers theo cấu trúc vốn mục tiêu ra 1.17 (cao hơn beta 5 năm 1.04, “less aggressive”). LSPD: industry beta 1.72 thay vì beta quan sát 2.33. Vestas: re-levered, risk-adjusted 1.14 |
| **Cost of equity** | LSPD thử CAPM, Fama-French 3 và 5 nhân tố, build-up, implied CoE, rồi chọn CAPM 12.78%. CJT so CAPM 9.10% với CoE từ DDM 11.05% và ROE TB 5 năm 8.82% |
| **Risk-free** | Vestas: **bình quân trọng số theo doanh thu** của lợi suất 10 năm các nước chiếm > 1% doanh thu, ra 1.87%. DNL: forward yield có điều chỉnh kỳ vọng tăng lãi suất |
| **ERP** | MSI dùng ERP 8.3% (cao hơn Damodaran 4.77%) và nói thẳng đây là “cushion” chống rủi ro lãi suất |
| **Cost of debt** | CJT xét 3 cách (lãi suất PV của hybrid debentures 7%, lãi suất bình quân 5.5%, credit spread) và chọn 7% vì bảo thủ. QAN: bình quân YTM + spread theo rating + lãi P&L. DNL: synthetic rating |
| **WACC theo giai đoạn** | QAN: WACC kỳ dự phóng 9.5%, **WACC terminal 8.9%** (Kd 4.0%, Ke 10.0% theo trung bình lịch sử). CBA: CoE 8.83% kỳ dự phóng, 9.51% terminal |
| **Benchmark chéo** | CJT so WACC 8.2% với Damodaran ngành air transport 6.98%. MSI so với WACC của peers (TYL 7.56%, LHX 8.58%, AXON 11.54%) |

### 5.3 Terminal value: luôn kiểm tra chéo

| Bài | Cách làm |
|---|---|
| CJT 2024 | TG 2.25% cho implied exit 8.5x; exit 9.0x cho implied g 2.55%. Exit 9.0x là **chiết khấu so với trung bình 5 năm 11.0x** của chính CJT |
| LSPD 2026 | TG 3% cho implied P/E ~9x (≈ Fiserv). Exit 14x P/E cho implied g ~6.4%. **TV chiếm ~54% (TG) và ~65% (exit) giá trị vốn chủ** |
| Vestas 2021 | g 2.5%, TV €54bn, implied EV/EBITDA 12.4x |
| **DOM 2025** | **Key Value Driver formula: g = Reinvestment rate × RONIC** = 6.5% × 15% ≈ **0.97%**. RONIC 15% thấp hơn ROIC lịch sử ~20% (bảo thủ). Các thành phần NOPAT, D&A, Capex, ΔNWC terminal đều được hiện rõ |
| QAN 2023 | g 2.5% = trung vị giữa tăng trưởng GDP dài hạn của Úc và cận dưới 2% mục tiêu lạm phát RBA |
| DNL 2019 | g 3.5% tam giác hoá từ lạm phát dài hạn PH 3.5%, tăng trưởng tiêu dùng APAC 3.8% và tăng trưởng hoá chất đặc biệt ở thị trường trưởng thành 3.7% |
| MSI 2022 | g 2.5% = bình quân trọng số GDP của US, UK, Canada |

### 5.4 Từ giá trị nội tại đến **giá mục tiêu 12 tháng**

Một chi tiết kỹ thuật nhiều đội bỏ sót. Các bài Waterloo **roll-forward giá trị hiện tại thêm 1 năm theo chi phí vốn**:
- LSPD: implied $7.96 × (1 + 12.78%) ≈ **$8.97** (1-yr target, TG method).
- CJT: implied $146 × (1 + 8.2%) ≈ **$158**.

Họ còn tính **fully diluted shares theo treasury stock method** (ITM options, shares repurchased from proceeds, warrants). Với CJT, 4.02 triệu warrants của Amazon/DHL làm số cổ phiếu tăng từ 17.2 lên 21.2 triệu. Bước này ảnh hưởng mạnh đến giá/cổ phiếu.

DOM thì làm **EV → Equity bridge** có đủ NOA, cash, **management options định giá bằng Black-Scholes** và debt.

### 5.5 Relative valuation “có điều chỉnh”, không lấy trung bình ngành thô

- **QAN 2023**: tính **premium/discount lịch sử CY15–19** của QAN so với từng rổ peer, loại bỏ các giai đoạn méo (COVID, price war 2010–14, khủng hoảng nợ châu Âu, AA phá sản), áp vào median multiple của rổ rồi đặt trọng số 30/30/40. Lý do chọn EV/EBITDA forward được nêu 4 ý, trong đó có AASB-16 làm lease/khấu hao nằm dưới EBITDA.
- **CBA 2020**: áp **premium lịch sử** (P/E +13.7%, P/BV +38%) vì ROE của CBA cao hơn, cộng **hồi quy P/BV–ROE** (R² = 0.581).
- **DOM 2025**: 2 rổ (BĐS Ba Lan và Tây Âu) cộng hồi quy ROE/PBV.
- **CJT 2024**: tiêu chí chọn comps nằm ở Appendix 15, loại outliers (ATSG, Chorus).
- **Vestas 2021**: 4 nhóm peers (wind non-China, wind China, solar OEM, green tech), áp *small premium* có lý do (công nghệ dẫn đầu).

### 5.6 Reverse DCF: công cụ tạo “variant perception”

| Bài | Câu hỏi | Kết quả và cách dùng |
|---|---|---|
| QAN 2023 | Giá VWAP 1 tháng ngầm định load factor bao nhiêu? | Load factor FY24/25 giảm 6.2%, **thấp hơn 2.3–4.6% so với mức tối thiểu lịch sử**, nên thị trường đang quá bi quan → BUY |
| CJT 2024 | Giá hiện tại ngầm định tăng trưởng bao nhiêu? | Revenue CAGR **6.0%** và margin tăng nhẹ, thấp hơn tăng trưởng TMĐT, nên thị trường đánh giá thấp → BUY |
| LSPD 2026 | Cần giả định gì để ra giá hiện tại (với biên lợi nhuận ngang peers có lãi)? | Cần tăng trưởng doanh thu ~10%/năm liên tục 10 năm, “extremely hard to achieve” → SELL |

### 5.7 Đối chiếu với consensus

- QAN: *“Our FY24e EBIT margin is 42bps above consensus”*, với 3 lý do cụ thể.
- MSI: upside 6.5% được so với kỳ vọng lợi nhuận S&P 500 của giới phân tích (3.9%).
- DOM: football field có dải **Consensus** (189–262) cạnh DCF, Relative, SOTP, DDM.
- QAN: football field có dải **Broker** và **52-week**.

---

## 6. Kiểm định độ vững (Robustness): nhiều tầng

| Công cụ | Bài | Chi tiết |
|---|---|---|
| **Bảng độ nhạy 2 chiều** | Hầu hết | WACC × g; WACC × exit multiple (CJT, LSPD); **Revenue × Costs** (DOM: doanh thu −5% và chi phí +5% cho giá 126 so với 260) |
| **Độ nhạy 1 biến ±10%** | MSI 2022 | Mỗi line item ±10%: WACC +85bp cho −15%; COGS +10% cho −11.3%; SG&A +10% cho −2.22% |
| **Bull / Base / Bear** | Tất cả | Bảng giả định rõ (DOM: g 0.6/1.0/1.7%, GM 2030E 24/27/30%, EBITDA margin 15/18/21%, **giữ nguyên WACC** để cô lập yếu tố vận hành). CJT: Revenue CAGR 5.3/8.0/10.8%, implied return 3/33/100% |
| **Monte Carlo** | DOM (10k), Vestas (100k), MSI (**1 triệu**), QAN, CBA | Thay đổi đồng thời margin, WACC, growth, deliveries (DOM); WACC, g, COGS, giá bán, deliveries theo vùng (Vestas). Báo cáo **xác suất đạt upside**: Vestas có 65% khả năng upside ≥ 10%; MSI có 51% khả năng vượt 3.9% |
| **Xác suất cho bull/bear** | Vestas 2021 | Monte Carlo cho 10% xác suất ≥ bull, 6% ≤ bear |
| **Brownian motion price path** | MSI 2022 | 1 triệu đường giá 252 ngày theo lợi suất ngày từ 2012, cho 53% xác suất vượt kỳ vọng |
| **VaR** | MSI 2022 | Phân phối lợi suất và volatility |
| **Valuation waterfall** | LSPD 2026 (Appendix 17) | Cầu nối từ Bear → Base → Bull theo từng giả định (market share capture, costs align with peers, pricing, best-in-class cost structure) |
| **Độ nhạy KPI vận hành** | QAN 2023 | RPK ±10% cho giá $4.62 – $7.57; mỗi 10bp hiệu quả nhiên liệu cho +1.8% giá; capacity −5% cho −16.3% |

### Rủi ro luôn đi kèm “Valuation impact” và “Mitigation”

Format chuẩn của DOM 2025, MSI 2022 và QAN 2023:

> **[M1] Interest rate and inflation risk:** *mô tả…* **Valuation:** a 2% increase in WACC would lower our target price to PLN 207 (−20.3%). **Mitigation:** DOM’s focus on premium properties attracts higher-income buyers…

Kèm **Risk matrix** (Probability × Impact), phân loại rủi ro Market / Operational / Political / ESG. LSPD 2026 còn **sensitize trực tiếp rủi ro phản biện** (R1 và R2 cùng xảy ra chỉ đẩy TP từ $9.6 lên $10.5, nên khuyến nghị không đổi).

---

## 7. Gắn tài chính với ESG và Quản trị

- **Executive compensation vs TSR** (CJT, LSPD): đặt tổng thù lao lãnh đạo cạnh lợi nhuận cổ đông 5 năm (LSPD: thù lao lãnh đạo vẫn cao trong khi lợi nhuận cổ đông 5 năm âm sâu).
- **Incentive metrics**: DOM gắn thưởng với gross/net profit và ESG; CJT với ROIC tuyệt đối và relative TSR.
- **ESG trong định giá**: DOM tham khảo **ESG-adjusted beta 0.95** của Sustainalytics nhưng *quyết định không điều chỉnh*, có lý do (chưa có green bond hay SLL trong ngành tại Ba Lan; chuyên gia xác nhận ESG chưa ảnh hưởng chi phí vốn). Việc giải thích tại sao *không* điều chỉnh cũng được tính điểm.
- **Proprietary ESG scorecard** so với điểm của LSEG, MSCI, Bloomberg, Sustainalytics.

---

## 8. Kỹ thuật trình bày giúp số liệu “nói”

1. **Bố cục 2 cột**: thân bài bên trái (~2/3), cột phải là các Figure nhỏ kèm nguồn. **Mọi Figure đều được nhắc trong thân bài** (“(Figure 17)”).
2. **Tiêu đề đoạn là kết luận**, không phải chủ đề (“Lightspeed Capital is masking structural weakness in payments margins”).
3. **Trích dẫn chuyên gia đặt cạnh số liệu**: hộp quote “Expert A, Senior Technology Leader…”. DOM có 11 chuyên gia; LSPD và CJT có Appendix danh sách phỏng vấn.
4. **Primary research định lượng**: CJT khảo sát hành vi TMĐT (n=97); LSPD tổng hợp ~10 bảng xếp hạng PoS, 1.766 khiếu nại BBB và 645 review nhân viên.
5. **Cấu trúc Appendix chuyên cho tài chính** (Waterloo 2026): Valuation support (FCF projections, CoE methods, diluted shares, 2 bảng sensitivity), Reverse DCF, Valuation waterfall, Precedent transactions, Organic growth, Glossary KPI.
6. **Ngắn và đặc**: thân bài khoảng 10 trang, chi tiết mô hình nằm ở phụ lục.

---

## 9. Checklist áp dụng (theo thứ tự làm việc)

**A. Trước khi mở Excel**
- [ ] Viết 2–3 thesis. Mỗi thesis ghi rõ **1–2 driver tài chính** và **thị trường đang nghĩ gì khác**.
- [ ] Liệt kê KPI ngành mà ban lãnh đạo và analyst theo dõi, rồi lấy dữ liệu ít nhất 5–10 năm.
- [ ] Lên kế hoạch primary research (phỏng vấn chuyên gia, khảo sát, dữ liệu thay thế).

**B. Phân tích lịch sử**
- [ ] Chuẩn hoá: loại one-off, tách organic và M&A, xử lý giai đoạn bất thường.
- [ ] Bảng DuPont (3 hoặc 5 bước) + ROIC + Liquidity + Leverage, 5 năm lịch sử.
- [ ] ROIC = NOPAT margin × IC turnover; vẽ ROIC so với WACC.
- [ ] Unit economics theo segment; so sánh với 3–5 peers.
- [ ] Earnings quality: Piotroski, Beneish, Altman (nếu phù hợp); đối chiếu cam kết của ban lãnh đạo với kết quả thực tế.
- [ ] Capital allocation: capex/EBITDA, FCF, NWC, cổ tức, buyback, đòn bẩy mục tiêu.

**C. Dự phóng**
- [ ] Doanh thu = Volume × Price/Unit theo segment (hoặc giải thích vì sao không làm được và neo vào biến ngoại sinh).
- [ ] Chi phí tách cố định và biến đổi; margin có lý do định lượng.
- [ ] Kỳ dự phóng có lý do; cuối kỳ ROIC hội tụ về WACC, g FCF hội tụ về g terminal.
- [ ] Bảng DuPont dự phóng 5 năm, nhất quán với thesis.

**D. Định giá**
- [ ] Phương pháp chính phù hợp bản chất doanh nghiệp, trọng số có lý do.
- [ ] Beta, CoE, Kd: ít nhất 2–3 cách và chọn bảo thủ.
- [ ] Terminal: TG và exit multiple, có implied cross-check, % TV/EV, g có căn cứ (GDP + lạm phát, hoặc g = RR × RONIC).
- [ ] EV → Equity bridge đầy đủ; cổ phiếu pha loãng; roll-forward ra TP 12 tháng.
- [ ] Relative valuation có điều chỉnh (premium/discount lịch sử, hồi quy multiple–ROE, tiêu chí chọn peers).
- [ ] Reverse DCF và so sánh consensus để làm rõ variant view.
- [ ] Football field (gồm 52-week, consensus).

**E. Kiểm định & rủi ro**
- [ ] Sensitivity 2 chiều (WACC×g, WACC×multiple, Revenue×Cost).
- [ ] Bull/Base/Bear với bảng giả định.
- [ ] Monte Carlo, báo cáo xác suất đạt hoặc vượt ngưỡng khuyến nghị.
- [ ] Mỗi rủi ro: mô tả, **tác động định lượng lên TP**, mitigation, vị trí trên risk matrix.

---

## 10. Áp dụng vào mẫu DGW (Digiworld) bạn gửi

Từ 2 trang trong ảnh (phần “Financial Analysis” và “Valuation” của báo cáo DGW), báo cáo đã có nhiều điểm giống bài vô địch: doanh thu theo quý và theo ngành hàng, dự phóng theo segment (Mobile, Laptop, Office Equipment, Home Appliances, Consumer goods), GPM, OPM và NPAT-MI so với peers, ROE so với peers, cổ tức. Để lên mức CFARC champion, các nâng cấp nên ưu tiên là:

| # | Khoảng cách | Nâng cấp theo mẫu vô địch |
|---|---|---|
| 1 | Dự phóng chủ yếu dựa trên % tăng trưởng và CAGR theo segment | Dựng **Volume × ASP** cho từng segment (ví dụ Mobile: số máy bán ra × giá bình quân; neo vào thị phần Xiaomi hoặc Apple, chu kỳ thay máy 2–3 năm mà báo cáo đã nhắc). Nếu thiếu dữ liệu, nói rõ lý do như CJT và neo vào một biến ngoại sinh có thể kiểm chứng |
| 2 | Có ROE, biên lợi nhuận, peers nhưng chưa thấy **bảng DuPont + ROIC chuẩn** | Thêm bảng “form chuẩn” ở mục 3 (5 năm lịch sử, 5 năm dự phóng); với nhà phân phối nên thêm **CCC, inventory days, receivable days** như DNL 2019, vì vốn lưu động là driver số 1 của ROIC ngành phân phối |
| 3 | Chưa thấy **ROIC vs WACC** | Vẽ ROIC so với WACC FY18–28F. Với DGW, phân rã ROIC = NOPAT margin (mỏng) × IC turnover (cao) để cho thấy chiến lược “margin optimization” đẩy ROIC thế nào |
| 4 | Biên lợi nhuận theo segment mới ở mức mô tả | Làm **margin bridge** (mix effect và rate effect) giữa các năm; định lượng việc chuyển sang ngành hàng biên cao làm GPM tăng bao nhiêu bps (giống HMSP mix của DNL) |
| 5 | Chưa có reverse DCF và consensus | Reverse DCF: giá hiện tại ngầm định CAGR doanh thu hoặc NPAT-MI bao nhiêu, so với dự phóng của nhóm để làm rõ variant view |
| 6 | Kiểm định độ vững | WACC×g, WACC×P/E, Revenue×GPM; bull/bear theo chu kỳ thay máy; Monte Carlo cho GPM, tăng trưởng Mobile/Laptop, WACC |
| 7 | Rủi ro | Mỗi rủi ro (tập trung vào nhà cung cấp Xiaomi/Apple, tồn kho, tỷ giá, cạnh tranh) đều có **“Valuation impact: −x%”** và mitigation |
| 8 | Chi phí vốn | Beta: hồi quy với VN-Index, bottom-up peers và Damodaran rồi chọn bảo thủ; Rf = TPCP 10 năm; ERP Việt Nam có country risk premium; nêu WACC ngành để đối chiếu |
| 9 | Cổ tức | Mô hình hoá theo chính sách thực tế (VND/cp và tỷ lệ payout), kiểm tra bằng FCFE (dòng tiền có đủ để trả không) và DDM để kiểm chứng |
| 10 | Primary research | Phỏng vấn đại lý hoặc nhà bán lẻ (TGDĐ, FPT Shop), khảo sát chu kỳ thay máy và ý định mua laptop, dữ liệu giá bán theo kênh |

---

## 11. Phụ lục: Mẫu bảng nhanh để copy vào báo cáo

**(a) WACC build-up**

| Input | Giá trị | Nguồn/Phương pháp |
|---|---|---|
| Risk-free rate | | TPCP 10 năm (hoặc bình quân trọng số doanh thu) |
| Beta (levered) | | max/avg của: regression, bottom-up re-levered, Damodaran |
| ERP (+CRP) | | Damodaran / lịch sử thị trường |
| Cost of equity | | CAPM (đối chiếu FF3, build-up, implied) |
| Pre-tax Kd | | YTM trái phiếu / synthetic rating / lãi vay bình quân |
| Tax rate | | Thuế suất biên |
| D/(D+E) mục tiêu | | Cấu trúc vốn mục tiêu / peers |
| **WACC** | | So với Damodaran ngành và WACC của peers |

**(b) Terminal value cross-check**

| | Terminal growth method | Exit multiple method |
|---|---|---|
| Giả định | g = …% (GDP + lạm phát, hoặc RR × RONIC) | …x EV/EBITDA (so với TB lịch sử và peers) |
| Implied | Exit multiple = …x | g = …% |
| TV / EV | …% | …% |
| Giá trị hiện tại/cp | | |
| **TP 12 tháng** = giá trị × (1 + Ke hoặc WACC) | | |

**(c) Risk register**

| Mã | Rủi ro | Xác suất | Tác động | Valuation impact | Mitigation |
|---|---|---|---|---|---|
| M1 | | L/M/H | L/M/H | Δ biến X% → TP −Y% | |

---

## Nguồn

- CFA Institute – Research Challenge Past Champions: <https://www.cfainstitute.org/insights/events/research-challenge/past-champions>
- 2026 – University of Waterloo (Lightspeed): <https://www.cfainstitute.org/sites/default/files/docs/insights/events/research-challenge/rc-2026-winning-written-report-university-of-waterloo.pdf>
- 2025 – Kozminski University (Dom Development): <https://www.cfainstitute.org/sites/default/files/docs/insights/events/research-challenge/rc-2025-winning-written-report-kozminski-university.pdf>
- 2024 – University of Waterloo (Cargojet): <https://www.cfainstitute.org/sites/default/files/-/media/documents/support/research-challenge/challenge/rc-2024-winning-written-report-university-of-waterloo.pdf>
- 2023 – University of Sydney (Qantas): <https://www.cfainstitute.org/sites/default/files/-/media/documents/support/research-challenge/challenge/rc-2023-winning-written-report-university-of-sydney.pdf>
- 2022 – Northern Illinois University (Motorola Solutions): <https://www.cfainstitute.org/sites/default/files/-/media/documents/support/research-challenge/challenge/rc-2022-winning-written-report-northern-illinois-univ.pdf>
- 2021 – BI Norwegian Business School (Vestas): <https://www.cfainstitute.org/sites/default/files/-/media/documents/support/research-challenge/challenge/rc-2021-winning-report-bi-norwegian-business-school.pdf>
- 2020 – University of Sydney (Commonwealth Bank): <https://www.cfainstitute.org/sites/default/files/-/media/documents/support/research-challenge/challenge/rc-2020-winning-report-university-of-sydney.pdf>
- 2019 – Ateneo de Manila University (D&L Industries): <https://www.cfainstitute.org/sites/default/files/-/media/documents/support/research-challenge/challenge/rc-2019-winning-report-ateneo-de-manila-university.pdf>
