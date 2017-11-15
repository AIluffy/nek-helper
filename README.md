# nek-helper 
基于nek-ui的code snippet插件，请使用1.15.0以上的code版本，no deep shit。

## Features

1. html文件内，k开头的前缀，对应nek-ui相应的组件，如k-card对应KLCard组件。**注：** KLModal，KLNotify及KLImagePreview的code snippet放置在js文件中。不支持国际化KLLocaleProvider组件。
2. js文件内，n开头的前缀。目前支持如下code snippet
    
    - n-component: 
    
    ```javascript
    var component = new NEKUI.Component({
        template:template,
        data: {
            
        }
    });
    ```

    - n-modal:

    ```javasript
    var modal = new NEKUI.KLModal({
        data: {
            title: '',
            contentTemplate: ''
        }
    });
    ```

    - n-notify

    ```javascript
    NEKUI.KLNotify.warning('');
    ```

    - n-imgPreview

    ```javascript
    new NEKUI.KLImagePreview({
        data: {
            imageList: [{
                name: '',
                src: ''
            }],
            curIndex: 0
        }
    })
    ```

    - n-menu-data (导航菜单数据)

    ```javascript
    menus: [
        {
            title: '首页',
            key: 'home'
        },
        {
            title: '',
            open: true,
            key: '',
            children: [
                {
                    open: true,
                    title: '',
                    url: '/'
                }
            ]
        }
    ];
    ```

    - n-pager-data (分页数据)

    ```javascript
    current: 1,
    pageSize: 10,
    sumTotal: 100,
    ```

    - n-step-data (步骤数据)

    ```javascript
    current: 0,
    steps: [{
        status: 0,
        title: '',
        description: ''
    }]
    ```