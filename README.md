# odoo_revision
17/10/2024
1.Thành phần của 1 module trong odoo:

data/
models/
controllers/
views/
static/

wizard/
report/
tests/ 

2.Các loại Models:

Models

AbstractModels

TransientModels

3.Các loại fields:

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

4.Recordsets

5.Method decorators:

@api.model

@api.constrains

@api.depends

@api.onchange

@api.multi

