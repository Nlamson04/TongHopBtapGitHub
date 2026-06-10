# BaiTapLon_PhatTrienUngDUngTrenThietBiDiDong
# Nguyễn Lam Sơn_K225480106076
## MÔN HỌC: PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419
# BÀI TẬP LỚN:
# 1. Viết phần mềm trên công cụ Mit App inventor <br>
   (tập trung vào quy trình tạo ra phần mềm) <br>
   app có 3 screen: <br>
   + about về bản thân+nút gọi sang 2 screen còn lại <br>
   + giải 1 bài toán đơn giản <br>
   + sử dụng webview: hiển thị 1 trang web có sẵn, hỗ trợ giao diện điện thoại <br>
   mô tả: thanh công cụ có gì? kéo thả + thay đổi thuộc tính: làm ntn, để làm gì? <br>
          block: mô tả bản chất việc kéo thả block ntn? <br>
                 ưu điểm gì so với viết code? nhược điểm? <br>
                 copy paste block ? (backpack) <br>
# 2. Viết app sử dụng Android Studio <br>
   + Android manifest.xml  => mô tả gì? app cần quyền để do-st: khai báo ntn? để làm gì? <br>
   + vòng đời của 1 ứng dụng android. <br>
     code tự sinh sau khi tạo 1 project: có sẵn hàm onCreate: tại sao??? <br>
   + Code: java language. <br>
     app cần check xem có quyền để do-st? : code ntn? ý nghĩa? <br>
     giao diện: (res/layout) mô tả bằng file XML + UI Design review <br>
        + thuộc tính text, hoặc các thuộc tính khác: giá trị hardcode => lưu vào nới khác, tham chiếu tới nó: <br>
          cú pháp của việc tham chiếu là gì? <br>
          ưu điểm của việc tham chiếu này? <br>
          OS hỗ trợ auto việc lấy giá trị tham chiếu theo LOCATION, LANGUAGE, THEME <br>
          việc hỗ trợ auto này giúp app làm được điều gì?	<br>
        + đối tượng chứa: gộp các đối tượng con lại: cùng 1 quy luật sắp xếp để hiển thị <br>
          các đối tượng con nằm kề nhau theo chiều dọc | hoặc ngang, gravity <br>
     code tương tác với layout: vd hiển thị text <br>
          mong muốn text hiển thị phù hợp với thiết lập LOCATION, LANGUAGE, THEME của người dùng <br>
          thì làm ntn? (tránh hardcode) <br>
     event (sự kiện) người dùng tác động vào app: CLICK vào button, click vào text,... <br>
          với 1 sự kiện nào đó, muốn chạy 1 đoạn code để do-st <br>
          thì LAYTOUT cần làm gì? <br>
              CODE viết như nào (2 cách) <br>
---------------------------
     trong app có các thư mục đặc biệt: Assets
     khi sử dụng Window Explorer để copy các files + folder vào trong Assets
     thì khi compiler: mọi file này đều đi theo app, nằm trong app
     trong app có thể truy cập được đến các file này
     cú pháp truy cập vào là gì?
     lợi ích của việc app có sẵn các files (offline cũng có)?
     ứng dụng: app hướng dẫn việc X

==> tạo app1 sử dụng cơ chế Dữ liệu chuẩn bị trước trong Assets <br>
       -  format dữ liệu: tuỳ ý, nội dung tuỳ ý <br>
       -  công cụ để hiển thị dữ liệu: tuỳ ý <br>
       - có cần phải tiền xử lý trước khi hiển thị ko: tuỳ ý. <br>
       - SV TỰ ĐẶT RA VẤN ĐỀ => TỰ GIẢI QUYẾT VẤN ĐỀ <br>
       - MÔ TẢ ĐƯỢC DỮ LIỆU CÓ ĐẶC THÙ GÌ <br>
                   1. DÙNG THUẬT TOÁN NÀO ĐỂ XỬ LÝ DỮ LIỆU (NẾU CẦN) <br>
                   2. DÙNG ĐỐI TƯỢNG NÀO ĐỂ HIỂN THỊ DỮ LIỆU. <br>
                   3. (ĐỘ SÁNG TẠO LÀ KO GIỚI HẠN) <br>
------------------------
APP2 (android studio):  tạo app tương đương với Mit App inventor <br>
  app có 3 activity <br>
  + activity1: about: about+nút gọi sang 2 activity còn lại <br>
  + activity2: giải toán đơn giản (tuỳ ý). mỗi khi giải xong bài toán: gọi api tại https://k58kmt.tdh.io.vn/api <br>
    để gửi bài toán lên đó <br>
    {app_by:mã số sv, input: {a:1,b:2,c:3,name:"hello tắc kè"},output:{ketluan:"vô nghiệm", abc:"xyz", nghiem:3.14}} <br>
    nhận lại json: {ok:1, stt:1234} <br>
  + activity3: <br>
    dùng web-view để truy cập từ <br>
    1 trang web https://k58kmt.tdh.io.vn?masv=mã sv của bạn <br>
======================= <br>
    vết để lại: mô tả quá trình làm bài tập ra file .md => upload github <br>
    kèm hình ảnh minh hoạ quá trình làm. <br>

    print ra giấy đóng quyển, nộp bm. <br>
