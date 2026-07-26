# Features Added

- Simplified index management
- Modified the OOTB `cqPageContent` index to work with full-text queries

```text
path=/content/wknd/us/en
type=cq:PageContent
fulltext=*Meet our extraordinary travel guides*
p.limit=-1
p.hits=full
p.indexTag=cqPageContentModified
```
The index tag is added to force the system to pick cqPageContent index, 
else it would pick up pathRefrence index as that is less costly and expected results will not be shown.