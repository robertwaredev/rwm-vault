---
excludes: 
extends: 
icon: pencil
limit: 100
mapWithTag: true
tagNames: 
version: 7
---

status:: {"type":"Select","options":{"valuesList":{"1":"Idea","2":"Draft","3":"Final","4":"Reviewed","5":"Published"},"sourceType":"ValuesList","valuesListNotePath":"","valuesFromDVQuery":""},"command":{"id":"insert__Script__status","icon":"list-plus","label":"Insert status field"}}
topic:: {"type":"MultiFile","options":{"dvQueryString":"dv.pages('\"Atlas/Maps\"').file.link","customRendering":"","customSorting":"a.basename > b.basename ? 1; -1"},"command":{"id":"insert__Script__topic","icon":"list-plus","label":"Insert topic field"}}
pinned:: {"type":"Boolean","options":{},"command":{"id":"insert__Script__pinned","icon":"pin","label":"Insert pinned field"}}
type:: {"type":"Select","options":{"valuesList":{"1":"Long Form","2":"Short Form"},"sourceType":"ValuesList","valuesListNotePath":"","valuesFromDVQuery":""}}