# BÀI LÀM:
# PHẦN 1
## 1. LÀM APP TRÊN MIT APP INVENTOR
# Địa chỉ công cụ: http://ai2.appinventor.mit.edu/ (Đăng nhập bằng tài khoản Google).
## Cách thực hiện: <br>
Tạo App: Click Projects -> Start new project -> Đặt tên: BaiTapLon_App1. <br> 
Tạo 3 Màn hình (Screen): Góc trên bên phải có nút Add Screen. Bạn tạo thêm Screen2 và Screen3. <br>
Thiết kế Giao diện (Tab Designer): <br>
Screen1 (About): Cột Palette (bên trái), kéo Image, Label (ghi thông tin của bạn) và 2 Button vào màn hình giữa (Viewer). Sang cột Properties (bên phải) đổi tên Button thành "Chuyển Screen 2" và "Chuyển Screen 3". <br>
Screen2 (Toán): Kéo 2 TextBox (để nhập a, b), 1 Button (Giải), 1 Label (Hiển thị kết quả). <br>
Screen3 (Web): Góc trái tìm mục User Interface, kéo linh kiện WebViewer vào. Nhìn sang phải cột Properties, ô HomeUrl dán link: https://m.dantri.com.vn. <br>
Viết logic (Tab Blocks ở góc phải trên cùng): <br>
Ở Screen1: Click vào Button1 bên menu trái, kéo khối when Button1.Click do. Vào mục Control, kéo khối open another screen screenName và ghép vào. Gõ "Screen2". Làm tương tự cho Button 2 chuyển sang "Screen3". <br>
Ở Screen2: Dùng khối toán học (Math) để lập trình cộng/trừ 2 TextBox hiển thị ra Label. <br>
# Thực Hành:
1 Tạo Projects đătj tên là baitaplon
# <img width="1917" height="926" alt="image" src="https://github.com/user-attachments/assets/ceb8198d-43e4-4321-9dd8-de42f0a1d596" />
2 Add Screen.tạo thêm Screen2 và Screen3.
# <img width="632" height="237" alt="image" src="https://github.com/user-attachments/assets/f614b9a4-f86e-42a5-ad6f-b8485bf6dbb3" />
3 Thiết kế Giao diện
## screen1: 
# <img width="1918" height="1025" alt="image" src="https://github.com/user-attachments/assets/2e2021d1-4d63-4b09-a96c-77036b8a53c1" />
## screen2:
# <img width="1918" height="1027" alt="image" src="https://github.com/user-attachments/assets/41f1b3e9-717d-42a9-84f9-91b70b706937" />
## csreen3:
# <img width="1918" height="1023" alt="image" src="https://github.com/user-attachments/assets/c0f41239-df50-42e0-a66d-e7ff998880c3" />
# 2. VIẾT LOGIC (TAB BLOCKS - GÓC TRÊN CÙNG BÊN PHẢI)
Bấm vào nút Blocks ở góc trên cùng bên phải để chuyển từ giao diện thiết kế sang giao diện ghép khối lệnh. <br>
## 1. Viết logic cho Screen1 (Chuyển màn hình) <br>
Viết logic cho Screen1 (Chuyển màn hình) <br>
(Đảm bảo bạn đang chọn Screen1 ở góc trái) <br>
## Bước 1: Ở menu bên trái, bấm vào chữ Btn_Toan. 
Nó sẽ hiện ra một loạt khối lệnh màu vàng. Bạn lấy con chuột kéo khối when Btn_Toan.Click do thả ra màn hình trống ở giữa. <br>
## Bước 2: Ở menu bên trái, bấm vào danh mục Control (màu vàng đậm hệ thống). 
Kéo khối open another screen screenName gắn vào bên trong cái miệng chữ do của khối <br>
## Bước 3: Ở menu bên trái, bấm vào danh mục Text (màu hồng). 
Kéo khối chuỗi rỗng có dấu ngoặc kép "" gắn vào vị trí screenName. <br>
Sau đó click chuột vào trong dấu <br>
ngoặc kép đó và gõ đúng chữ: Screen2 (chú ý viết hoa chữ S, viết liền không dấu). <br>
## Làm tương tự cho nút Web: Kéo khối when Btn_Web.Click do -> gắn khối open another screen screenName -> gắn khối "" và gõ vào chữ Screen3. <br>
# <img width="840" height="468" alt="image" src="https://github.com/user-attachments/assets/572094b0-a543-40e8-a3f8-e8f876b8785c" />
## 2. Viết logic cho Screen2 (Lập trình phép toán cộng a + b)
Viết logic cho Screen2 
(Lập trình phép toán cộng $a + b$)
(Bấm chọn chuyển sang màn hình Screen2 ở menu góc trên bên trái, sau đó chọn Tab Blocks)
## Bước 1:Ở menu bên trái, bấm vào chữ Btn_TinhTong. 
Kéo khối when Btn_TinhTong.Click do thả ra màn hình trống.
## Bước 2: Ở menu bên trái, bấm vào chữ Lbl_KetQua.
Kéo khối set Lbl_KetQua.Text to gắn vào bên trong miệng chữ do.
## Bước 3: Ở menu bên trái, bấm vào danh mục Math (màu xanh dương).
Tìm và kéo khối phép cộng có dấu cộng + (... + ...) gắn vào sau chữ to của khối bước 2.
## Bước 4: Ở menu bên trái, bấm vào chữ Txt_SoA.
Tìm khối lệnh tên là Txt_SoA.Text (màu xanh lá cây nhạt) kéo ra gắn vào ô trống thứ nhất của phép cộng +.
## Bước 5: Ở menu bên trái, bấm vào chữ Txt_SoB. 
Tìm khối lệnh tên là Txt_SoB.Text kéo ra gắn vào ô trống thứ hai còn lại của phép cộng +.
# <img width="1918" height="947" alt="image" src="https://github.com/user-attachments/assets/2c39d7f8-141f-4ef8-a6b0-f3f5cd555241" />
# NỘI DUNG LÝ THUYẾT VỀ LOGIC:
## Quy trình thiết kế giao diện ứng dụng (Tab Designer)
Ứng dụng được thiết kế gồm 3 màn hình (Screen) cụ thể như sau:

