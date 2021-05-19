<!-- headings -->
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

<!-- Italics -->
_Chữ in nghiêng_

<!-- Bold -->
**Chữ in đậm**

<!--Horizontal rule  -->

---

<!-- Bullet list -->

* apple
* oranges
* pears

<!-- Number List -->

1. Wash
2. rinse
3. repeat

<!-- Link -->
[Sử dụng link](http://example.com)

<!-- Link tham khao -->

* ### **[Link Tham Khao MarkDown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)**

<!-- Images -->

![Image](https://cdn.iconscout.com/icon/premium/png-512-thumb/markdown-6-570527.png)

<!--Blockquotes  -->

>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

[![IMAGE ALT TEXT HERE](https://www.youtube.com/watch?v=HUBNt18RFbo)](https://www.youtube.com/watch?v=HUBNt18RFbo)

[![IMAGE ALT TEXT HERE](https://media-exp1.licdn.com/dms/image/C560BAQHMnA03XDdf3w/company-logo_200_200/0/1519855918965?e=2159024400&v=beta&t=CrP5Le1mWICRcaxIGNBuajHcHGFPuyNA5C8DI339lSk)](https://www.youtube.com/watch?v=HUBNt18RFbo)




## HTML5
---
* ### HTML là gì?
    HTLM là ngôn ngữ đánh dấu siêu văn bản
* ### HTML DOM là gì?
    1. DOM 
    
            Viết tắt của Document Object Model
            Gồm 3 thành phần: 
            - Element
            - Attribute
            - Text
    
    2. Mô hình DOM HTML

         ![Mô Hình DOM HTML](https://www.w3schools.com/js/pic_htmltree.gif)


* ### Xử lý Text
    * Heading
        1. Heading 1-6
        ```html
        <h1>Heading 1</h1>   
        <h2>Heading 2</h2>   
        <h3>Heading 3</h3>   
        <h4>Heading 4</h4>   
        <h5>Heading 5</h5>   
        <h6>Heading 6</h6>   
        ```
        2. Paragraphs
        ```html 
        <p>Paragraph</p>
        <pre></pre>                  -hiển thị mặt định text
        <hr>                         -gạch ngang
        <br>                         -xuống dòng
        <strong></strong> <b></b>    -in đậm
        <i></i>                      -in nghiêng
        ```
        3. Link

        ```html
        <a href="link" target="#"></a>   
        - Tag a có 2 Attibute thường dùng là:  
        + href cho biết điểm đến của liên kết
        + target có 4 loại: 
            _self  : Mở tài liệu trong cùng 1 cửa sổ khi click vào
            _blank : Mở tài liệu trong một cửa sổ mới.
            _parent: Mở tài liệu trong khung cha chứa nó
            _top   : Mở tài liệu trong khung chính
        ```
        

* ### Element Thường Sử Dụng
    1. Img
        ```html
            <img src="#" alt="#"></img>
            -Thẻ Img có 2 Attribute thường dùng là:
                + src: Đường dẫn ảnh
                + alt: Chỉ định một văn bản thay thế khi hình ảnh bị lỗi
    2. Picture
        ```html
            <picture>
                <source media="(min-width: 650px)" srcset="img_food.jpg">
                <source media="(min-width: 465px)" srcset="img_car.jpg">
                <img src="img_girl.jpg">
            </picture>

            -media: xác định khung hình hiển thị ảnh
            -srcset: đường dẫn ảnh
    3. Table
        ```html
        <table>
            <caption></caption>
            <tr>
                <th></th>
            </tr>
            <tr>
                <td></td>
            </tr>
        </table>
        - caption: Là Tag chú thích của bảng luôn nằm đầu trong Tag Table
        - tr : Là tag xác định một hàng trong bảng
        - th : Tiêu đề của bảng
        - td : Là tag xác định dữ liệu của bảng
    4. List
        ```html
        <ul>
            <li><li>
        </ul>
        -Một list luôn nằm trong 1 Tag ul hoặc ol
            + ul: mặc định các mục trong danh sách sẽ được đánh dấu bằng một vòng tròn màu đen nhỏ
            + ol: mặc định các mục trong danh sách sẽ được đánh dấu bằng số thứ tự bắt đầu từ 1. 
        -Mỗi mục bắt đầu với 1 Tag li
    5. Block và Inline
        - Block: là các thẻ có kiểu display: block luôn được xuống dòng và chiếm toàn bộ width nếu width không được set ví dụ như thẻ div, p, section, ul, nav..
        - Inline: là các thẻ có kiểu display: inline sẽ nằm trên cùng một dòng nếu các item vượt quá độ dài của dòng thì item sẽ xuống dòng mới. Các item có kiểu display này không thể set được width và height. Có thể điều chỉnh được padding và margin left and right còn bottom và top thì không ví dụ như các thẻ span, i, a, b, img, input, lable..
        - [Tham Khảo Thêm](https://www.w3schools.com/html/html_blocks.asp)
    6. Layout Element
        ```html 
        <header>    - Xác định phần đầu của một trang web
        <nav>       - Xác định tập hợp các liên kết
        <section>   - Xác đinh một phần trong tài liệu
        <article>   - Xác định nội dung độc lập
        <aside>     - Xác định nội dung bên cạnh nội dung
        <footer>    - Xác định chân trang cho một tài liệu hoặc một phần
        <details>   - Xác định các chi tiết bổ sung mà người dùng có thể mở và đóng theo yêu cầu
        <summary>   - Xác định đề tài cho details phần tử
        <div>       - được sử dụng để tạo ra một khu vực kiểu block nào đó trên một website, hay bạn có thể hiểu là gom nhóm tập hợp các phần tử trên website vào một khu vực.
    7. Thẻ meta
        - Được sử dụng để cung cấp metadata về tài liệu HTML.
        - Được sử dụng để định nghĩa các thông tin cơ bản như mô tả trang web, từ khóa, tác giả.
        ```html
            <meta name="#" content="" charset="" http-equiv="">
                - Name: Cung cấp tên HTML cho một thông tin có trong thuộc tính content
                - Content: Xác định nội dung cho thông tin dữ liệu
                - Charset: Mã hóa ký tự- Xác định bộ mã ký tự cho văn bản HTML
                - http-quiv : Cung cấp tiêu đề HTML cho một thông tin có trong thuộc tính content
        ```
    
* ### Attribute 
    1. Class 
        - Sử dụng được trên nhiều element HTML 
        - Phân biệt chữ hoa chữ thường
        - Những cách đặt tên Class phổ biến:
            + BEM: Block Element Modifier 
                + Block: Là thành phần của trang web hay ứng dụng đó.
                + Element: Là một thành phần bên trong block, phụ thuộc vào parent block của nó.
                + Modifier: Được dùng để thay đổi cách hiển thị block hoặc phần tử 
                + Cú pháp: 
                .block{} .block__element{} .block--modifier{}
        - [Link Tham Khảo](https://topdev.vn/blog/bem-la-gi/#_tai-sao-lai-phai-su-dung-bem-1)    
    2. ID
        - Được sử dụng để chỉ định một id duy nhất cho một phần tử HTML
        - ID là duy nhất.
        - Phân biệt chữ hoa chữ thường.
        - JS có thể truy cập một phần tử có id cụ thể bằng method getElementById()     
    3. Title
        - Xác định thông tin thêm về một phần tử
        - Khi rê chuột lên phần tử có thuộc tính title thì nó sẽ hiển thị dưới dạng văn bản
        - Nó có thể sử dụng ở bất kỳ trên phần tử HTML.  
    4. Viewport
         ```html
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            - initial-scale=1.0 : Độ phóng to ban đầu
            - device-width      : Chiều rộng bằng chiều rộng của thiết bị.
        ```
        - Giải quyết vấn đề nội dung không hiển thị như ý muốn cụ thể là nội dung bị phóng to hoặc thu nhỏ với tỷ lệ khác đi.
        - [Tham khảo thêm](https://hocwebchuan.com/tutorial/responsive/responsive_viewport.php)
* ### Form Attribute
    1. optgroup
        - Dùng để nhóm các tùy chọn có liên quan trong một phần tử select
        ```html
                <optgroup label="German Cars">
                    <option value="mercedes">Mercedes</option>
                    <option value="audi">Audi</option>
                </optgroup>
        ```

    2. datalist
        - Một danh sách dữ liệu với tùy chọn được xác định trước 
        - list tham chiếu đến phần tử `<datalist>` chứa các tùy chọn được xác định trước cho phần tử `<input>`
        ```html
        <input list="browsers" name="browser" id="browser">
        <datalist id="browsers">
            <option value="Edge">
            <option value="Firefox">
            <option value="Chrome">
            <option value="Opera">
            <option value="Safari">
        </datalist>
        <input type="submit">
    3. output
        - Thực hiện một phép tính và hiển thị kết quả trong phần tử `<output></output>`
        ```html
            <form oninput="x.value=parseInt(a.value)+parseInt(b.value)">
                <input type="range" id="a" value="50">
                +<input type="number" id="b" value="25">
                =<output name="x" for="a b"></output>
            </form>
        ```
        - oninput : thực thi JS
    4. action
        - Xác định hành động sẽ được thực hiện khi biểu mẫu được gửi.
        ```html
        <form action="index.html"> </form>
        ```
    5. target
        - Chỉ định nơi hiển thị phản hồi nhận được sau khi gửi biểu mẫu.
        - Các giá trị của target:
        - \_blank: Khi submit hay nhấn vào link nó sẽ chuyển link đó sang tab mới của trình duyệt.
        - \_top: Tương tự \_blank nhưng nó mở link ngay tab hiện tại
        - \_self: Tương tự \_blank nhưng nó mở link ngay tab hiện tại ở khung chứa nó
        - \_parent: Tương tự như \_self nhưng nó mở link ở phần cha chứa nó
        - framename: Trang được liên kết sẽ mở ra trong khung được đặt tên

        ```html
        <form action="index.html" target="_blank"></form>
        ```
    6. method
        - Chỉ định phương thức HTTP sẽ được sử dụng khi gửi dữ liệu biểu mẫu.
        - các giá trị của method: get và post
        - get: các thông tin trong form sẽ mô tả bởi URL và nhìn vào thanh địa chỉ trình duyệt sẽ thấy thông tin. Nên những dữ liệu nhạy cảm sẽ không sử dụng nó, độ dài của URL bị giới hạn (2048 ký tự)
        - post: Sẽ không nhìn thấy dữ liệu biểu diễn qua URL như thế này mà dữ liệu sẽ được ẩn.

        ```html
        <form action="index.html" method="get" target="_blank"></form>
        ```
    7. autocomplete
        - Khi bật tính năng tự động hoàn thành, trình duyệt sẽ tự động hoàn thành các giá trị dựa trên các giá trị mà người dùng đã nhập trước đó.

        - Có 2 giá trị là on và off

        ```html
        <form action="index.html" method="get" autocomplete></form>
        ```
    8. novalidate
        - Khi bật tính năng novalidate thì khi submit dữ liệu sẽ không được validate

        ```html
        <form action="index.html" method="get" novalidate></form>
        ```
    9. name
        - Chỉ định tên của một biểu mẫu.
        - Sử dụng để tham chiếu các phần tử trong JavaScript hoặc để tham chiếu dữ liệu biểu mẫu sau khi biểu mẫu được gửi.
        ```html
        <form action="index.html" method="get" name="form1"></form>
        ```
    10. enctype
        - Chỉ dùng cho method post
        - Chỉ định cách dữ liệu biểu mẫu được mã hóa khi gửi đến máy chủ.
        - Có 3 giá trị:

        - text/plain: gửi dữ liệu nhưng không được mã hóa
        - multipart/form-data: giá trị này là cần thiết nếu tải tệp lên thông qua form
        - application/x-www-form-urlencoded: đây là giá trị mặc định, tất cả các ký tự đều được mã hóa (dấu space sẽ được mã hóa thành dấu +) và các ký tự đặc biệt được chuyển đổi thành giá trị ASCII HEX.
* ### Form element
     1. input Attributes
         
         a. accept
        
        - Thuộc tính `accept` chỉ có thể được sử dụng với `<input type = "file">`.
        - Chỉ định những loại tệp mà người dùng có thể chọn từ hộp thoại nhập tệp.
        - các value như: `audio/*` , `video/*` , `image/*`, `file_extension` (gif, .jpg, doc,...),

        ```html
        <form action="#" id="form1">
        <input type="file" id="img" name="img" accept="image/*" />
        </form>
        ```

        b. autocomplete

        - Tương tự như của form

        ```html
        <form action="#" id="form1">
        <input type="text" autocomplete />
        </form>
        ```

        c. autofocus

        - Chỉ định một element `<input>` sẽ tự động focus khi tải trang

        ```html
        <form action="#" id="form1">
        <input type="text" autofocus />
        </form>
        ```

        d. checked

        - Chỉ định rằng một element `<input>` nên được chọn trước khi tải trang
        - Nó có thể được sử dụng với `<input type = "checkbox">` và `<input type = "radio">` .

        ```html
        <form action="/action_page.php">
        <input type="checkbox" checked />
        <input type="submit" value="Submit" />
        </form>
        ```

        f. disabled

        - Vô hiệu hóa thẻ `input` đó

        ```html
        <form action="#" id="form1">
        <input type="text" disabled />
        </form>
        ```

         g. form

        - Chỉ định `form` mà phần tử `<input>` thuộc về thông qua `id` của `form` đó.

        ```html
        <form action="#" id="form1"><input type="text" " /></form>
        <input type="text" form="form1" />
        ```

         h. max - min

        - Chỉ định giá trị lớn nhất và nhỏ nhất cho phần tử `<input>`
        - Chỉ sử dụng với các type: number, range, date, datetime-local, month, time and week.

        ```html
        <form action="/action_page.php">
        <label for="quantity">Quantity (between 1 and 5):</label>
        <input type="number" min="1" max="5" /><br />
        <input type="submit" />
        </form>
        ```

         i. maxlength - minlength

        - chỉ định số ký tự tối đa và tối thiểu được phép trong phần tử `<input>`.

        ```html
        <form action="/action_page.php">
        <label for="username">Username:</label>
        <input type="text" minlength="1" maxlength="10" /><br />
        <input type="submit" value="Submit" />
        </form>
        ```

         j. multiple

        - Hoạt động với các loại đầu vào sau: email và tệp
        - Chỉ định rằng người dùng được phép nhập nhiều hơn một giá trị vào phần tử `<input>`.

        ```html
        <form action="/action_page.php">
        <label for="files">Select files:</label>
        <input type="file" id="files" name="files" multiple />
        <input type="submit" />
        </form>
        ```

        k. pattern

        - Chỉ định một biểu thức chính quy mà giá trị của phần tử `<input>` được kiểm tra khi gửi biểu mẫu.
        - Chỉ hoạt động với: văn bản, ngày tháng, tìm kiếm, url, số điện thoại, email và mật khẩu.

        ```html
        <form action="/action_page.php">
        <label for="country_code">Country code:</label>
        <input type="text" pattern="[A-Za-z]{3}" />
        <input type="submit" />
        </form>
        ```

        l. readonly

        - Chỉ để đọc không thể sửa đổi trường đầu vào chỉ đọc (tuy nhiên, người dùng có thể gắn thẻ, đánh dấu và sao chép văn bản từ trường đó)

        ```html
        <form action="/action_page.php">
        <input type="text" value="abc" readonly />
        <input type="submit" />
        </form>
        ```

        m. type

        - Dùng để chỉ định loại phần tử `<input>` để hiển thị
        - Các giá trị của type
        - button
        - checkbox
        - color
        - date
        - datetime-local
        - email
        - file
        - hidden
        - image
        - month
        - number
        - password
        - radio
        - range
        - reset
        - search
        - submit
        - tel
        - text
        - time
        - url
        - week

        ```html
        <input type="url" />
        ```

        n. value

        - Chỉ định giá trị của phần tử `<input>`

        ```html
        <form action="/action_page.php">
        <input type="text" value="country" />
        </form>
        ```

    2. lable element

        - Dùng làm nhãn cho các element của form
        - Attribute `for`: phải bằng thuộc tính id của element `<input>` để liên kết chúng với nhau

        ```html
        <form action="/action_page.php">
        <label for="country_code">Country code:</label>
        <input type="text" id="country_code" />
        <input type="submit" />
        </form>
        ```

    3. select element

        - Danh sách thả xuống
        - Chứa các `<option>` element
        - Attribute `size` chỉ định số lượng giá trị hiển thị

        - Attribute `multiple` cho phép chọn nhiều `option`

        ```html
        <label for="cars">Choose a car:</label>
        <select id="cars" name="cars" size="3" multiple>
        <option value="volvo">Volvo</option>
        <option value="saab">Saab</option>
        <option value="fiat">Fiat</option>
        <option value="audi">Audi</option>
        </select>
        ```

    4. option element

        - Xác định một tùy chọn có thể được chọn
        - Mặc định, mục đầu tiên trong danh sách thả xuống được chọn.
        - Để xác định một tùy chọn đã chọn trước, thêm attribure `selected` vào `<option>`
        - attribute `value` nội dung của `value` sẽ được gửi khi submit `form`, nếu `value` trống thì nội dung của `<option>nội dung</option>` sẽ thay thế

    5. textarea element

        - Xác định trường nhập nhiều dòng
        - có 2 attribute là `rows` và `cols` để xác định chiều ngang chiều dọc
        - có thể sử dụng css `width` và `height` để xác định chiều ngang chiều dọc

        ```html
        <form action="#" multiple>
        <textarea cols="30" rows="10"></textarea>
        </form>
        ```

    6. fieldset element

        - Được sử dụng để nhóm các element trong một `form`.
        - Thẻ `legend` dùng làm caption của fieldset
        - Attribute `form` dùng để xác định `form` của các field trong `fieldset` thuộc về
        - Attribute `disabled` dùng để vô hiệu hóa các element trong fieldset

        ```html
        <fieldset>
        <legend>Personalia:</legend>
        <label for="fname">First name:</label>
        <input type="text" id="fname" name="fname" />
        </fieldset>
        ```
        
        <img src="https://developers.google.com/web/fundamentals/performance/critical-rendering-path/images/render-tree-construction.png" width=400 >
