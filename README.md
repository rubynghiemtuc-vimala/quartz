# Dự Án Từ Điển Pali (Obsidian + Quartz)

Chào mừng bạn đến với dự án Từ Điển Pali! Đây là kho chứa mã nguồn và dữ liệu của trang web Từ Điển Pali, được xây dựng dựa trên hệ thống ghi chú thông minh **Obsidian** và công cụ xuất bản web **Quartz**.

## 1. Cấu trúc thư mục (Vault)
Toàn bộ dữ liệu nội dung từ điển nằm trong thư mục `content/`. Khi làm việc, các thành viên trong team chỉ cần mở thư mục `content/` này bằng phần mềm **Obsidian**.

Cấu trúc chi tiết của thư mục `content/`:
- **`0_Nhap.md` (Trạm trung chuyển):** Nơi để paste (dán) văn bản thô từ Word/PDF vào. Obsidian sẽ giữ lại các định dạng in đậm, in nghiêng, bảng biểu. Sau đó có thể dùng công cụ để tự động cắt nhỏ.
- **`1_Tu_Vung/`:** Chứa các file từ vựng đơn lẻ (mỗi từ một file). Đây là trái tim của từ điển.
- **`2_Bai_Hoc/`:** Chứa các bài chú giải, ngữ pháp, các bài học dài có phân tích câu Pali.
- **`3_Chu_De/`:** Chứa các file tổng hợp (MOC - Map of Content), phân loại theo các chủ đề lớn (ví dụ: Thanh Tịnh Đạo, Các bậc Thánh, Kiết sử...).
- **`99_Templates/`:** Chứa các khuôn mẫu (nếu có) để tạo file nhanh.

## 2. Quy tắc biên soạn (Dành cho Team)

1. **Giữ nguyên bản gốc:** Các trích đoạn kinh điển, chú giải Pali phải được giữ nguyên vẹn 100% ngữ pháp và cấu trúc câu của Thầy.
2. **Định dạng Pali:** 
   - Chữ tiếng Việt giải thích: Viết bình thường.
   - Chữ tiếng Pali: Viết *in nghiêng* (`*chữ*`).
   - Các từ khóa quan trọng/định nghĩa: Viết **in đậm** (`**chữ**`).
   - Các từ khóa cực kỳ quan trọng: ***In đậm & In nghiêng*** (`***chữ***`).
3. **Liên kết chéo (Wikilink):** Khi nhắc đến một thuật ngữ Pali quan trọng trong bài, hãy bọc nó trong dấu ngoặc vuông `[[ ]]` (ví dụ: `[[Saddhammo]]`). Điều này giúp từ điển tự động tạo mạng lưới liên kết thông minh.

## 3. Cách cập nhật Web (Deploy)
Trang web được tự động cập nhật (Auto-deploy) thông qua **Cloudflare Pages**. 
Để đưa bài viết mới lên web, team chỉ cần làm 2 bước:
1. Viết bài và chỉnh sửa xong trong Obsidian.
2. Dùng Git (hoặc GitHub Desktop) để **Commit** và **Push** mã nguồn lên kho chứa (Repository) này. 
3. Chờ 2 phút, Cloudflare sẽ tự động kéo dữ liệu mới và cập nhật giao diện web!

---
*Được khởi tạo và thiết lập tự động - Chúc team biên soạn và học tập tinh tấn!*