* **Screen1 (About Bản Thân):** - Sử dụng đối tượng `Image1` hiển thị ảnh đại diện cá nhân (`anh_the_nguyen_lam_son.jpg`).
  - Sử dụng các `Label1`, `Label2`, `Label3` để hiển thị thông tin tĩnh bao gồm: "Họ và tên: Nguyễn Lam Sơn", "MSSV: 20261234", "Lớp: K58KMT".
  - Sử dụng 2 nút bấm `Btn_Toan` và `Btn_Web` định dạng chữ hiển thị để người dùng click chuyển trang.
  # <img width="1918" height="1025" alt="image" src="https://github.com/user-attachments/assets/2e2021d1-4d63-4b09-a96c-77036b8a53c1" />

* **Screen2 (Bài toán đơn giản):**
  - Thiết kế bài toán tính tổng hai số nhập vào từ bàn phím.
  - Sử dụng `Txt_SoA` và `Txt_SoB` cấu hình thuộc tính `NumbersOnly = True` để bắt buộc nhập số.
  - Sử dụng `Btn_TinhTong` để kích hoạt sự kiện xử lý.
  - Sử dụng `Lbl_KetQua` đổi màu chữ sang màu Đỏ để hiển thị kết quả đầu ra.
# <img width="1918" height="1027" alt="image" src="https://github.com/user-attachments/assets/41f1b3e9-717d-42a9-84f9-91b70b706937" />

* **Screen3 (WebView hiển thị trang báo):**
  - Kéo linh kiện `WebViewer1` chiếm toàn màn hình.
  - Thay đổi thuộc tính `HomeUrl` trỏ thẳng tới địa chỉ: `https://m.dantri.com.vn` để tự động tải giao diện báo điện tử hỗ trợ mobile.
# <img width="1918" height="1023" alt="image" src="https://github.com/user-attachments/assets/c0f41239-df50-42e0-a66d-e7ff998880c3" />

## 2. Mô tả các thành phần hệ thống và Bản chất lập trình Block
* **Thanh công cụ quản lý:**
  - *Palette:* Nơi chứa toàn bộ kho linh kiện gốc của hệ thống Android.
  - *Viewer:* Màn hình giả lập hiển thị giúp sắp xếp bố cục linh kiện bằng mắt thường.
  - *Components:* Cây quản lý phân cấp, giúp quản lý và đổi tên định danh ID đối tượng (ví dụ: đổi từ Button1 thành Btn_Toan).
  - *Properties:* Bản tùy chỉnh chi tiết thông số linh kiện (màu sắc, kích cỡ chữ, kích thước dài rộng).

* **Bản chất của việc kéo thả Block:**
  - Bản chất là lập trình trực quan hướng sự kiện. Thay vì phải gõ từng dòng mã lệnh, người lập trình ghép nối các khối logic toán học, văn bản và điều khiển có sẵn lại với nhau. Hệ thống thiết kế các rãnh khớp nối thông minh, nếu ghép sai kiểu dữ liệu (ví dụ ghép chữ vào phép toán cộng), khối lệnh sẽ không khít nhau, từ đó triệt tiêu hoàn toàn lỗi cú pháp (Syntax Error) như thiếu dấu `;` hay dấu `{}` trong code truyền thống.
  - *Ưu điểm:* Dễ tiếp cận, trực quan, tốc độ xây dựng luồng ứng dụng cực nhanh.
  - *Nhược điểm:* Khi logic phình to, giao diện kéo thả blocks cực kỳ rối mắt, khó quản lý mã nguồn và hạn chế can thiệp sâu vào các tính năng phần cứng nâng cao của hệ điều hành.

* **Tính năng Backpack (Cái Balo):**
  - Nằm ở góc trên bên phải màn hình Blocks. Đây là bộ nhớ đệm dùng để lưu trữ tạm thời các khối logic phức tạp. Khi muốn nhân bản đoạn code chuyển màn hình từ Screen1 sang áp dụng cho các màn hình khác, ta chỉ cần kéo cụm block đó thả vào Backpack, sau đó sang màn hình mới mở Backpack ra kéo thả ngược lại. Đây chính là cơ chế Copy - Paste mã nguồn trực quan.
