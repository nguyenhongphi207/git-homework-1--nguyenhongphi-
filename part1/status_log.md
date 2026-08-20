nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        part1/

nothing added to commit but untracked files present (use "git add" to track)



nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   part1/notes.txt
        new file:   part1/todo.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        part1/draft.md
        part1/status_log.md


\ No newline at end of file
(END)
--- a/part1/todo.txt
+++ b/part1/todo.txt
@@ -1 +1,3 @@
 do homework
+play game
+eat 
\ No newline at end of file
(END)



#vì sao tùy chọn -a chỉ hoạt động đối với các tệp đã được theo dõi trước đó (tracked files).?

    Giải thích dựa trên tài liệu: Tùy chọn -a (hoặc --all) cho phép Git tự động phát hiện, đưa các tệp có thay đổi vào vùng Staging Area và commit chúng ngay lập tức, bỏ qua bước chạy lệnh git add thủ công. Tuy nhiên, cơ chế này chỉ áp dụng cho những tệp đã được theo dõi (tracked). Đối với các tệp chưa được theo dõi (untracked) (ví dụ như tệp mới tạo hoàn toàn chưa từng được thêm vào Git), Git không quản lý chúng nên không thể tự động đưa vào vùng chờ. Do đó, tệp untracked vẫn bắt buộc phải dùng lệnh git add <file> thủ công lần đầu


#sự khác biệt giữa fetch và pull ?
git fetch: Chỉ thực hiện tải toàn bộ dữ liệu, các commit mới và thông tin lịch sử từ máy chủ từ xa (remote repository) về kho lưu trữ cục bộ trên đĩa cứng của bạn. Nó cập nhật các nhánh remote-tracking (ví dụ: origin/main) nhưng không tự động trộn hay làm ảnh hưởng đến thư mục làm việc hiện tại của bạn. Lệnh này rất an toàn vì bạn có thể kiểm tra mã nguồn trước khi trộn.
git pull: Là một lệnh gộp tự động hoạt động theo nguyên lý: git pull = git fetch + git merge. Nó không chỉ tải các thay đổi mới về mà còn ngay lập tức tiến hành gộp (merge) thẳng các thay đổi đó trực tiếp vào thư mục làm việc hiện tại của bạn. Lệnh này giúp đồng bộ nhanh nhưng có thể gây ra xung đột (merge conflicts) nếu bạn cũng đang có những chỉnh sửa chưa đồng bộ trên cùng dòng tệp.