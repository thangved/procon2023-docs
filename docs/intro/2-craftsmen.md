# Thợ thủ công

Mỗi thợ thủ công có thể thực hiện các chuyển động sau mỗi lượt:

## Ở lại (STAY)

Thợ thủ công giữ nguyên vị trí. Không có hành động nào được thực hiện.

## Di chuyển (MOVE)

Thợ thủ công di chuyển theo một trong tám hướng xung quanh vị trí hiện tại

- [x] Lên (UP)
- [x] Xuống (DOWN)
- [x] Trái (LEFT)
- [x] Phải (RIGHT)
- [x] Phía trên bên trái (UPPER_LEFT)
- [x] Phía trên bên phải (UPPER_RIGHT)
- [x] Phía dưới bên trái (LOWER_LEFT)
- [x] Phía dưới bên phải (LOWER_RIGHT)

Tuy nhiên, **<u>họ không được phép di chuyển đến nơi Bức tường của đội khác được định vị cũng như Ao</u>**.
Ngoài ra, chỉ một Thợ thủ công được phép trên một khu vực được chia.
Bất kỳ Thợ thủ công nào cũng không thể di chuyển đến khu vực có bất kỳ Thợ thủ công nào ở một lượt trước lượt hiện tại.
Nếu hai Thợ thủ công bất kỳ thông báo di chuyển đến cùng một khu vực, bất kỳ ai trong số họ không thể di chuyển đến đó.
Nếu bất kỳ Thợ thủ công nào thông báo di chuyển đến khu vực mà họ không được phép di chuyển, thì hành động được phép đối với Thợ thủ công đó chỉ là “Ở lại”.

## Xây dựng (BUILD)

Tường có thể được xây dựng ở bất kỳ khu vực nào trong **<u>bốn khu vực liền kề</u>**.

- [x] Trên (ABOVE)
- [x] Dưới (BELOW)
- [x] Trái (LEFT)
- [x] Phải (RIGHT)

**<u>Bất kỳ bức tường không thể được xây dựng trên khu vực có bất kỳ Lâu đài, Tường của đối thủ hoặc Thợ thủ công nào</u>**.
Nếu bất kỳ Thợ thủ công nào thông báo xây Tường trên một khu vực như vậy, thì hành động được phép đối với Thợ thủ công đó chỉ là "Ở lại".

## Phá hủy (DESTROY)

Bạn có thể loại bỏ **<u>Tường của mình hoặc Tường của đối thủ</u>** khỏi bất kỳ khu vực nào trong **<u>bốn khu vực lân cận</u>**.

- [x] Trên (ABOVE)
- [x] Dưới (BELOW)
- [x] Trái (LEFT)
- [x] Phải (RIGHT)

Khi một Bức tường bị phá hủy, khu vực đó trở thành Trung lập hoặc Lãnh thổ.
Điều kiện chuyển sang Neutral hoặc Territory sẽ được giải thích sau.
Nếu bất kỳ Thợ thủ công nào tuyên bố phá hủy một khu vực không có Tường nào được xây dựng, thì hành động được phép đối với Thợ thủ công đó chỉ là "Ở lại".
