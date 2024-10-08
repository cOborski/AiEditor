#  Font size configuration


## Samples

```typescript
new AiEditor({
    element: "#aiEditor",
    fontSize:{
        values:[
            {name: "初号", value: 56},
            {name: "小初", value: 48},
            {name: "一号", value: 34.7},
            {name: "小一", value: 32},
            {name: "二号", value: 29.3},
            {name: "小二", value: 24},
            {name: "三号", value: 21.3},
            {name: "小三", value: 20},
            {name: "四号", value: 18.7},
            {name: "小四", value: 16},
            {name: "五号", value: 14},
            {name: "小五", value: 12},
        ]
    },
})
```
In the above code, "name" represents the font size name, and "value" represents the font size in pixels (px).


## Set the default font size

In AIEditor, the default font size is 14px. If you want to change the default font size, you need to add the following configuration:

```ts 5
new AiEditor({
    element: "#aiEditor",
    fontSize: {
        defaultValue: 18
    },
})
```

At the same time, you need to modify the class style of `aie-content`. The code is as follows:

```css
.aie-content {
    font-size: 18px;
}
```