# u-loading
> A vue loading plug-in

## Install
```
npm i u-loading --save
```
## Import
```
//  Introduced in main.js

import  uLoading  from  'u-loading'
Vue.use(uLoading);
```
## Use
```
<uLoading></uLoading>
```
## Attributes
<table width="100%">
    <tr>
        <th>parameter</th>
        <th>explain</th>
        <th>type</th>
        <th>optional</th>
        <th>default</th>
    </tr>
    <tr>
        <td>type</td>
        <td>Animation</td>
        <td>Number</td>
        <td>1~93</td>
        <td>1</td>
    </tr>
    <tr>
        <td>zIndex</td>
        <td>z-index</td>
        <td>Number</td>
        <td>--</td>
        <td>1000</td>
    </tr>
    <tr>
        <td>fixed</td>
        <td>full screen</td>
        <td>Boolean</td>
        <td>true / false</td>
        <td>true</td>
    </tr>
    <tr>
        <td>bgColor</td>
        <td>Mask layer color</td>
        <td>String</td>
        <td>--</td>
        <td>#263238</td>
    </tr>
    <tr>
        <td>radius</td>
        <td>Mask layer fillet</td>
        <td>String</td>
        <td>--</td>
        <td>0px</td>
    </tr>
    <tr>
        <td>bottom</td>
        <td>bottom side</td>
        <td>Boolean</td>
        <td>true / false</td>
        <td>false</td>
    </tr>
</table>