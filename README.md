# 🏪 Shop Mini - Quản lý doanh thu & kho hàng

> Ứng dụng quản lý doanh thu theo tuần và kho hàng nguyên liệu cho shop nhỏ, chạy hoàn toàn trên trình duyệt với đồng bộ GitHub.

---

## ✨ Tính năng

| Tính năng | Mô tả |
|-----------|-------|
| 📊 **Doanh thu tuần** | Theo dõi số đơn và doanh thu 7 ngày (T2-CN), thêm/xóa tuần dễ dàng |
| 📦 **Kho hàng** | Quản lý nguyên liệu, tính toán tồn kho tự động, cảnh báo cần mua |
| 🛒 **Danh sách mua** | Tự động liệt kê vật liệu sắp hết để nhập hàng |
| 📝 **Ghi chú** | Ghi lại các việc cần làm, nhắc nhở nội bộ |
| ☁️ **Đồng bộ GitHub** | Lưu dữ liệu lên GitHub, truy cập từ mọi nơi |
| 🔒 **Chế độ chỉnh sửa** | Khóa/mở khóa bằng mật khẩu để tránh sửa nhầm |
| 📤 **Export** | Xuất JSON, CSV hoặc in PDF |

---

## 🚀 Cách dùng

1. Mở file `index.html` trong trình duyệt (hoặc deploy lên GitHub Pages)
2. Bấm **Edit** → nhập mật khẩu `123456` để mở khóa chỉnh sửa
3. Nhập dữ liệu doanh thu, kho hàng, ghi chú
4. Bấm **Cấu hình** → nhập GitHub Token + Repo → **Lưu cấu hình**
5. Bấm **Save** để đồng bộ lên GitHub

---

## 🔧 Cấu hình GitHub

1. Vào [GitHub Settings → Developer settings → Personal access tokens → Fine-grained tokens](https://github.com/settings/tokens?type=beta)
2. Tạo token mới với quyền **Contents: Read + Write**
3. Tạo repo mới (ví dụ: `shop-mini-data`) và thêm 1 file `README.md` bất kỳ để repo có commit
4. Trong app, nhập:
   - **Token**: `ghp_xxxxxxxxxxxx`
   - **Repo**: `username/shop-mini-data`
   - **Branch**: `main`
   - **Path**: `data.json`

---

## 📁 Cấu trúc dữ liệu (`data.json`)

```json
{
  "shopName": "SHOP MINI",
  "weeks": [
    {
      "weekNumber": 26,
      "year": 2026,
      "days": [
        { "date": "29/06/2026", "dayOfWeek": "T2", "orders": 10, "money": 18000 }
      ]
    }
  ],
  "inventory": [
    { "name": "Ly nhựa 500ml", "current": 1000, "used": 50, "remaining": 950 }
  ],
  "notes": [
    { "text": "Nhập thêm ly nhựa", "time": "22/06/2026 08:30" }
  ]
}
```

---

## 🛡️ Bảo mật

- **Token GitHub** chỉ lưu trong `localStorage` trình duyệt, **không bao giờ** đẩy lên GitHub
- Dữ liệu đồng bộ lên GitHub đã được **xóa sạch token** trước khi push
- Mật khẩu mặc định: `123456` (có thể đổi trong code)

---

## 📝 License

MIT License — Tự do sử dụng và chỉnh sửa.

---

<p align="center">Made with ☕ for small shop owners</p>
