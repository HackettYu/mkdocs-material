# [hackettyu'snippets] Javascript 获取 UUID

- 生成 uuid

```javascript
const UUIDGenerator = () =>
([1e7] + -1e3 + -4e3 + -8e3 + -1e11).replace(/[018]/g, c =>
(c ^ crypto.getRandomValues(new Uint8Array(1))[0] & 15 >> c / 4).toString(16)
);
// UUIDGenerator() -> '7982fcfe-5721-4632-bede-6000885be57d'
```