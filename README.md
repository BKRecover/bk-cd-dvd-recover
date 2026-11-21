# BK CD/DVD Recover

**Free Windows software that reads damaged CDs and DVDs — scratched, dirty, oxidised or flaky — and gets the files off them.**
Made by BK RECOVER (Vietnam Computer Solutions JSC). English and Vietnamese.

*Phần mềm miễn phí cho Windows: đọc đĩa CD/DVD xước, bẩn, oxy hoá, đọc chập chờn và lấy dữ liệu ra. Của BK RECOVER. [Tiếng Việt ở dưới.](#tiếng-việt)*

---

## Download

**[Latest release →](https://github.com/BKRecover/bk-cd-dvd-recover/releases/latest)** — `BKCdDvdRecover-Setup-<version>.exe` plus its `.sha256`.

Requirements: Windows 10 or 11, 64-bit, a CD/DVD drive, administrator rights (the software talks to the drive directly). Nothing else to install.

### "Windows protected your PC"
The installer is not yet code-signed, so SmartScreen shows this warning. Click **More info → Run anyway**.
To be sure the file is ours, compare its SHA-256 with the `.sha256` file on the release page — in PowerShell:

```powershell
Get-FileHash .\BKCdDvdRecover-Setup-1.0.0-beta.exe -Algorithm SHA256
```

## What it does

1. **Choose disc** — every CD/DVD drive is listed with what it holds.
2. **Save to** — pick a folder on a hard disk; the disc is first copied sector by sector into an image (`.iso`, or `.bin`+`.cue` for CDs) with a map of what was read.
3. **Read disc** — a fast pass over the good part, then the edges of the damage, then repeated retries of the bad spots. A live picture of the disc shows read / damaged / not yet read / unrecorded areas. Pause and resume at any time, even after closing the program; a cleaning guide appears when the disc reads badly, and a 15-minute rest is offered when a warm disc slows down.
4. **Results** — the files on the disc (ISO 9660 / Joliet: data discs, DVD-Video, VCD) with each one's state; save the ones you want, with a report.

The software **only reads**. It never writes to a disc, never connects to the internet, and collects nothing.

## This is a beta

It is complete and usable; we are still polishing it. If something goes wrong, please [open an issue](https://github.com/BKRecover/bk-cd-dvd-recover/issues) and attach the `.log` file from your destination folder (or `loi-khoi-dong.txt` from the installation folder if the window never appeared). Not yet: UDF discs, CD Audio to WAV, Blu-ray.

## Terms

Free for everyone, including shops and service companies. Provided as is; see [EULA-en.txt](EULA-en.txt). The source code is not published.

Discs that stay unreadable after cleaning and repeated passes can often be recovered at the BK RECOVER lab with polishing and specialised equipment: [bkrecover.com](https://bkrecover.com) · [recoverdata.com.vn](https://recoverdata.com.vn) · support@bkrecover.com · +84 1900 636 196

---

## Tiếng Việt

**BK CD/DVD Recover** là phần mềm miễn phí của BK RECOVER (Công ty CP Giải pháp Máy tính Việt Nam) để lấy dữ liệu từ đĩa CD/DVD bị xước, bẩn, oxy hoá hoặc đọc chập chờn.

### Tải về
**[Bản mới nhất →](https://github.com/BKRecover/bk-cd-dvd-recover/releases/latest)** — tệp `BKCdDvdRecover-Setup-<phiên bản>.exe` và tệp `.sha256` đi kèm.

Cần Windows 10/11 64-bit, ổ CD/DVD và quyền quản trị (phần mềm nói chuyện trực tiếp với ổ đĩa). Không cần cài thêm gì.

### Cảnh báo "Windows protected your PC"
Bộ cài chưa ký số nên SmartScreen hiện cảnh báo này. Bấm **More info → Run anyway**. Muốn chắc chắn tệp là của chúng tôi, đối chiếu SHA-256 với tệp `.sha256` trên trang tải về (PowerShell: `Get-FileHash <tệp> -Algorithm SHA256`).

### Phần mềm làm gì
1. **Chọn đĩa** — liệt kê các ổ CD/DVD và đĩa đang có.
2. **Nơi lưu** — chọn thư mục trên ổ cứng; đĩa được chép từng sector thành ảnh (`.iso`, hoặc `.bin`+`.cue` với CD) kèm bản đồ chỗ đã đọc.
3. **Đọc đĩa** — lượt nhanh qua phần lành, rồi sát mép chỗ hỏng, rồi đọc lại chỗ hỏng nhiều lần. Hình đĩa hiện vùng đã đọc / lỗi / chưa đọc / chưa ghi. Tạm dừng và đọc tiếp bất cứ lúc nào, kể cả sau khi tắt máy; có hướng dẫn lau đĩa khi đĩa đọc kém và đề nghị nghỉ 15 phút khi đĩa nóng.
4. **Kết quả** — danh sách file (ISO 9660 / Joliet: đĩa dữ liệu, DVD phim, VCD) kèm tình trạng; chọn file để lưu, có báo cáo.

Phần mềm **chỉ đọc**: không bao giờ ghi lên đĩa, không kết nối mạng, không thu thập gì.

### Bản Beta
Dùng được đầy đủ, đang tiếp tục hoàn thiện. Gặp lỗi xin [báo ở đây](https://github.com/BKRecover/bk-cd-dvd-recover/issues) kèm tệp `.log` trong thư mục lưu (hoặc `loi-khoi-dong.txt` trong thư mục cài nếu không mở được cửa sổ). Chưa có: đĩa UDF, CD Audio ra WAV, Blu-ray.

### Điều khoản
Miễn phí cho mọi người, kể cả cửa hàng và công ty dịch vụ. Cung cấp nguyên trạng; xem [EULA.txt](EULA.txt). Mã nguồn không công bố.

Đĩa vẫn không đọc được sau khi lau và đọc lại nhiều lần: phòng lab BK RECOVER có thể đánh bóng và đọc bằng thiết bị chuyên dụng — [bkrecover.com](https://bkrecover.com) · [recoverdata.com.vn](https://recoverdata.com.vn) · support@bkrecover.com · 1900 636 196