# <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/61306bcc-bd17-4508-bce9-3de06c6ef09b" />
# PHẦN 2: ANDROID STUDIO - KIẾN THỨC NỀN TẢNG (LÝ THUYẾT & CHUẨN BỊ)
Mở Android Studio -> Chọn New Project -> Empty Views Activity
## 2.1 AndroidManifest.xml là gì?
- Nó là "giấy khai sinh" và là bảng cấu hình của ứng dụng. Mọi Activity bạn tạo ra, mọi quyền truy cập hệ thống đều phải khai báo ở đây.
- xin quyền dùng Internet (phục vụ cho tính năng WebView), gõ dòng lệnh này vào # <uses-permission android:name="android.permission.INTERNET" />
# <img width="1107" height="1000" alt="image" src="https://github.com/user-attachments/assets/488e213b-0bad-427f-8158-a2407cfd78b1" />
## 2.2 Vòng đời ứng dụng & File Code Java
- Ứng dụng Android viết bằng ngôn ngữ Java. Nó có một vòng đời trải qua nhiều trạng thái (mở app, ẩn xuống nền, tắt app). Hàm onCreate luôn có sẵn khi tạo project vì đây là bước đầu tiên trong vòng đời ứng dụng khi màn hình được tạo ra; nó chịu trách nhiệm khởi tạo các biến và liên kết giao diện người dùng. <br>
- Mở thư mục: MainActivity.java
- mọi code tương tác cơ bản ở giai đoạn đầu sẽ viết bên trong hàm này: onCreate
# <img width="1108" height="1078" alt="image" src="https://github.com/user-attachments/assets/be2fbbcf-27bc-49bd-965c-c123dfc26fe6" />
## 2.3. Thiết kế giao diện (Layout) & Tránh Hardcode
- Giao diện được mô tả bằng file XML nằm trong thư mục res/layout. Để tránh hardcode (viết thẳng giá trị chết vào giao diện), bạn phải lưu các thuộc tính text vào một nơi khác rồi tham chiếu tới nó <br>
** Ưu điểm của việc này là hệ điều hành (OS) sẽ tự động lấy giá trị tham chiếu theo Location (Vị trí), Language (Ngôn ngữ), Theme (Chủ đề) của người dùng. Việc hỗ trợ auto này giúp app tự động chuyển đổi ngôn ngữ hoặc giao diện sáng/tối mà lập trình viên không cần viết thêm code <br>
- Mở file res/values/strings.xml: Thêm một dòng: <string name="loi_chao">Xin chào bạn</string> <br>
# <img width="1265" height="458" alt="image" src="https://github.com/user-attachments/assets/200409e2-65d3-49d3-a257-8961d11cbefe" />
- Tiếp theo, mở file giao diện res/layout/activity_main.xml: Khi tạo một chữ hiển thị, thay vì viết android:text="Xin chào bạn" (đây là hardcode),viết cú pháp tham chiếu: android:text="@string/loi_chao" <br>
# <img width="1091" height="776" alt="image" src="https://github.com/user-attachments/assets/fdd0b032-6d7c-437a-87d4-d04cf5bbaf5d" />
## Bước 2.4: Event (sự kiện người dùng)
- Khi click vào Button, ta viết code xử lý. Có 2 cách:
- Gắn trực tiếp trong Java bằng setOnClickListener.
- Khai báo trong XML android:onClick="tenHam" rồi viết hàm trong Java
# <img width="1040" height="382" alt="image" src="https://github.com/user-attachments/assets/760624a6-9041-4ae5-987d-e936b8446d48" />
## 2.5. AssetsTạo folder: 
- Chuột phải vào app/src/main → New → Directory → đặt tên assets.
- Thêm file: Copy file data.json hoặc data.txt vào folder assets.
** Mở file Java: Trong MainActivity.java, thêm:
- Mục tiêu: Thêm dữ liệu offline.
# <img width="1077" height="978" alt="image" src="https://github.com/user-attachments/assets/129348c9-792c-4293-9f48-e178a1482d0d" />
# <img width="1117" height="231" alt="image" src="https://github.com/user-attachments/assets/327daeaa-7fb9-451f-8580-14c9df4c1224" />
# PHẦN 3: TẠO THÊM 2 ACTIVITY MỚI ( ACTIVITY 2, ACTIVITY3 )
** B1
- Mặc định khi tạo dự án, đã có sẵn màn hình thứ nhất là MainActivity. Bây giờ ta cần tạo thêm Activity 2 và Activity 3
-Cách làm: Chuột phải vào thư mục chứa code Java của bạn (ví dụ: com.example.baitaplon)
--> Chọn New --> Activity --> Empty Views Activity.
- Tạo cái thứ nhất đặt tên là: GiaiToanActivityLàm tương tự tạo cái thứ hai đặt tên là: WebViewActivity
## KẾT QUẢ
- thống tự sinh: Android Studio sẽ tự động tạo ra 2 file Java trong thư mục code và 2 file giao diện XML tương ứng (activity_giai_toan.xml và activity_web_view.xml) trong thư mục res/layout
# <img width="563" height="932" alt="image" src="https://github.com/user-attachments/assets/9ed5a906-9734-4a89-895a-61a4e65d6929" />
** B2
CẤU HÌNH HỆ THỐNG VÀ XIN QUYỀN TRUY CẬP INTERNET
-Hướng dẫn thực hiện:
** Mở thư mục app --> manifests --> Click đúp mở file AndroidManifest.xml.
- Tiến hành chèn thêm các dòng xin quyền Internet (INTERNET, ACCESS_NETWORK_STATE) và thuộc tính cho phép chạy mạng không mã hóa (usesCleartextTraffic="true").

## Mã nguồn hoàn chỉnh AndroidManifest.xml:

<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    package="com.example.baitaplon">
    
    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />

    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.BaitapLon"
        android:usesCleartextTraffic="true"> <activity
            android:name=".WebViewActivity"
            android:exported="false" />
        <activity
            android:name=".GiaiToanActivity"
            android:exported="false" />
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>
</manifest>

