- _div_ là một thẻ block,có dạng 100% phần tử chứa nó(chưa nói đến vấn đề khi sd với css)
- _img_ là thẻ inline , thẻ tự đóng, dùng đẻ hiển thị hình ảnh với 2 thuộc tính là 'src'(source) và 'alt' (alternate text)
  alt sử dụng khi link src lỗi thì alt sẽ hiển thị để người dùng biết hình ảnh đó nói về cái gì
  _span_ là thẻ inline nó thường được dùng cho những đoạn chữ ngắn
  _class_ là thuộc tính dùng để sử dụng các class cho thẻ sau đó dùng để style trong css
  Việc đặt tên class khá là nan giải, nên đặt tiếng anh ngắn gọn đễ hiểu
  thẻ tiêu đề : h1 h2 h3 h4 h5 h6
  h1 mỗi trang chỉ có tối đa 1 thẻ h1 thẻ này dùng cho những tiêu đề lớn của trang
  h2 dùng được nhiều thường dùng cho blog to
  h3 dùng dc nhiều thường được dùng cho những blog nhỏ
  h456 tương ứng cho nhwunxg tiêu đề
  thẻ a : là thẻ inline , chắc chắn là dùng cho liên kết nó có 3 thuộc tính hay dùng là href, target , rel
  khi dùng 'target' có giá trị là 'blank' thì thẻ a nên thêm thuộc tính 'rel' bằng 'noopener norefferer'
- font chữ 1 là có sẵn ở google fonts
  2 là ko có sẵn ở gg fonts mà được mua hoặc tải trên mạng về máy
  _font-weight_ : độ đậm nhạt của chữ từ 100 -> 900
  font-family là thiết lập font chữ, truyền vào là font name
- CSS selectors: tag, class, id, attribute

* Tags : h1 h2 h3 div body span a
* Class .name, .tour, .tour-header
  +ID: #header, #content
  special selector : \* : chọn toàn bộ selectors

- Cấu trúc 1 đoạn CSS:
  cssSelectors{
  property: value;  
  }

- user agent stylesheet: Css mặc định của trình duyệt, mỗi trình duyệt sẽ có css mặc định khác nhau
- _css-reset_ dùng để reset css mặc địnhtrình duyệt, và bắt buộc phải có đầu tiên
- _san-serif_: chữ không có chân
- _serif_ : chữ có chân
  - _width_ : độ rộng
  - height chiều cao
  - Border: Viền
- _color_ : màu chữ
- _background-color_: màu nền
  Mã màu: Hexa(#ffa400) , orange, rgb(0,0,0)
  _alpha-opacity_ : 0-> 1

- **\_box sizing**: margin padding border width height, đơn vị px

_content-box_: độ rộng luc này của 1 khối sẽ bằng width + padding(left+right) + border(left +right)
_border-box_: Độ rộng lúc này của 1 khối sẽ bao gồm padding và border, nen áp dụng cho toàn bộ selectors(\*)
_shorthand_ viết rút gọn

- _margin_ : khoảng cách khối này với khối khác không liên quan đến kích thước của cái phần tử đó

- _text-decoration_ gạch dưới của thẻ a, none, underline, line-through
- _border-radius_: độ bo góc của khối, càng lớn thì càng bo góc, nếu hình vuông mà có bo góc lướn thì sẽ tọc ra hfinh tròn còn nếu là hình chữ nhật có bo góc lớn thì sẽ tạo ra hình elipse.

bordeer- top (right-left) radius
........bottom ................

- line-height: khoảng cách giữa các dòng chữ
- Khi những thẻ inline nằm cạnh nhau thì chúng nó sẽ nằm trên 1 hàng, ngược lại những thẻ block thì nó sẽ tạo ra hàng mới
  _display_ : block, inline, inline-block, none, flex, grid
- `block`: biến thành thẻ `block`
- `inline`: biến thành thẻ `inline` , bị hạn chế vài thuộc tính css liên quan đến box-sizing như padding top-bottom, margin top-bottom -`inline-block` : biến thành thẻ `inline-block` : là sự kết hợp giữa inline và block, khi các selectors hoặc thẻ có thuộc tính inline-block thì nó sẽ kế thừa đặc tính của inline, tức là nằm cạnh nhau thì sẽ nằm trên 1 hàng, có độ rộng bằng nội dung mà nó chứa, ko bị hạn chế css
  `flex`
- _padding_ : Không thể dùng số âm
  _margin_ : Có thể dùng số âm, có giá trị `auto`

  _min-width_ : chiều rộng tối thiểu, ví dụ 100px : tối thiểu 100px
  _max-width_ : chiều rộng tối đa, ".............." tối đa 100px;

  _align-items_: stretch (mặc định) làm cho các cột cao bằng nhau
  start căn trên
  end căn dưới
  center: căn giữa
  calc : hàm tính toán , phải có khaorng cách giữa phép tính
  _component_ : mục đíhc là tái sử dụng và có thể tùy chỉnh 1 chỗ để sd nhiều nơi
  _column-gap_ KHOẢNG TRỐNG là chiều dọc
  _row-gap_ KHOẢNG TRỐNG là chiều ngang
  _mixins:_
  _position_: có 5 giá trị chính: relative, absolute, fixed, static, sticky
  _relative_: Khi sử dụng giá trị này thì phải xem xem phần tử con của nó có sử dụng position là `absolute` hay không

  - khi sử dụng thuộc tính position này thì đi kèm sẽ có các thuộc tính khác như top right bottom left và z-index thì nó mới hoạt độg
    _absolute_:
    _responsive_

_opacity_: độ trong suốt

@media screen and (max-width: 'breakpoint - 0.2 px'){}
@media screen and (min-width: 'breakpoint'){}
