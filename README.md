# cramming-plan
Kế hoạch ôn thi Kì 3 năm 2

## I. Gantt Chart kế hoạch ôn thi (tham khảo)

```mermaid
gantt
    title Kế hoạch ôn thi kì 2 năm 3
    dateFormat  DD/MM
    axisFormat  %d/%m (%a)
    todayMarker stroke-width:2px,stroke:#Crimson,opacity:0.9
    %% tickInterval 1day

    section Lịch học
        %% Tự học :milestone, active, 27/03, 1d
        CSDLPT : done, 19/05, 1d
        CNPM : done, 20/05, 1d
        ATTT : done, 22/05, 1d
        LTW : done, 23/05, 1d
        AI : done, 24/05, 1d

        CSDLPT : done, 26/05, 1d
        Nộp BTL CSDLPT :crit, milestone, 26/05, 1d
        CNPM : done, 27/05, 1d
        ATTT : done, 29/05, 1d
        LTW : done, 30/05, 1d
        AI : done, 31/05, 1d

    section Cấu trúc dữ liệu & Giải thuật
        Ôn lý thuyết (3 thuật toán, quy hoạch động)       :done, ctdl_on, 28/05, 1d
        stack, queue                                      :done, 1d
        đồ thị trọng số, cây nhị phân                     :done, 1d
        Thi thực hành (31/05)                             :crit, milestone, thi_ctdlgt, 31/05, 1d

    section Lập trình web
        NodeJS                                            :done, 24/05, 1d
        ExpressJS                                         :done, 24/05, 30/05
        Code xong bài Sân bóng                            :crit, 26/05, 01/06
        HTML, CSS, JS, DOM                                :active, 02/06, 3d
        ReactJS                                           :active, 02/06, 3d
        Express + MongoDB (Mongoose)                              :active, 03/06, 3d
        Axios, Tailwind, Git (bài thu hoạch đẩy lên git) :active, 02/06, 2d
        Tự code 1 bài CRUD (react, express, sqlite, axios, tailwind) :active, 02/06, 2d
        Code bài LTW - photo upload :active, 02/06, 3d
        Storage, Authentication                     :active, after thi_ttcs, until thi_ltw
        Thi thực hành (07/06)                             :crit,milestone, thi_ltw, 07/06, 1d

    section Thực tập cơ sở
        Code (Lấy từ bài LTW) -> Phân tích & thiết kế (usecase, sequence, class, erd) :done, 25/05, 01/06
        Cài đặt, chạy thử, làm báo cáo (Theo template, có hình ảnh, sơ đồ, bảng biểu) :done, crit, 25/05, 01/06
        Ôn lý thuyết, hiểu bài, cách trình bày                                        :after thi_ctdlgt, until thi_ttcs
        Nộp báo cáo -> nộp muộn, thầy ko nhận                                                :crit,milestone, thi_ttcs, 01/06, 1d
        Demo (04/06)                                                :crit,milestone, thi_ttcs, 04/06, 1d

    section An toàn thông tin
        Ôn tập                                            :attt, after thi_ltw, until thi_attt
        Thi trắc nghiệm (10/06)                           :milestone, thi_attt, 10/06, 1d

    section Nhập môn AI
        Ôn tập                                            :ai, after thi_attt, until thi_ai
        Thi tự luận (13/06)                               :milestone, thi_ai, 13/06, 1d

    section Công nghệ phần mềm
        Tổng hợp lại bài CNPM theo code Sân bóng (tương tự TTCS) -> nộp vớ vẩn                   :crit, btl_cnpm, 26/05, 1d
        Ôn tập (UML usecase, scenario, sequence, class, erd) :cnpm, after thi_ai, until thi_cnpm
        Thi tự luận (18/06)                               :crit,milestone, thi_cnpm, 18/06, 1d

    section CSDL phân tán
        Ôn lý thuyết & Truy vấn                           :after thi_cnpm, until thi_csdl
        Làm và nộp BTL                                    :crit, done, btl_csdl, 21/05, 1d
        Báo cáo & vấn đáp (22/06)                         :crit,milestone, thi_csdl, 22/06, 1d
```

## II. Các chủ đề cần ôn

Học xong: 31/5

Học lại:

- Ctdl & gt -> thi thực hành (31/5)

Phải có code:

- lập trình web -> thi thực hành (7/6)
- csdl phân tán -> báo cáo btl, ko thi, vấn đáp (22/6)
- thực tập cơ sở -> chấm bài (4/6)