** B3: 
QUAN TRỌNG - THAY ĐỔI THÔNG TIN BẢN THÂN TRONG TÀI NGUYÊN CHUỖI
Hướng dẫn thực hiện:
- Vào thư mục app --> res --> values --> Mở file strings.xml.
- Xóa sạch code cũ, dán đè đoạn code dưới đây để cập nhật tên Nguyễn Lam Sơn và MSSV K225480106076 tập trung tại đây nhằm tránh lỗi hardcode text.

## Mã nguồn hoàn chỉnh strings.xml:

<resources>
    <string name="app_name">BaitapLon</string>
    <string name="title_btl">BÀI TẬP LỚN MÔN TEE0419</string>
    <string name="info_sv">Họ và tên: Nguyễn Lam Sơn\nMSSV: K225480106076</string>
    <string name="btn_giai_toan">Mở Màn Hình Giải Toán</string>
    <string name="btn_webview">Mở Màn Hình Web View</string>
    <string name="title_assets">DỮ LIỆU ĐỌC TỪ ASSETS (APP1):</string>
    <string name="loading_assets">Đang tải dữ liệu từ tệp tin...</string>
    <string name="title_pt">Giải phương trình ax + b = 0</string>
    <string name="hint_a">Nhập hệ số a</string>
    <string name="hint_b">Nhập hệ số b</string>
    <string name="hint_name">Nhập tên của bạn</string>
    <string name="btn_tinh">Tính toán &amp; Gửi API</string>
    <string name="text_kq">Kết quả hiển thị tại đây</string>
</resources>

** B4:
- LẬP TRÌNH ĐIỀU HƯỚNG VÀ ĐỌC TỆP ASSETS TẠI MÀN HÌNH CHÍNH
- Hướng dẫn thực hiện: Mở file MainActivity.java và viết code bắt sự kiện click cho 2 nút bấm để chuyển màn hình (Intent) sang Activity giải toán và WebView, đồng thời đọc file data.txt từ thư mục Assets.

## Mã nguồn hoàn chỉnh MainActivity.java:

package com.example.baitaplon;

import android.content.Intent;
import android.os.Bundle;
import android.widget.Button;
import android.widget.TextView;
import androidx.appcompat.app.AppCompatActivity;
import java.io.BufferedReader;
import java.io.InputStream;
import java.io.InputStreamReader;

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Button btnGiaiToan = findViewById(R.id.btn_den_giai_toan);
        Button btnWebView = findViewById(R.id.btn_den_webview);
        TextView tvAssets = findViewById(R.id.tv_hien_thi_assets);

        // Chuyển sang Activity Giải Toán
        btnGiaiToan.setOnClickListener(v -> {
            Intent intent = new Intent(MainActivity.this, GiaiToanActivity.class);
            startActivity(intent);
        });

        // Chuyển sang Activity WebView
        btnWebView.setOnClickListener(v -> {
            Intent intent = new Intent(MainActivity.this, WebViewActivity.class);
            startActivity(intent);
        });

        // Đọc tệp tin data.txt từ Assets (Offline)
        StringBuilder chuoiKhaiThac = new StringBuilder();
        try {
            InputStream is = getAssets().open("data.txt");
            BufferedReader reader = new BufferedReader(new InputStreamReader(is));
            String dongDuLieu;
            while ((dongDuLieu = reader.readLine()) != null) {
                chuoiKhaiThac.append(dongDuLieu).append("\n");
            }
            reader.close();
            tvAssets.setText(chuoiKhaiThac.toString());
        } catch (Exception e) {
            e.printStackTrace();
            tvAssets.setText("Lỗi: Không tìm thấy tệp data.txt trong thư mục Assets!");
        }
    }
}

## Trong bài này em Khởi tạo và Cấu hình Môi trường Thiết bị Thật Để chạy ứng dụng mượt mà không tốn RAM máy tính, tiến hành cấu hình điện thoại thật qua các bước:
Mở Cài đặt điện thoại --> Thông tin phần mềm --> Ấn 7 lần vào Số hiệu bản dựng để mở Chế độ nhà phát triển.
- Vào Tùy chọn nhà phát triển --> Bật công tắc Gỡ lỗi USB (USB Debugging).
- Cắm cáp kết nối máy tính và chọn "Luôn cho phép từ máy tính này".
# <img width="375" height="232" alt="image" src="https://github.com/user-attachments/assets/34ae61e0-5528-48b8-9ae9-c78eede04582" />

-------------------------
Bấm nút Run chạy ứng dụng. Khi màn hình chính vừa hiện lên trên điện thoại thật Màn hình hiển thị đúng Họ tên, MSSV của bạn và load thành công dữ liệu từ file văn bản trong Assets
-------------------------

# <img width="2000" height="1200" alt="image" src="https://github.com/user-attachments/assets/a12ae0c6-f0a9-4c49-aac7-32ce9a64115a" />
** B5: 
LẬP TRÌNH THUẬT TOÁN GIẢI TOÁN VÀ ĐÓNG GÓI JSON GỬI API MẠNG
- Hướng dẫn thực hiện: Mở file GiaiToanActivity.java.
- Code này chịu trách nhiệm lấy giá trị a, b, giải phương trình bậc nhất, đóng gói MSSV K225480106076 cùng kết quả vào chuỗi cấu trúc JSON, sử dụng thư viện OkHttpClient để POST lên server của thầy.

## Mã nguồn hoàn chỉnh GiaiToanActivity.java:

package com.example.baitaplon;

