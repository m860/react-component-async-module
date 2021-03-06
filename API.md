<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [AsyncComponent](#asynccomponent)
    -   [propTypes](#proptypes)

## AsyncComponent

[src/components/AsyncComponent.js:21-88](https://github.com/m860/react-async-component/blob/2777387cabdb53aa8c4b3625479694a6d3ff3e8a/src/components/AsyncComponent.js#L21-L88 "Source code on GitHub")

**Extends Component**

异步组件

**Parameters**

-   `props`  

**Examples**

```javascript
import AsyncComponent from 'react-async-component'

<AsyncComponent
    components={[
        System.import('./A.js')
    ]}>
    {ModuleA=>{
        return <ModuleA/>
    }}
</AsyncComponent>
```

### propTypes

[src/components/AsyncComponent.js:30-35](https://github.com/m860/react-async-component/blob/2777387cabdb53aa8c4b3625479694a6d3ff3e8a/src/components/AsyncComponent.js#L30-L35 "Source code on GitHub")

propTypes

**Properties**

-   `components` **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)** components,使用`System.import`(webpack 4建议使用`import`的方式引用,需要使用babel插件`babel-plugin-syntax-dynamic-import`)进行引用,也可以使用同步的方式引用,如:require('xxx').default
-   `children` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)** 异步回调
-   `renderLoading` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)?** 
-   `renderError` **[Function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/function)?** renderError包含一个参数
