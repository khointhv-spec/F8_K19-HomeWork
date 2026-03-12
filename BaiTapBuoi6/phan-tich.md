Câu 1: Selector nào có độ ưu tiên cao nhất trong CSS?

**TL: Inline style**

Câu 2: Nếu một phần tử HTML có cả h1, .title, và #main cùng set color — selector nào thắng? Tại sao?

**TL: #main-vì id là selector có độ ưu tiên cao hơn so với tag và class**

Câu 3: Nếu bạn thêm style="color: pink" trực tiếp vào phần tử ở Câu 2, kết quả thay đổi như thế nào?

**TL: Sẽ thay đổi color thành màu pink vì đang dùng inline style**

Câu 4: Tại sao theme.css có thể override style từ base.css? Điều kiện để override thành công là gì?

**TL: Vì theme.css được link sau base.css nên sẽ override được.Điều kiện để override thành công là các selector trong
theme.css phải giống như base.css và được load sau**

Câu 5: Trong project của bạn, có hai phần tử đều dùng class .title nhưng hiển thị màu khác nhau. Giải thích tại sao.

**TL: Câu 5: Ví dụ trong home/index.html:**
- h1 có class="title" id="main": selector #main (specificity 1-0-0) thắng .title (0-1-0) → màu PINK
- h2 có class="title": chỉ có .title (0-1-0) → bị theme.css override → màu TEAL
**Hai phần tử đều dùng .title nhưng h1 có thêm #main với specificity cao hơn nên màu khác.**

Câu 6: Phần tử nào trong project của bạn có CSS phức tạp nhất? Liệt kê các selector tác động lên nó và giải thích
selector nào thắng cuối cùng.

**TL: h1 có class="title" id="special" style="color: black" trong index của dashboard là phức tạp nhất vì sử dụng đồng
thời cả 3 cách CSS gồm inline, internal, external.Các selector tác động lên nó là h1, .title, #special, inline
style.Internal CSS sẽ thắng external CSS tại vì cùng specificity, nên rule viết sau (internal) thắng rule viết trước (external).Nhưng inline CSS lại thắng internal CSS thì nó được
ưu tiên cao nhất trong 3 cách viết CSS.**

