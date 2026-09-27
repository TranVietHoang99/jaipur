# 🐪 Jaipur

Game bài **Jaipur** cho 2 người, chơi ngay trên trình duyệt, không cần server hay tài khoản.

## Chế độ chơi
- **Chơi với máy**: nhập tên, bấm *Chơi với máy*.
- **Online 1 đấu 1**: bấm *Tạo phòng*, gửi mã phòng hoặc link cho bạn bè; bạn bè nhập mã và bấm *Vào phòng*.
  Người tạo phòng phải **giữ tab mở** suốt trận, vì máy chủ phòng giữ trạng thái ván chơi.

## Luật tóm tắt
Mỗi lượt chọn một việc:
- **Lấy 1 hàng** từ chợ (tay tối đa 7 lá, lạc đà không tính).
- **Đổi hàng**: lấy từ 2 lá hàng trở lên ở chợ, đưa lại đúng số lá đó bằng hàng trên tay và/hoặc lạc đà. Không được đổi cùng loại hàng.
- **Lấy tất cả lạc đà** ở chợ.
- **Bán hàng**: chỉ bán 1 loại mỗi lượt. Kim cương, vàng, bạc phải bán ít nhất 2 lá. Bán 3/4/5+ lá được token thưởng.

Ván kết thúc khi đã hết 3 loại token hàng, hoặc chồng bài không đủ để bổ sung chợ. Ai nhiều lạc đà hơn được +5.
Thắng 2 ván là thắng trận.

## Cách bấm
- Chọn 1 lá ở chợ → nút **Lấy**.
- Chọn ≥2 lá ở chợ, rồi chọn lá trên tay và/hoặc bấm **+** ở đàn lạc đà → nút **Đổi**.
- Chỉ chọn lá trên tay → nút **Bán**.

## Kỹ thuật
Một file `index.html` duy nhất. Kết nối P2P bằng [PeerJS](https://peerjs.com/) (WebRTC), giống Sequence Mèo.
Chạy thử: `npx http-server jaipur -p 5179`.
