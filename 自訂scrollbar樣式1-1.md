---
title: 1. 自訂scrollbar樣式1-1

---

1. 在固定畫面的內容物過多或是內容過長時,我們會使用overflow: scroll;強制出現可滑動的長條來操作可視內容
2. 會有些狀況明明出現可拖拉的動作但卻不見scrollbar,這時我們可以找到該區塊的外層對scrollbar座改良使其可視

例如:
```CSS=
/* width */
::-webkit-scrollbar {
  width: 50px;
}

/* Track */
::-webkit-scrollbar-track {
  box-shadow: inset 0 0 5px grey;
  border-radius: 10px;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: rgba(0,0,0, 0.2);
  border-radius: 10px;
}

```固定畫面的內容物過多或是內容過長時,我們會使用overflow: scroll;強制出現可滑動的長條來操作可視內容
2. 會有些狀況明明出現可拖拉的動作但卻不見scrollbar,這時我們可以找到該區塊的外層對scrollbar座改良使其可視

例如:
```

```