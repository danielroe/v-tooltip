# Getting started

v-tooltip is a library helping you add tooltips, dropdowns and other poppers into your Vue application.

[Looking for the old docs?](../legacy/v2/)

## Sponsors

Thank you to my sponsors allowing me to spend more time on Open Source projects! 🙏️

<sponsor-button/>

[![sponsors logos](https://guillaume-chau.info/sponsors.png)](https://guillaume-chau.info/sponsors)

## Quick start

1. Install the package:

<code-group>
<code-block title="npm">
```shell
npm i -S v-tooltip@next
```
</code-block>

<code-block title="yarn">
```shell
yarn add v-tooltip@next
```
</code-block>
</code-group>

2. Add the plugin into your app:

```js
import Vue from 'vue'
import VTooltip from 'v-tooltip'

Vue.use(VTooltip)
```

3. Add the default style:

```js
import 'v-tooltip/dist/v-tooltip.css'
```

[Learn more about installation](./installation.md)

4. Use the `v-tooltip` directive:

```vue
<button v-tooltip="'You have ' + count + ' new messages.'">
```

<TooltipSimpleExample />

[Learn more about the directive](./directive.md)

5. Use the `VDropdown` or `VMenu` component:

```vue
<VDropdown>
  <!-- This will be the popover target (for the events and position) -->
  <button>Click me</button>
  <!-- This will be the content of the popover -->
  <template #popper>
    <MyAwesomeComponent/>
  </template>
</VDropdown>
```

<DropdownSimpleExample />

[Learn more about the component](./component.md)
