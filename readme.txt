Cấu trúc thư mục:
    + src: source code
        + main.js => file gốc
        + App.vue => component
        + assets: hình ảnh, font chữ
        + component: chứa các component con

    + component: 
        + 3 thành phần:
            + Template: html => hiển thị html
            + Script: js => xử lý logic
            + Style: css => làm đẹp
                + Hỗ trợ scss
                + scoped style: style dành riêng cho Component
    + Tạo component:
        + Tạo file .vue
        + Import 
        + Khai báo
    + 2 ways binding:
        + Bind dữ liệu 2 chiều: sẽ phụ thuộc vào kiểu của element. vd: input -> string
    + Binding:
        + Value binding: {{ }}
        + property binding:
        + v-bind:<tên thuộc tính>="<biến>"          ==> viết tắt:   :<tên thuộc tính>="<biến>
    + Model: v-model: liên kết element với property
    + Event handling:
        + Bắt sự kiện từ các element
        + v-on:<tên sự kiện>="function()"
            => viết tắt: v-on === @         ---> @click
        + Prevent default event:        @click.prevent=""
            + Hủy bỏ event mặc định của element đi
    + ref: ánh xạ đến element
    + Conditional rendering:
        + v-show: show/hide 1 element theo điều kiện
            + nếu hide thì add style display: none và show thì bỏ display: none
        + v-if: giống v-show nhưng khi hide thì element đó biến mất
        + v-el: 
    + List rendering:
        + v-for
    + methods: hàm của vue object(khai báo function thực hiện hành động nào đó khi lẵng nghe sự kiện của dom)
    + watch: function là biến đc khời tạo trong hàm data() 
        => lắng nghe sự thay đổi của biến đó ==> action...
    + hooks 
        + mounted: chạy đầu tiên khi component đc mount vào dom
    + props: nhận data từ component cha truyền xuống
    + filters: convert data trc khi đc render