# vue-neditor-wrap

## Installation
```bash
$ npm i @ctsy/neditor
```

## Quick Start

1. 入口文件中引入文件

    ```html
    <script src="https://npm.tansuyun.cn/neditor@tsy/neditor.min.js"></script>
    ```

2. 引入`VueNeditorWrap`组件

    `import VueNeditorWrap from '@ctsy/neditor'`

3. 注册组件
    ```js
    components: {
        VueNeditorWrap
    },
    ```
4. `v-model`绑定数据
    ```html
    <vue-neditor-wrap v-model="content" :config="myConfig" :destroy="false" @ready="ready"></vue-neditor-wrap>
    ```
    ```js
    data () {
        return {
            myConfig: {
                // 编辑器不自动被内容撑高
                autoHeightEnabled: false,
                // 初始容器高度
                initialFrameHeight: 240,
                // 初始容器宽度
                initialFrameWidth: '100%',
                // 关闭自动保存
                enableAutoSave: false
            },
            content: '',
        }
    }
    ```
    > 至此你已经可以在页面中看到一个初始化之后的`NEditor`了，并且它已经成功和数据绑定了！

    ![](https://raw.githubusercontent.com/c-tsy/imgs/master/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20181124115713.png)

    ![](https://raw.githubusercontent.com/c-tsy/imgs/master/%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20181124114504.png)

## License

[MIT](http://opensource.org/licenses/MIT)

