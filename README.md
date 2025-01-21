<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Luyện Tập và Vận Dụng Bài 16, 17, 18</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 20px;
            background-color: #f4f4f9;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .main-title {
            text-align: center;
            font-size: 24px;
            font-weight: bold;
            color: #e74c3c;
            margin-bottom: 30px;
        }
        h1 {
            color: #e74c3c;
            text-transform: uppercase;
            margin-bottom: 15px;
        }
        h2 {
            color: #3498db;
            margin-top: 20px;
        }
        p {
            margin: 10px 0;
        }
        ol {
            margin: 10px 0;
            padding-left: 20px;
        }
        li {
            margin: 5px 0;
        }
        code {
            background: #f4f4f4;
            padding: 2px 4px;
            border-radius: 4px;
        }
        .highlight {
            background-color: #fdebd0;
            padding: 10px;
            border-left: 4px solid #e74c3c;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="main-title">LUYỆN TẬP, VẬN DỤNG BÀI 16, 17, 18</div>

        <!-- Bài 16 -->
        <h1>Bài 16</h1>
        <ol>
            <li><strong>LUYỆN TẬP 1:</strong> Phần tử HTML có thể ẩn đi trên trang web được không? Nếu có thì dùng lệnh CSS gì?
                <div class="highlight">
                    <p><strong>Trả lời:</strong> Có thể ẩn phần tử HTML bằng cách sử dụng:</p>
                    <code>visibility: hidden;</code>
                    <p>hoặc:</p>
                    <code>display: none;</code>
                </div>
            </li>
            <li><strong>LUYỆN TẬP 2:</strong> Hãy giải thích ý nghĩa của định dạng sau:
                <div class="highlight">
                    <code>.test .test_more { background-color: red; }</code>
                    <p><strong>Giải thích:</strong> Định dạng này áp dụng màu nền <code>red</code> cho bất kỳ phần tử HTML nào có lớp <code>test_more</code> nằm trong phần tử có lớp <code>test</code>.</p>
                </div>
            </li>
            <li><strong>VẬN DỤNG 1:</strong> Có cách nào định dạng các đoạn P1, P2, P3 khác nhau và giữ nguyên định dạng cho các đoạn còn lại không? Hãy nêu cách giải quyết.
                <div class="highlight">
                    <p><strong>Trả lời:</strong></p>
                    <ul>
                        <li>Gắn lớp <code>important</code> cho P1: <code>&lt;p class="important">P1&lt;/p&gt;</code>.</li>
                        <li>Gắn lớp <code>normal</code> cho P2 và P3: <code>&lt;p class="normal">P2&lt;/p&gt;</code>, <code>&lt;p class="normal">P3&lt;/p&gt;</code>.</li>
                        <li>Sử dụng CSS:
                            <pre>
.important {
    color: red;
    font-weight: bold;
}
.normal {
    color: blue;
    font-style: italic;
}
                            </pre>
                        </li>
                    </ul>
                </div>
            </li>
            <li><strong>VẬN DỤNG 2:</strong> Có thể định dạng các khung với thông số viền khác nhau không? Nếu có, hãy trình bày cách thực hiện.
                <div class="highlight">
                    <p><strong>Trả lời:</strong> Hoàn toàn có thể sử dụng CSS:</p>
                    <pre>.box {
    border-top: 3px solid red;
    border-bottom: 5px dashed blue;
    border-left: 2px dotted green;
    border-right: 4px double black;
}
                    </pre>
                    <p>Ví dụ minh họa: <code>&lt;div class="box">Nội dung&lt;/div&gt;</code>.</p>
                </div>
            </li>
        </ol>

        <!-- Bài 17 -->
        <h1>Bài 17</h1>
        <ol>
            <li><strong>LUYỆN TẬP 1:</strong> Giải thích sự khác nhau giữa hai định dạng sau:
                <div class="highlight">
                    <code>#p123 + p { color: red; }</code>  
                    <code>h2#p123 + p { color: red; }</code>  
                    <p><strong>Trả lời:</strong></p>
                    <ul>
                        <li><code>#p123 + p</code>: Áp dụng cho thẻ <code>p</code> ngay sau phần tử có ID <code>p123</code>.</li>
                        <li><code>h2#p123 + p</code>: Áp dụng cho thẻ <code>p</code> ngay sau một thẻ <code>h2</code> có ID <code>p123</code>.</li>
                    </ul>
                </div>
            </li>
            <li><strong>LUYỆN TẬP 2:</strong> Trong phần thực hành, cần định dạng các tên riêng (người, tổ chức) bằng cách đóng khung và in nghiêng. Thực hiện như sau:
                <div class="highlight">
                    <pre>
.name {
    font-style: italic; /* In nghiêng */
    border: 1px solid #000; /* Đóng khung */
    padding: 2px; /* Thêm khoảng cách */
    display: inline-block; /* Gọn gàng */
}
                    </pre>
                </div>
            </li>
            <li><strong>VẬN DỤNG 1:</strong> Tìm hiểu thêm các dạng pseudo-class khác, nêu ý nghĩa và tìm ví dụ ứng dụng thực tế.
                <div class="highlight">
                    <p><strong>Trả lời:</strong></p>
                    <ul>
                        <li><code>:hover</code>: Kích hoạt khi người dùng di chuột qua phần tử.</li>
                        <li><code>:active</code>: Kích hoạt khi phần tử đang được nhấn giữ.</li>
                        <li><code>:focus</code>: Kích hoạt khi phần tử đang trong trạng thái focus.</li>
                        <li><code>:nth-child()</code>: Chọn các phần tử con dựa trên vị trí.</li>
                    </ul>
                </div>
            </li>
            <li><strong>VẬN DỤNG 2:</strong> Tìm hiểu thêm các dạng pseudo-element khác, nêu ý nghĩa và tìm ví dụ ứng dụng thực tế.
                <div class="highlight">
                    <p><strong>Trả lời:</strong></p>
                    <ul>
                        <li><code>::before</code>: Chèn nội dung trước nội dung chính của phần tử.</li>
                        <li><code>::after</code>: Chèn nội dung sau nội dung chính của phần tử.</li>
                        <li><code>::first-line</code>: Định dạng dòng đầu tiên của nội dung văn bản.</li>
                    </ul>
                </div>
            </li>
        </ol>

        <!-- Bài 18 -->
        <h1>Bài 18</h1>
        <ol>
            <li><strong>LUYỆN TẬP:</strong> 
                <a href="https://mai1210.github.io/LUY-N-T-P-B-I-18/" target="_blank">Bài LUYỆN TẬP</a>
            </li>
            <li><strong>VẬN DỤNG:</strong> 
                <a href="https://tutranthanh.github.io/foodshopnhom2/" target="_blank">Bài VẬN DỤNG</a>
            </li>
        </ol>
    </div>
</body>
</html>
