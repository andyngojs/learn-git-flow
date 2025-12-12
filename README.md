# Git Flow

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
VD: lấy latest commit `main` vào `feat-2` (checkout `feat-2` & rebase main -> feat-2) => Fix conflict (current changes: commit của `main` và incoming changes: commit của `feat-2` nếu dùng VSCODE)

Steps:
- git checkout sang target branch để lấy latest code
- checkout về nhánh của mình
- git rebase [tên target branch] / (rigtht-click target branch - choose 'rebase current changes onto [target branch]' nếu dùng source tree)
- Fix confict (Nếu có)
- Sau rebase, nhớ push code lên remote `git push --force-with-lease` (để thay đổi lịch sử commit trên remote khớp với local.)

### Commit 

Commit theo convention: https://www.conventionalcommits.org/en/v1.0.0/
