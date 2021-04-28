# Game
# VideoDEMO

https://drive.google.com/file/d/1WYVlpU2-x7yh_qqGsr_HRvDElS2vtuTS/view?usp=sharing

# Technologies

Project sử dụng IDE và các thư viện sau:

- Code::blocks 17.12 mingw
- SDL2 image devel 2.0.5 mingw
- SDL2 ttf devel 2.0.15 mingw
- SDL2 devel 2.0.5 mingw

# Contents

## Các tính năng và thuật toán của trò chơi :

- Dùng *isPlaying* đảm bảo là còn *đúng* thì chạy game.
- Trong khi chơi thì có *isRunning* để đảm bảo là *còn sống* khi *chết* thì xóa và trở về Menu.
- Có nút Quit trong khi chơi nhưng nó cũng chỉ đưa về Menu và coi lượt chơi dó là thất bại.
- Thao tác ấn chỉ bằng chuột trái.
- Cách thức chơi ở trong phần *?* ở góc trái màn hình.
- Nút *exit* là cách thức để tắt trò chơi.
- Nút *Play* và *Replay* để chơi và làm mới *Engine*.
- Nút *X* để thoát khỏi phần *?* .
- Điểm ở đây là thời gian.
- Tốc độ di chuyển của các vật không thay đổi *RẤT DỄ CHƠI* trừ khi bạn đen.
- Thao tác ở *Menu* chỉ bao gồm thao tác Nhập giữ liệu từ chuột .

## Các hàm của trò chơi:

### Character:
- Khởi tạo , cập nhật vị trí và xóa.
- *AmongUs* là nhân vật chính *Prevent* là các vật cản.
### Input:
- Nhập dữ liệu gồm chuột, bàn phím, và thao tác khác.
- Triển khai các thao tác khi có *dữ liệu*.
### Conllision:
- Kiểm tra va chạm.
- Áp dụng bố cục vuông nên thu hẹp giới hạn va chạm vào trong của vật cản.
### Core:
- Khởi tạo phần trò chơi.
### Graphics:
- Khởi tạo đồ họa.
- Vẽ chữ với phông chữ và cỡ chữ mặc định (Text).
### Object:
- Hàm để khởi tạo nhiều *Prevent*.
### Physics:
- Gồm hàm tính toán và khởi tạo vector 2D.
- *RigidBody* : Xác định vị trí , vận tốc qua lực tác động vào vật 1 cách ổn định.
### Menu:
#### Menu của game gồm các tính năng: 
- *Play* và *Replay*: chơi và bắt đầu lại trò chơi.
- *Exit* : thoát game.
- *?* : cốt truyện và cách chơi game ( RenderH1, RenderH2 ).
#### Menu còn đảm bảo các cách kết thúc trò chơi khác nhau :
- Thắng khi va chạm với phi thuyền cuối cùng ( RenderV ).
- Thua khi va chạm hoặc rớt ( RenderM và *dead = true* ).
- CỐ TÌNH THUA khi không va chạm với phi thuyền cuối cùng ( RenderL ).

