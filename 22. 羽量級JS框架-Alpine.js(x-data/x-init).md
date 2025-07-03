### 紀錄內容：

x-data用於宣告新組建的作用域，類似於 Vue 組件的 `data`

**範例:** `<div x-data="{ foo: 'bar' }">...</div>`

還可以將資料（與行為）擷取到可重用的函數中：

```jsx
<div x-data="dropdown()">
    <button x-on:click="open">Open</button>

    <div x-show="isOpen()" x-on:click.away="close">
        // Dropdown
    </div>
</div>

<script>
    function dropdown() {
        return {
            show: false,
            open() { this.show = true },
            close() { this.show = false },
            isOpen() { return this.show === true },
        }
    }
</script>
```

初始化:
**範例:** `<div x-data="{ foo: 'bar' }" x-init="foo = 'baz'"></div>`