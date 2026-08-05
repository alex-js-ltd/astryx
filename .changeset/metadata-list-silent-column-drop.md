---
'@astryxdesign/core': patch
---

[fix] MetadataList: honor a numeric `columns` count when labels default to stacked (`position: 'top'`). Previously a fixed count like `columns={3}` silently fell back to the same responsive auto-fill grid as `columns="multi"` whenever no `label` prop (or an explicit `top` position) was set — the requested column count never reached the DOM. No API change.
@alex-js-ltd
