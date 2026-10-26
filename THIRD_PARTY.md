# Công cụ và nguồn thiết kế

- [skill-icons](https://github.com/tandpfun/skill-icons), bản 7f7e691e71aec64e8354bf697835e009d1ad80f8: 12 icon SVG trong assets/icons. Giấy phép MIT được giữ tại assets/icons/LICENSE.txt.
- [readme-typing-svg](https://github.com/DenverCoder1/readme-typing-svg): tạo assets/typing.svg qua dịch vụ công khai, với nội dung tiếng Việt và màu xanh mint. Font đã được nhúng trong SVG.
- [Platane/snk](https://github.com/Platane/snk), bản d8f6715049803e982ee5ff501b6b9b7d5deeb09b: tạo hoạt ảnh từ biểu đồ đóng góp của chính tungtungsahul.
- [awesome-github-profile-readme](https://github.com/abhisheknaiidu/awesome-github-profile-readme) và [github-profile-readme-generator](https://github.com/rahuldkjain/github-profile-readme-generator): tham khảo cấu trúc hồ sơ, phần công nghệ và bố cục dự án; không sao chép hồ sơ cá nhân hoặc cài các ứng dụng này làm Codex skill.
- [Pixelify Sans](https://github.com/google/fonts/tree/main/ofl/pixelifysans) cho tiêu đề lớn và [VT323](https://github.com/google/fonts/tree/main/ofl/vt323) cho kiểu terminal pixel có đủ dấu tiếng Việt. Font gốc và giấy phép SIL Open Font License được lưu tại assets/fonts. Chữ trong các hình SVG đã chuyển thành đường nét để hiển thị đồng nhất trên GitHub. Chữ thường của README dùng phông mặc định của GitHub.

Banner pixel và hai hình dự án được thiết kế riêng cho hồ sơ này. ScamGuard AI được ghi rõ là dự án phát triển cùng nhóm, liên kết tới repo gốc.

## Tự động cập nhật

Workflow .github/workflows/profile-visuals.yml cập nhật chữ chạy và hai bản sáng/tối của con rắn mỗi ngày lúc 00:23 UTC (07:23 giờ Việt Nam), khi sửa workflow hoặc khi chạy thủ công trong GitHub Actions. GitHub có thể chạy lịch muộn. Workflow dùng GITHUB_TOKEN mặc định, không cần thêm secret.

Các icon, chữ chạy và con rắn được lưu trong repo, nên trang hồ sơ không cần tải ảnh trực tiếp từ dịch vụ ngoài. Công cụ tạo chữ chạy được gọi khi workflow chạy. Mỗi lần tạo, workflow kiểm tra XML/SVG trước khi ghi file vào nhánh main.
