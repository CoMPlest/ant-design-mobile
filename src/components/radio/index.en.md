# Radio

<code src="./demos/index.tsx"></code>

## API

```ts | pure
type RadioValue = string | number
```

### Radio

| Name           | Description                                                           | Type                                    | Default |
| -------------- | --------------------------------------------------------------------- | --------------------------------------- | ------- |
| checked        | To specify whether it is currently selected                           | `boolean`                               | `false` |
| defaultChecked | To specify whether it is currently selected by default                | `boolean`                               | `false` |
| disabled       | Diabled state                                                         | `boolean`                               | `false` |
| onChange       | Callback function when checked is changed                             | `(val: boolean) => void`                | -       |
| value          | Value is carrying identification, used in `Group` mode                | `RadioValue`                            | -       |
| block          | Whether to render as a block-level element                            | `boolean`                               | `false` |
| id             | The id of the input element, often used in conjunction with the label | `string`                                | -       |
| icon           | Customized `icon` icon                                                | `(checked: boolean) => React.ReactNode` | -       |

### Radio.Group

| Name         | Description                                 | Type                          | Default |
| ------------ | ------------------------------------------- | ----------------------------- | ------- |
| defaultValue | Option selected by default                  | `RadioValue`                  | -       |
| disabled     | Disabled for the whole group                | `boolean`                     | `false` |
| value        | Specified selected option                   | `RadioValue`                  | -       |
| onChange     | Callback function when the value is changed | `(value: RadioValue) => void` | -       |