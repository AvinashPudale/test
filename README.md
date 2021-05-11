## test
### this for test header
---
layout: checklists
title: BOM
description: Bill of Materials for electrical, mechanical and power
checks:
  - title: Online E-commerce
    list:
      - name: RS Components
      - name: Element14
      - name: Mouser
      - name: DigiKey
  - title: Spreadsheet column titles
    list:
      - name: Designator
      - name: Value
      - name: Quantity
      - name: Package
      - name: Category
      - name: Stock
      - name: Manufacturer
      - name: Manufacturer Part No.
      - name: Link to Datasheet
      - name: Vendor name
      - name: Link to Vendor item
      - name: Unit Cost
      - name: "Total Cost <code>( Max(Quantity, Minimum Order) * Unit Cost)</code>"
      - name: Minimum Order Quantity
      - name: Description
---
---
layout: page
title: Checklists
permalink: /checklists
sequence: 1
---

<p class="subtitle">Good checklists to go through!</p>

<nav class="panel">
  {% for checklist in site.checklists %}
  <a class="panel-block searchable" href="{{ checklist.url }}">
    <span class="panel-icon">
      <i class="fas fa-book" aria-hidden="true"></i>
    </span>
    <strong>{{ checklist.title }}</strong> : {{ checklist.description }}
  </a>
  {% endfor %}
</nav>
