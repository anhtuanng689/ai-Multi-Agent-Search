1. Reflex Agent
python autograder.py -q q1
2. Minimax
python autograder.py -q q2
3. Alpha-Beta Pruning
python autograder.py -q q3
4. Expectimax
python autograder.py -q q4
5. Evaluation Function
python autograder.py -q q5

Đầu tiên, em dùng list để lưu vị trí các thức ăn lại. Ở vòng for thứ nhất, em cho nó tập trung đi ăn các thức ăn gần nhất bằng hàm tính manhattan. Ở vòng for thứ hai là tìm ra con ma gần nhất so với vị trí của pacman để tránh nó. Nếu khoảng cách manhattan giữa vị trí pacman và con ma là 1 thì em cho trả về âm vô cùng vì không bao giờ max được nên k lấy. Cuối cùng hàm trả về điểm với minFood nhỏ nhất.
