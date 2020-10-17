# Multi Agent Search
## Câu 1: Reflex Agent
Dùng mảng để lưu lại vị trí thức ăn. Sử dụng khoảng cách manhattan để đánh giá. Duyệt qua toàn bộ thức ăn ở gần mình nhất. Nếu phát hiện pacman quá gần ma thì phải tránh chúng vì điểm ở bước đi gần thức ăn tăng lên bằng khoảng cách đến thức ăn và giảm đối với ma nên ta cần tránh xa ma ra. Cuối cùng hàm trả về điểm với minFood nhỏ nhất.
## Câu 2: Minimax
Tính toán dựa trên việc ma di chuyển tối ưu. Nếu thắng, thua hoặc độ sâu đã duyệt đến vị trị cần tìm, sẽ trả về hàm đánh giá. Khi index = 0 là pacman, return hàm maximizer, index > 0 là ma, return hàm minimizer. Hàm maximizer tìm giá trị lớn nhất trong trạng thái tiếp theo và trả về hành động với trạng thái đó. Hàm minimizer thì ngược lại.
## Câu 3: Alpha-Beta Pruning
Giống câu 2 nhưng có thêm cắt tỉa Alpla-Beta (Alpla là giá trị tốt nhất của maximizer, Beta là giá trị tốt nhất của min).
## Câu 4: Expectimax
Tính toán dựa trên việc ma di chuyển ngẫu nhiên. Giống câu 2 nhưng hàm minimizer thay đổi, thay vì tìm giá trị nhỏ nhất, hàm sẽ đánh giá dựa trên giá trị trung bình.
## Câu 5: Evaluation Function
Giống câu 1, hàm được tính bằng khoảng cách đến thức ăn gần nhất, số lượng thức ăn còn lại, viên sức mạnh còn lại và khoảng cách tới ma.

