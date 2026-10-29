BAI TAP 5.4 - HOTEL MANAGEMENT SYSTEM
======================================

THANH PHAN
- HotelManagement.sln: solution Visual Studio
- HotelManagement.csproj: ung dung C# Windows Forms .NET Framework 4.8
- DTO: cac lop chua du lieu
- DAL: truy cap SQL Server bang ADO.NET/SqlParameter
- BUS: xu ly nghiep vu
- GUI: giao dien Windows Forms tao bang code
- HotelDB.sql: tao CSDL, 5 bang va du lieu mau

HUONG DAN CHAY
1. Cai SQL Server va SQL Server Management Studio (SSMS).
2. Mo SSMS, mo file HotelDB.sql, bam Execute.
   Luu y: file SQL se tao lai cac bang va xoa du lieu cu trong cac bang nay.
3. Mo App.config va sua Data Source cho dung may:
   - SQL Express thuong la .\\SQLEXPRESS
   - SQL Server default instance co the la dau cham (.)
   - LocalDB thuong la (localdb)\\MSSQLLocalDB
4. Mo HotelManagement.sln bang Visual Studio tren Windows.
5. Chon .NET Framework 4.8 (can cai Developer Pack neu chua co).
6. Build Solution, sau do nhan F5.

CHUC NANG
- Xem danh sach phong va loc theo loai/trang thai bang DataView.RowFilter.
- Tra cuu khach theo CCCD bang SqlParameter; them khach moi khi check-in.
- Chon phong trong, tao phieu nhan phong va cap nhat trang thai trong transaction.
- Goi dich vu cho phieu dang luu tru.
- Tinh tien phong theo gio (lam tron len tung phut, toi thieu 1 phut) + tien dich vu.
- Check-out luu tong tien, ngay tra va cap nhat phong thanh Dang don dep trong SqlTransaction.

GHI CHU
- Don gia, du lieu mau co the sua trong SQL Server.
- De dua phong tu "Dang don dep" ve "Trong", hien tai can cap nhat TrangThai trong SSMS:
  UPDATE Phong SET TrangThai=N'Trống' WHERE SoPhong='P202';
  Co the bo sung nut "Hoan tat don phong" neu giao vien yeu cau.
- Day la bai mau hoc tap; hay mo project, chay thu va dieu chinh ten lop/giao dien theo yeu cau giao vien.
