# AI

DFS: ! Sử dụng Stack
	- DFS là thuật toán duyệt từ gốc và phát duyệt ra xa nhất theo mỗi nhánh
	- path là danh sách đường đi từ đầu tới đích
	- pathToCurrent là danh sách đường đi tới node đang duyệt
Giải thuật :
	Push startState vào stack;
	pop 1 phần tử từ stack ra lưu vào biến currState và bắt đầu duyệt;
	Chạy 1 vòng lặp với điều kiện dừng lại khi currState là goalState;
		kiểm tra xem currstate có nằm trong Visited hay ko;
			nếu không có thì thêm vào visited;
			lấy successor tại currState;
			push các node con của currState vào stack, cập nhật path, cập nhật pathToCurrent và tiếp tục duyệt
	Khi duyệt xong trả về path

BFS: ! Sử dụng Queue
	BFS là thuật toán duyệt theo từng bậc theo chiều ngang. Đầu tiên sẽ duyệt các Node kề với startState, sau đó sẽ duyệt đến các Node kề với các Node vừa duyệt và cứ thế rộng ra cho đến khi tìm thất đường đi đến goalState.

Giải thuật :
	ngoài việc sử dung Queue thay cho Stack thì về cơ bản giải thuật của BFS và DFS là giống nhau

UFS: ! Sử dụng PriorityQueue
	UFS là thuật toán dựa vào chi phí thấp nhất tính từ nút gốc để tìm đường đi, về bản chất thì cũng khá tương đồng với BFS nhưng nó sẽ chọn state có chi phí thấp nhất để ưu tiên duyệt trước.

A*
	A* cũng sử dụng PriorityQueue nhưng ngoài chi phí ra nó còn có thêm giá trị Heuristic để quyết định xem sẽ chọn state nào để duyệt trước.



	 
