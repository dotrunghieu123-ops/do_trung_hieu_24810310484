CAFE POS SYSTEM - HUONG DAN CHAY

A. NOI DUNG
- CafePOSSystem.sln / CafePOSSystem.csproj: mo bang Visual Studio.
- CafePOSDB.sql: tao database CafePOSDB va du lieu mau.
- App.config: chuoi ket noi SQL Server.
- Program.cs: diem bat dau chuong trinh.
- Db.cs: truy cap SQL theo mo hinh disconnected, co QueryDataSet (DataSet), Query (DataTable), SqlDataAdapter.
- FrmCafePOS.cs: giao dien POS, danh sach ban, them mon, chuyen ban, thanh toan.
- FrmMenu.cs: CRUD mon an va CRUD danh muc, kiem tra du lieu.

B. YEU CAU
- Windows 10/11
- Visual Studio 2019/2022
- .NET Framework 4.8 Developer Pack
- SQL Server Express/Developer va SSMS (hoac cong cu chay SQL)

C. CAC BUOC CAI DAT
1. Mo SQL Server Management Studio, ket noi vao instance SQL Server cua ban.
2. Mo file CafePOSDB.sql, bam Execute. CHU Y: script se xoa database CafePOSDB cu neu da ton tai.
3. Mo CafePOSSystem.sln bang Visual Studio.
4. Mo App.config, sua Data Source:
   - SQL Server mac dinh: Data Source=.;
   - SQL Express: Data Source=.\\SQLEXPRESS;
   - LocalDB: Data Source=(localdb)\\MSSQLLocalDB;
   Dung Integrated Security=True neu ban dang dang nhap Windows.
5. Build > Build Solution, sau do bam F5.
6. Chon ban, chon danh muc, chon mon, so luong, bam Them mon.
7. Bam Chuyen ban de chuyen hoa don sang ban trong.
8. Bam Thanh toan de chot hoa don va giai phong ban.
9. Bam Quan ly thuc don de them/sua/xoa mon va danh muc.

D. CAC CHUC NANG
- Hien thi ban va mau trang thai: trong / co khach.
- Chon ban va xem hoa don chua thanh toan.
- Them mon vao hoa don; neu mon da co thi cong don so luong.
- Thanh toan dung SqlTransaction: tinh tong tien, cap nhat hoa don, cap nhat trang thai ban.
- Chuyen ban dung transaction.
- Them/sua/xoa mon an; bat/tat trang thai dang ban.
- Them/sua/xoa danh muc.
- Kiem tra ten khong rong, gia khong am, khong cho xoa danh muc/mon dang duoc tham chieu boi du lieu khac.
- Su dung DataSet, DataTable va SqlDataAdapter cho mo hinh disconnected.

E. LUU Y
- Ma nguon duoc viet bang code, khong can keo tha Designer.
- Neu gap loi khong ket noi SQL, kiem tra ten instance va chuoi ket noi trong App.config.
- Neu project bao thieu .NET Framework 4.8, cai Developer Pack hoac doi Target Framework sang ban co tren may.
- Code duoc dong goi thanh bo project de mo va build trong Visual Studio; hay build tren may cua ban de xac nhan moi truong SQL/Visual Studio.
