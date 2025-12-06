# learn-git-flow

### 1-demo rebase 
Thay đổi lịch sử commit của branch

flow: 
```
Lấy các commit mới từ main

Gỡ (detach) commit của `feat-2` ra

Xếp commit của `feat-2` lên trên commit mới của main

Tạo ra commit mới có SHA hoàn toàn khác, dù nội dung giống
```

Conflict 
VD: lấy latest commit `main` vào `feat-2` (checkout `feat-2` & rebase main -> feat-2) => Fix conflict (current changes: commit của `main` và incoming changes: commit của `feat-2`)