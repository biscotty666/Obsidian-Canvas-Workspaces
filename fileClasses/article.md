---
extends: Default
---

title:: {"type":"Input","options":{}}
"Date Published":: {"type":"Date","options":{"dateFormat":"YYYY-MM-DD ddd","defaultInsertAsLink":"false"},"command":{"id":"insert__article__\"Date Published\"","icon":"list-plus","label":"Insert \"Date Published\" field"}}
Published to:: {"type":"Multi","options":{"valuesList":{"1":"SubStack","2":"biscotty.online"},"sourceType":"ValuesListNotePath","valuesListNotePath":"fileClasses.conf/Published To.md","valuesFromDVQuery":""}}
link:: {"type":"Input","options":{}}
Author:: {"type":"File","options":{}}
PubDate:: {"type":"Date","options":{"dateFormat":"YYYY-MM-DD ddd","defaultInsertAsLink":"false"},"command":{"id":"insert__presetField__PubDate","icon":"list-plus","label":"Insert PubDate field"}}
Published:: {"type":"Boolean","options":{},"command":{"id":"insert__presetField__Published","icon":"list-plus","label":"Insert Published field"}}
Cover:: {"type":"Input","options":{"template":""},"command":{"id":"insert__presetField__Cover","icon":"list-plus","label":"Insert Cover field"}}
Stage:: {"type":"Select","options":{"valuesList":{},"sourceType":"ValuesListNotePath","valuesListNotePath":"fileClasses.conf/Stage.md","valuesFromDVQuery":""},"command":{"id":"insert__presetField__Stage","icon":"list-plus","label":"Insert Stage field"}}