import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;
import org.json.JSONObject;
import java.io.IOException;
import okhttp3.Call;
import okhttp3.Callback;
import okhttp3.MediaType;
import okhttp3.OkHttpClient;
import okhttp3.Request;
import okhttp3.RequestBody;
import okhttp3.Response;

public class GiaiToanActivity extends AppCompatActivity {
    private EditText edtA, edtB, edtTen;
    private TextView tvKetQua;
    private final OkHttpClient client = new OkHttpClient();

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_giai_toan);

        edtA = findViewById(R.id.edt_nhap_a);
        edtB = findViewById(R.id.edt_nhap_b);
        edtTen = findViewById(R.id.edt_nhap_ten);
        tvKetQua = findViewById(R.id.tv_ket_qua);
        Button btnTinh = findViewById(R.id.btn_tinh_toan);

        btnTinh.setOnClickListener(v -> thuatToanVaApi());
    }

    private void thuatToanVaApi() {
        try {
            double a = Double.parseDouble(edtA.getText().toString());
            double b = Double.parseDouble(edtB.getText().toString());
            String name = edtTen.getText().toString();
            String mssv = "K225480106076"; // Gắn MSSV của bạn

            // Thuật toán giải toán
            String ketLuan;
            String nghiemStr;
            if (a == 0) {
                if (b == 0) {
                    ketLuan = "Vô số nghiệm";
                    nghiemStr = "Mọi x";
                } else {
                    ketLuan = "Vô nghiệm";
                    nghiemStr = "Không có";
                }
            } else {
                double x = -b / a;
                ketLuan = "Có nghiệm";
                nghiemStr = String.valueOf(x);
            }

            tvKetQua.setText(ketLuan + " | x = " + nghiemStr);

            // Đóng gói cấu trúc JSON gửi API theo tài liệu
            JSONObject jsonPayload = new JSONObject();
            jsonPayload.put("app_by", mssv);

            JSONObject jsonInput = new JSONObject();
            jsonInput.put("a", a);
            jsonInput.put("b", b);
            jsonInput.put("c", 0);
            jsonInput.put("name", name);
            jsonPayload.put("input", jsonInput);

            JSONObject jsonOutput = new JSONObject();
            jsonOutput.put("ketluan", ketLuan);
            jsonOutput.put("abc", "xyz");
            jsonOutput.put("nghiem", nghiemStr);
            jsonPayload.put("output", jsonOutput);

            // Thực thi kết nối mạng
            MediaType JSON = MediaType.get("application/json; charset=utf-8");
            RequestBody body = RequestBody.create(jsonPayload.toString(), JSON);
            Request request = new Request.Builder()
                    .url("https://k58kmt.tdh.io.vn/api")
                    .post(body)
                    .build();

            client.newCall(request).enqueue(new Callback() {
                @Override
                public void onFailure(Call call, IOException e) {
                    runOnUiThread(() -> tvKetQua.append("\n[API] Gửi thất bại!"));
                }

                @Override
                public void onResponse(Call call, Response response) throws IOException {
                    if (response.isSuccessful()) {
                        String resData = response.body().string();
                        runOnUiThread(() -> tvKetQua.append("\n[API] Trả về: " + resData));
                    }
                }
            });
        } catch (Exception e) {
            Toast.makeText(this, "Vui lòng nhập số hợp lệ!", Toast.LENGTH_SHORT).show();
        }
    }
}

--------------------------------
Từ màn hình chính bấm mở màn hình Giải toán. Nhập thử các số (Ví dụ: a = 4, b = 3), nhập tên rồi bấm tính toán. 
Đợi khoảng 1-2 giây khi dòng thông báo màu đen hiện chữ thành công: [API] Trả về: {"ok":1, "id":...} 
--------------------------------

# <img width="2000" height="1200" alt="image" src="https://github.com/user-attachments/assets/98ddc04d-fe49-442e-b6bc-56a76be41aab" />
** B6: 
LẬP TRÌNH NHÚNG TRÌNH DUYỆT WEB ĐỘNG TRUYỀN THAM SỐ MSSV
Hướng dẫn thực hiện: <br>
- Mở file WebViewActivity.java. Viết mã nguồn kích hoạt JavaScript cho WebView, nạp đường dẫn URL động bằng cách tự động ghép nối chuỗi tham số chứa mã sinh viên sinh viên của bạn (?masv=K225480106076) gửi lên server.

## Mã nguồn hoàn chỉnh WebViewActivity.java:

package com.example.baitaplon;

import android.os.Bundle;
import android.webkit.WebSettings;
import android.webkit.WebView;
import android.webkit.WebViewClient;
import androidx.appcompat.app.AppCompatActivity;

public class WebViewActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_web_view);

        WebView webView = findViewById(R.id.my_webview);
        
        WebSettings webSettings = webView.getSettings();
        webSettings.setJavaScriptEnabled(true); // Bật thực thi mã JS
        webView.setWebViewClient(new WebViewClient()); // Ép chạy trong app thay vì mở Chrome ngoài

        // Nối chuỗi mã số sinh viên vào đường dẫn web
        String myMssv = "K225480106076"; 
        String url = "https://k58kmt.tdh.io.vn?masv=" + myMssv;

        webView.loadUrl(url);
    }
}

-------------------------
Quay lại màn hình chính, bấm chọn nút mở màn hình WebView. Khi màn hình load xong dữ liệu thô (JSON) phản hồi từ hệ thống của thầy, hiển thị rõ ràng thông tin họ tên Nguyễn Lam Sơn cùng mã số sinh viên 
-------------------------

