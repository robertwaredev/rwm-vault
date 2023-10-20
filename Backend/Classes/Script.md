---
excludes: 
extends: 
icon: pencil
limit: 100
mapWithTag: true
tagNames: 
version: 7
---

Status:: {"type":"Select","options":{"valuesList":{"1":"Idea","2":"Draft","3":"Final","4":"Reviewed","5":"Published"},"sourceType":"ValuesList","valuesListNotePath":"","valuesFromDVQuery":""},"command":{"id":"insert__presetField__Status","icon":"list-plus","label":"Insert Status field"}}
Topic:: {"type":"MultiFile","options":{"dvQueryString":"dv.pages('\"Atlas/Maps\"').file.link","customRendering":"","customSorting":"a.basename > b.basename ? 1; -1"},"command":{"id":"insert__Script__Topic","icon":"list-plus","label":"Insert Topic field"}}
Pinned:: {"type":"Boolean","options":{},"command":{"id":"insert__presetField__Pinned","icon":"pin","label":"Insert Pinned field"}}
Type:: {"type":"Select","options":{"valuesList":{"1":"Long Form","2":"Short Form"},"sourceType":"ValuesList","valuesListNotePath":"","valuesFromDVQuery":""}}