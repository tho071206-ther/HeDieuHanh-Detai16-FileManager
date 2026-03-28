# HeDieuHanh-Detai16-FileManager

Mục I: CRUD + hiển thị file/folder
Mục II: Navigation + TreeView + Copy/Move
Mục III: Search + Properties
# Ai làm mục nào thì chỉ tập trung đúng phần đó, không đụng chéo
File nào thuộc phần mình thì code → Không cần làm dư
Không sửa file người khác nếu chưa hỏi
Tránh conflict Git
Nếu cần sửa → báo trước
Commit rõ ràng
Test riêng phần mình trước khi push
Tránh lỗi làm crash toàn bộ project
Không tự ý đổi tên file / folder
# Mỗi người pull bài về và làm 1 branch riêng: Không code trực tiếp trên main
# FileManagerApp

## Models  
###  FileItem.cs 


## Interfaces 
### 	 IFileService.cs    (Mục I + II)
//GetFiles(), GetFolders()  (Mục I)
//Create()
//Delete()
//Rename()
//Copy / Move    (Mục II)
## Services 
### 	 FileService.cs   (Mục I + II + III)
//CRUD file/folder   (Mục I)
//Copy / Move    (Mục II)
//Lấy FileInfo    (Mục III)
// Search file


## ViewModels
### 	 MainViewModel.cs       (Mục I)
// Hiển thị danh sách file/folder (ListView/GridView)
// Tạo mới (Create file/folder)
// Đổi tên (Rename)
// Xóa (Delete)
// Gọi FileService xử lý
###    NavigationViewModel.cs (Mục II)
// TreeView thư mục
// Click folder → load file
// Copy / Cut / Paste
//  Xử lý path
###   SearchViewModel.cs     (Mục III)
// Tìm kiếm file theo tên / đuôi
// Filter danh sách
//  Lấy thông tin file:
/// + Size
/// + Ngày tạo
// Xử lý thuộc tính:
/// + ReadOnly
/// + Hidden
### BaseViewModel.cs
### RelayCommand.cs


## Views
### 	NavigationView.xaml & NavigationView.xaml.cs   (Mục II)
// - UI TreeView bên trái
// - Hiển thị file bên phải
### SearchView.xaml &  SearchView.xaml.cs     (Mục III)
// - TextBox nhập search
// - Hiển thị kết quả
// - Hiển thị properties


