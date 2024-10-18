# Odoo Revision
**17/10/2024**

**1.Thành phần của 1 module trong odoo:**

data/

models/

controllers/

views/

static/

wizard/

report/

tests/ 

**2.Các loại Models:**

Models

AbstractModels

TransientModels

**3.Các loại fields:**

Basic fields: Boolen, Char, Float, Integer

Advanced fields: Binary, Html, Image, Monetary, Selection, Text

Date(time) fields

Relational fields: Many2one, One2many, Many2many

Pseudo-relational fields

Computed fields

Related fields

Automatic fields

	- id
 
	- create_date
 
	- create_uid
 
	- write_date
 
	- write_uid

**4.Recordsets**

**5.Method decorators:**

@api.model

@api.constrains

@api.depends

@api.onchange

@api.multi

**6. Common ORM methods**

Create/update

.create(vals_list) -> records

.copy(default=None)

.default_get(fields_list) -> default_values

.name_create(name)

.write(vals)

Search/Read

.browse([ids]) -> records

.search(domain[, offset=0][, limit=None][, order=None][, count=False])

.search_count(domain)

.name_search(name='', args=None, operator='ilike', limit=100) → records

.read([fields])

.read_group(domain, fields, groupby, offset=0, limit=None, orderby=False, lazy=True)

Fields
 
.fields_get([allfields][, attributes])

Unlink
 
.unlink()

Filter
 
.filtered(func)

Map
 
.mapped(func)


Sort
 
.sorted(key=None, reverse=False)

**7.Inheritance**

Cách 1: Classical inheritance

Cách 2: Extension

Cách 3: Delegation

**18/10/2024**

**8. Views**

Tree view: Hiển thị dữ liệu dưới dạng danh sách.

Form view: Hiển thị và chỉnh sửa chi tiết một bản ghi.

Search view: Cho phép tìm kiếm dữ liệu.

Kanban view: Hiển thị dữ liệu theo dạng bảng, có thể kéo thả.

Inheritance: Kế thừa và mở rộng các view có sẵn.

**9. Actions**

Window Actions: Mở các cửa sổ giao diện.

Url Actions: Chuyển hướng tới một URL cụ thể.

Server Actions: Thực hiện các tác vụ phía server.

Report Actions: Thực hiện tạo báo cáo.

Client Actions: Thực hiện hành động phía client.

Automated Actions: Các hành động tự động dựa trên điều kiện.

**10. Menus**

Menu trong Odoo là các mục điều hướng để truy cập vào các phần của ứng dụng/web. Các menu được định nghĩa trong file XML và có thể phân cấp nhiều mức để tổ chức giao diện người dùng.

**11. Security**

Access rights: Xác định các quyền truy cập (create, read, write, unlink) cho từng model.

Record rules: Xác định quy tắc để giới hạn quyền truy cập dữ liệu dựa trên các điều kiện.

Groups: Phân chia người dùng vào các nhóm có quyền hạn khác nhau.

