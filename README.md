# Odoo Revision
17/10/2024

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