# <img width="2000" height="1200" alt="image" src="https://github.com/user-attachments/assets/ddfa1f08-4dae-4c4f-968b-313b89c1d8ab" />
# PHẦN 4: Tóm tắt lý thuyết toàn diện, cô đọng và hệ thống cho toàn bộ các nội dung xuất hiện trong Bài Tập Lớn
## 1: TÓM TẮT LÝ THUYẾT NỀN TẢNG MIT APP INVENTOR (LẬP TRÌNH KÉO THẢ)
## 1.1 Quy trình thiết kế và cấu hình giao diện
- Thanh công cụ (Palette): Là kho lưu trữ chứa toàn bộ các đối tượng giao diện được định nghĩa sẵn. Quy trình thiết kế dựa trên thao tác chọn và kéo - thả đối tượng từ Palette vào màn hình mô phỏng (Viewer).

- Bảng thuộc tính (Properties): Là nơi quản lý các thông số kỹ thuật (Kích thước, Màu sắc, Văn bản hiển thị). Việc thay đổi thuộc tính nhằm mục đích cá nhân hóa hiển thị và xác định trạng thái ban đầu của đối tượng.

## 1.2. Bản chất, ưu và nhược điểm của lập trình khối (Block)
** Bản chất: Chuyển đổi tư duy lập trình từ dạng văn bản (Text-based) sang dạng hình khối trực quan (Visual-based). Các hàm xử lý, biến số, cấu trúc logic if-else hay vòng lặp được đóng gói thành các mảnh ghép đồ họa. Khi lắp ghép các khối khớp nối với nhau, hệ thống tự động biên dịch sang mã máy.

- Ưu điểm: Loại bỏ hoàn toàn lỗi cú pháp (như thiếu dấu ;, sai dấu {}, viết sai từ khóa lệnh); phát triển ứng dụng cực nhanh.

- Nhược điểm: Bị giới hạn khả năng can thiệp sâu vào nhân hệ điều hành; khó tối ưu hiệu năng; khi logic app lớn thì giao diện block cực kỳ rối và khó gỡ lỗi (debug); file .apk đầu ra bị nặng.

- Tính năng Cái balo (Backpack): Đóng vai trò là bộ nhớ tạm (Clipboard) toàn cục, cho phép sao chép một cụm logic khối phức tạp từ màn hình này để mang sang tái sử dụng ở màn hình khác một cách nhanh chóng.

## 2 : TÓM TẮT LÝ THUYẾT KIẾN TRÚC ỨNG DỤNG ANDROID STUDIO
## 2.1. Vai trò của tệp định cấu hình AndroidManifest.xml
** Bản chất: File cấu hình tối cao nằm tại gốc của mọi dự án Android. Nó khai báo sơ đồ kiến trúc tổng thể cho hệ điều hành hiểu, bao gồm: tên gói (package), danh sách màn hình (Activity), biểu tượng (icon), và đặc biệt là danh sách các quyền hạn hệ thống.

Cơ chế xin quyền kết nối Internet: Android sử dụng cơ chế bảo mật cô lập (Sandbox). Ứng dụng mặc định khi cài đặt không được tự ý truy cập Internet để bảo vệ dữ liệu người dùng. Để kích hoạt, lập trình viên phải khai báo tường minh quyền truy cập mạng (INTERNET, ACCESS_NETWORK_STATE) và quyền truyền tải HTTP thô (usesCleartextTraffic="true").

## 2.2. Vòng đời ứng dụng Android (Activity Lifecycle) và hàm onCreate
Vòng đời ứng dụng: Hoạt động của một Activity di chuyển liên tục qua một chuỗi các trạng thái được giám sát nghiêm ngặt bởi hệ thống (Khởi tạo, Hiển thị, Tạm dừng, Dừng hẳn, Bị hủy) nhằm tối ưu dung lượng RAM và điện năng (Pin).

** Bản chất hàm onCreate(): Khi Activity được kích hoạt, hệ điều hành Android luôn gọi hàm callback onCreate() đầu tiên. Đây là "điểm khởi thủy" bắt buộc để nạp cấu trúc layout XML lên bộ nhớ (setContentView), ánh xạ thành phần giao diện vào code Java (findViewById), và thiết lập các hàm lắng nghe sự kiện ban đầu.

## 2.3. Nguyên lý tài nguyên chuỗi (strings.xml) và lỗi Hardcode text
- Hardcode text: Việc viết trực tiếp chữ hiển thị bằng văn bản thô vào code giao diện XML (Ví dụ: android:text="Nguyễn Lam Sơn") gọi là Hardcode. Tác hại là làm ứng dụng bị thắt nút cổ chai, rất khó khăn và dễ gây sai sót khi cần chỉnh sửa, bảo trì thông tin.

- Tác dụng của strings.xml: Gom toàn bộ văn bản vào một tệp quản lý tập trung.

- Cú pháp tham chiếu: Trong file XML gọi @string/tên_định_danh, trong mã Java gọi R.string.tên_định_danh (hoặc getString(...)).

- Cơ chế tự động hóa của OS: Hệ điều hành Android tích hợp sẵn công nghệ tự động quét file này dựa trên Ngôn ngữ hệ thống (Language) và Vị trí địa lý (Location) để tự động dịch thuật giao diện mà lập trình viên hoàn toàn không cần chỉnh sửa lại code Java.

