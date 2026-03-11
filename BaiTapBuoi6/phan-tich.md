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

**TL: Có thể cùng một class .title nhưng 1 trong 2 phần tử đó sẽ có thêm các selector có độ ưu tiên cao hơn nên sẽ hiện
thị màu dựa trên các selector ưu tiên đó**

Câu 6: Phần tử nào trong project của bạn có CSS phức tạp nhất? Liệt kê các selector tác động lên nó và giải thích
selector nào thắng cuối cùng.

**TL: h1 có class="title" id="special" style="color: black" trong index của dashboard là phức tạp nhất vì sử dụng đồng
thời cả 3 cách CSS gồm inline, internal, external.Các selector tác động lên nó là h1, .title, #special, inline
style.Internal CSS sẽ thắng external CSS tại vì được viết sau cùng.Nhưng inline CSS lại thắng internal CSS thì nó được
ưu tiên cao nhất trong 3 cách viết CSS.**

