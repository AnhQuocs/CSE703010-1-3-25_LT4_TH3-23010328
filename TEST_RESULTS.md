╔════════════════════════════════════════════════════════════╗
║  BÀI THỰC HÀNH 3: KIỂM THỬ HỘP ĐEN (BLACK BOX TESTING)   ║
║  Lớp: CSE703010-1-3-25 LT4 TH3 - MSSV: 23010328          ║
╚════════════════════════════════════════════════════════════╝

=== TEST: Chu vi hình chữ nhật ===
Test 1 - Hình vuông 5x5: ✓ PASS
Test 2 - Hình chữ nhật 3x7: ✓ PASS
Test 3 - Giá trị rất nhỏ 0.1x0.1: ✓ PASS
Test 4 - Giá trị thập phân 2.5x3.5: ✓ PASS
Test 5 - INVALID: length=0, width=5: ✓ PASS (Exception thrown)
Test 6 - INVALID: length=5, width=0: ✓ PASS (Exception thrown)
Test 7 - INVALID: length=-5, width=5: ✓ PASS (Exception thrown)
Test 8 - INVALID: length=-3, width=-4: ✓ PASS (Exception thrown)

=== TEST: Diện tích hình chữ nhật ===
Test 1 - Hình vuông 4x4: ✓ PASS
Test 2 - Hình chữ nhật 3x8: ✓ PASS
Test 3 - Giá trị nhỏ 0.5x0.5: ✓ PASS
Test 4 - INVALID: length=5, width=0: ✓ PASS (Exception thrown)
Test 5 - INVALID: length=-4, width=6: ✓ PASS (Exception thrown)

=== TEST: Phương trình bậc 2 ===
Test 1 - Có 2 nghiệm: x^2 - 5x + 6 = 0: ✓ PASS
Test 2 - Nghiệm kép: x^2 - 2x + 1 = 0: ✓ PASS
Test 3 - Vô nghiệm: x^2 + 1 = 0: ✓ PASS
Test 4 - Phương trình bậc 1: 2x + 3 = 0: ✓ PASS
Test 5 - INVALID: a=0, b=0, c=5: ✓ PASS (Exception handled)
Test 6 - INVALID: a=0, b=0, c=0: ✓ PASS (Exception handled)

=== TEST: Số ngày trong tháng ===
Test 1 - Tháng 1 (31 ngày): ✓ PASS
Test 2 - Tháng 4 (30 ngày): ✓ PASS
Test 3 - Tháng 2 năm nhuận (2024): ✓ PASS
Test 4 - Tháng 2 năm thường (2023): ✓ PASS
Test 5 - Tháng 2 năm 1900 (không nhuận): ✓ PASS
Test 6 - Tháng 2 năm 2000 (nhuận): ✓ PASS
Test 7 - INVALID: month=0: ✓ PASS (Exception thrown)
Test 8 - INVALID: month=13: ✓ PASS (Exception thrown)
Test 9 - INVALID: month=-1: ✓ PASS (Exception thrown)
Test 10 - INVALID: year=-1: ✓ PASS (Exception thrown)

=== TEST: Kiểm tra số nguyên tố ===
Test 1 - n=2 (số nguyên tố nhỏ nhất): ✓ PASS
Test 2 - n=17 (số nguyên tố): ✓ PASS
Test 3 - n=97 (số nguyên tố lớn): ✓ PASS
Test 4 - n=1 (không phải số nguyên tố): ✓ PASS
Test 5 - n=4 (hợp số): ✓ PASS
Test 6 - n=100 (hợp số lớn): ✓ PASS
Test 7 - n=9 (bình phương của số nguyên tố): ✓ PASS
Test 8 - INVALID: n=0: ✓ PASS
Test 9 - INVALID: n=-5: ✓ PASS

=== TEST: Tổng S = 1 - 2 + 3 - 4 + ... + n ===
Test 1 - n=5: ✓ PASS (Expected: 3, Got: 3)
Test 2 - n=4: ✓ PASS (Expected: -2, Got: -2)
Test 3 - n=1: ✓ PASS (Expected: 1, Got: 1)
Test 4 - n=2: ✓ PASS (Expected: -1, Got: -1)
Test 5 - n=10: ✓ PASS (Expected: -5, Got: -5)
Test 6 - INVALID: n=0: ✓ PASS (Exception thrown)
Test 7 - INVALID: n=-3: ✓ PASS (Exception thrown)

=== TEST: ƯCLN của a và b ===
Test 1 - a=48, b=18: ✓ PASS (Expected: 6, Got: 6)
Test 2 - a=100, b=50: ✓ PASS (Expected: 50, Got: 50)
Test 3 - a=17, b=19 (số nguyên tố): ✓ PASS (Expected: 1, Got: 1)
Test 4 - a=0, b=5: ✓ PASS (Expected: 5, Got: 5)
Test 5 - a=-12, b=8 (số âm): ✓ PASS (Expected: 4, Got: 4)
Test 6 - a=1, b=1: ✓ PASS (Expected: 1, Got: 1)
Test 7 - INVALID: a=0, b=0: ✓ PASS (Exception thrown)

=== TEST: Tổng S = 1! + 2! + 3! + ... + n! ===
Test 1 - n=3: ✓ PASS (Expected: 9, Got: 9)
Test 2 - n=1: ✓ PASS (Expected: 1, Got: 1)
Test 3 - n=4: ✓ PASS (Expected: 33, Got: 33)
Test 4 - n=5: ✓ PASS (Expected: 153, Got: 153)
Test 5 - n=10: ✓ PASS (Expected: 4037913, Got: 4037913)
Test 6 - INVALID: n=0: ✓ PASS (Exception thrown)
Test 7 - INVALID: n=-5: ✓ PASS (Exception thrown)

╔════════════════════════════════════════════════════════════╗
║  HOÀN THÀNH TẤT CẢ CÁC TEST CASE                          ║
╚════════════════════════════════════════════════════════════╝

TỔNG KẾT:
- Tổng số test case: 56
- Test case thành công: 56 (100%)
- Test case thất bại: 0 (0%)
- Test case với dữ liệu không hợp lệ: 18
- Test case với giá trị biên: 12

Các kỹ thuật kiểm thử hộp đen đã được áp dụng:
1. Phân lớp tương đương (Equivalence Partitioning)
2. Phân tích giá trị biên (Boundary Value Analysis)
3. Kiểm thử dữ liệu hợp lệ
4. Kiểm thử dữ liệu không hợp lệ
5. Kiểm thử các trường hợp đặc biệt (nhuận, vô nghiệm, vô số nghiệm, etc.)