## 3: TÓM TẮT LÝ THUYẾT TRUY XUẤT DỮ LIỆU & GIAO TIẾP MẠNG
## 3.1. Cơ chế lưu trữ offline với thư mục Assets
** Bản chất: Toàn bộ các file nằm trong Assets sẽ được nén đi kèm trực tiếp vào bên trong bộ cài đặt ứng dụng (.apk).

- Cú pháp truy cập: Sử dụng AssetManager qua câu lệnh getAssets().open("tên_file.txt").

- Lợi ích: Ứng dụng có thể truy xuất và đọc hiểu thông tin một cách tức thì, hoàn toàn độc lập và không phụ thuộc vào mạng Internet (Ngoại tuyến - Offline).

- Ứng dụng: Làm app cẩm nang offline, tài liệu hướng dẫn tĩnh, bộ từ điển tra cứu nhanh, dữ liệu cấu hình game đồ họa tĩnh.

## 3.2. Giao thức kết nối mạng API và định dạng JSON thời gian thực
- API (Application Programming Interface): Cổng dịch vụ chuẩn hóa cho phép ứng dụng di động gửi dữ liệu lên máy chủ và đồng bộ nhận phản hồi ngược lại.

- JSON (JavaScript Object Notation): Là định dạng chuẩn quốc tế dùng để đóng gói dữ liệu dưới dạng cặp Khóa (Key) : Giá trị (Value) rất gọn nhẹ, giúp truyền tải dữ liệu qua môi trường Internet nhanh chóng, đồng bộ mượt mà giữa các nền tảng lập trình khác nhau.

- Cấu trúc JSON lồng nhau gửi lên máy chủ Bộ môn: Được đóng gói nghiêm ngặt thành 3 phần:

- app_by: Chứa chuỗi định danh duy nhất của bạn (Mã số sinh viên K225480106076) để server phân loại bài làm.

- input: Khối đối tượng con chứa các tham số đầu vào nhập từ giao diện di động (hệ số a, hệ số b, hệ số c, tên sinh viên name).

- output: Khối đối tượng con chứa kết quả xử lý của thuật toán trên điện thoại (trạng thái ketluan và chuỗi nghiệm phương trình nghiem).
# PHẦN 5: TỔNG KẾT QUÁ TRÌNH THỰC HIỆN BÀI TẬP LỚN
- Trải qua quá trình nghiên cứu, tự lực giải quyết vấn đề và triển khai thực tế hệ thống phần mềm Bài tập lớn môn học Phát triển ứng dụng trên thiết bị di động (TEE0419), em đã đúc kết được những giá trị kiến thức sâu sắc sau:
## 1. Về mặt nhận thức lý thuyết và bản chất công nghệ
- Hiểu sâu sắc về cấu trúc nền tảng: Em đã hiểu rõ vai trò điều phối tối cao của file AndroidManifest.xml trong kiến trúc hệ điều hành Android. Từ đó biết cách phân quyền hệ thống một cách an toàn và quản lý luồng cấu trúc Activity khoa học.

- Tư duy quản trị tài nguyên chuyên nghiệp: Việc loại bỏ hoàn toàn mã độc lập (lỗi hardcode) và chuyển dịch toàn bộ sang tệp tài nguyên hệ thống strings.xml đã giúp em nắm vững tư duy đa ngôn ngữ hóa và nội địa hóa ứng dụng di động theo quy chuẩn công nghiệp.

- Làm chủ quy trình vòng đời: Hiểu được dòng chảy trạng thái thông qua các hàm callback vòng đời (Lifecycle), từ đó tối ưu hóa được vùng nhớ bộ đệm, giải phóng tài nguyên nền và ngăn chặn triệt để hiện tượng tràn bộ nhớ hay tiêu tốn năng lượng pin thiết bị một cách lãng phí.

## 2. Về mặt kỹ năng thực hành và giải quyết vấn đề thực tế
- Khai thác dữ liệu Offline & Online linh hoạt: Em đã biết cách thiết lập cấu trúc và truy xuất dữ liệu phi cấu trúc ngoại tuyến thông qua hệ thống Assets phục vụ các kịch bản ngoại tuyến. Song song với đó, em đã làm chủ kỹ năng kết nối, đóng gói dữ liệu thời gian thực theo cấu trúc đối tượng JSON phức tạp lồng nhau nhằm trao đổi thông tin đồng bộ với hệ thống máy chủ mạng (API) bên ngoài thông qua phương thức mạng POST.

- Làm chủ quy trình kiểm thử và gỡ lỗi trên máy thật: Thay vì lạm dụng máy ảo tiêu tốn tài nguyên máy tính, em đã hoàn toàn làm chủ kỹ năng cấu hình môi trường phát triển (Developer Options, USB Debugging) trên thiết bị di động vật lý. Kỹ năng này giúp em tiếp cận sát nhất với trải nghiệm thực tế của người dùng cuối, biết cách theo dõi bảng log và xử lý ngoại lệ bất đồng bộ hiệu quả khi có sự cố mất kết nối mạng.

## Lời cảm ơn: Bài tập lớn này không chỉ giúp em hoàn thành nghĩa vụ môn học, mà quan trọng hơn cả, nó đã đặt những viên gạch nền móng vững chắc giúp em định hình tư duy lập trình di động chuyên nghiệp, sẵn sàng cho việc phát triển các sản phẩm phần mềm thực tế trong tương lai.