Ôn lý thuyết:

- cnpm -> thi tự luận, UML (18/6)
- attt -> trắc nghiệm (10/6)
- nhập môn AI -> tự luận (13/6)

### 1. Cấu trúc dữ liệu và giải thuật (31/5)

Note: tự ôn theo đề cương

3 thuật toán:

- quay lui liệt kê xâu nhị phân
- quay lui liệt kê tổ hợp
- quay lui liệt kê hoán vị

quy hoạch động

stack, queue

đồ thị trọng số, cây nhị phân

### 2. Lập trình web (7/6)

Note: chưa biết chi

HTML, CSS, JS, DOM, ReactJS, ExpressJS

ReactJS:

- ES6, JSX
- component, props, state
- event, lifecycle
- hooks, useState, useEffect
- input validation
- call API
- error handling
- crud with Restful API

Advanced:

- SPA
- Router v6
- nested routes
- dynamic routes
- protect routes

NodeJS:

- Chrome, V8 Engine, NodeJS
- node cli
- node http server

ExpressJS:

- routing
- parameter
- cors
- send data to server
- body parser
- package.json
- example: spotify, simple-blog

Authentication:

- stateful
- stateless

Storage:

- RDS
- ORM
- NoSQL - MongoDB
- example: simple-blog with MongoDB
- mongoose
- CRUD with MongoDB

phân tích yêu cầu bài LTW - photo upload (TH3 + final):
- kiến trúc tổng quan hệ thống và công nghệ sử dụng (FE, BE, DB)
- các thư viện sử dụng trong bài (vd kết nối BE -> DB dùng mongoose, gọi AIP từ FE -> BE dùng axios...)
- liệt kê các nhóm chức năng, và danh sách các chức năng cụ thể (vd nhóm user, gồm list user, get user detail..; nhóm upload, gồm...)
- sequence diagram (viết tóm tắt, ko cần vẽ cũng dc) theo MVC cho 1 vài usecase chính (vd list user, get user detail, cái nào model, cái nào view, cái nào controller...)

### 3. Cơ sở dữ liệu phân tán (22/6)

Note: chưa biết chi

Input:

- Slide tiếng việt
- Sách tham khảo tiếng anh

Biểu điểm:
- Kiểm tra giữa kì (10%) - rồi
- Bài tập nhóm (20%) - tgian nộp
- Thi cuối kì (60%)

Chủ đề:

- Định nghĩa
- Kiến trúc
- Điều khiển (view, materialized view, bảo mật, phân quyền, toàn vẹn dữ liệu, constraint)
- Truy vấn
- Giao dịch

### 4. Công nghệ phần mềm (18/6)

Note: biết sơ sơ, ko sâu

3 pha:

- phân tích
- thiết kế
- kiểm thử

Chủ đề:

- usecase
- scenario
- sequence
- class
- erd

### 5. Thực tập cơ sở (4/6)

Note: chưa làm dc chi

Điểm:

- tiến độ 30% -> phập phù
- báo cáo 40% -> cuối môn nộp
  - nêu vde
  - khảo sát, nghiên cứu, ứng dụng
  - phân tích, thiết kế (usecase, sequence, class, erd)
  - quá trình áp dụng, thực hiện (cài đặt, chạy thử)
  - trình bày khoa học, có đầu mục, hình ảnh, sơ đồ, bảng biểu
- demo 30% -> bảo vệ
  - chức năng, độ khó, workload
  - lưu loát, hiểu bài

### 6. Nhập môn trí tuệ nhân tạo (13/6)

Note: chưa biết chi, tạm bỏ qua, hên xui

Chủ đề:

- khái niệm, lịch sử hình thành phát triển
- giải quyết vấn đề bằng tìm kiếm
  - tìm kiếm mù
  - tìm kiếm có thông tin
  - tìm kiếm cục bộ
- biểu diễn tri thức
  - logic mệnh đề
  - logic vị từ cấp 1
- suy diễn xác suất
  - mạng Bayes
- học máy
  - cây quyết định
  - phân loại bayes đơn giản
  - học trên ví dụ
- AI có thể làm gì

### 7. An toàn thông tin (10/6)

Note: Trắc nghiệm, tạm bỏ qua, hên xui

Chủ đề:

- tổng quan
- tấn công và độc hại
- mã hóa
- kĩ thuật và công cụ attt
- quản lí, chính sách, pháp luật
- buffer overflow


