# link_graph

## 使用D3js创建

[点击查看Demo](https://honghurumeng.github.io/)

![demo](./image/截屏2024-05-30%2011.43.56.png)

## 配置json

``` javascript

const data = {
            //id    name    showName    color    radiusRatio    fontSizeRatio    fontColor    icon    link    hasMask    tooltip    transparent    copy
            "nodes": [
                { "id": "1", "name": "github", "showName": false, "color": "#FF5733", "radiusRatio": 0.13, "fontSizeRatio": 0.015, "fontColor": "white", "icon": "https://avatars.githubusercontent.com/u/60283556?v=4", "link": "https://github.com/Honghurumeng", "hasMask": true, "tooltip": "Github", "transparent": true },
                { "id": "2", "name": "gmail", "showName": false, "color": "#33FF57", "radiusRatio": 0.07, "fontSizeRatio": 0.012, "fontColor": "white", "hasMask": false, "tooltip": "点击复制：honghurumeng@gamil.com", "icon": 'https://ssl.gstatic.com/ui/v1/icons/mail/rfr/logo_gmail_lockup_default_2x_r5.png', "transparent": true, "copy": 'honghurumeng@gamil.com' },
                { "id": "7", "name": "qqmail", "showName": false, "color": "#33FF57", "radiusRatio": 0.05, "fontSizeRatio": 0.012, "fontColor": "white", "hasMask": false, "tooltip": "点击复制：710297266@qq.com", "icon": qqmail, "transparent": true, "copy": '710297266@qq.com' },
                { "id": "3", "name": "mtoast", "showName": false, "color": "#3357FF", "radiusRatio": 0.04, "fontSizeRatio": 0.02, "fontColor": "white", "hasMask": false, "tooltip": "单JS文件的原生toast", "link": 'https://honghurumeng.github.io/mtoast-demo', "icon": toast, "transparent": true },
                { "id": "4", "name": "五子棋", "showName": false, "color": "#000000", "radiusRatio": 0.04, "fontSizeRatio": 0.02, "fontColor": "white", "hasMask": false, "transparent": true, "icon": gobang, "tooltip": "五子棋游戏" },
                { "id": "5", "name": "双人", "showName": false, "color": "#000000", "radiusRatio": 0.02, "fontSizeRatio": 0.02, "fontColor": "white", "hasMask": false, "transparent": true, "link": 'https://honghurumeng.github.io/Gobang-VS-Human', "icon": p2, "tooltip": "开始双人对战" },
                { "id": "6", "name": "人机", "showName": false, "color": "#000000", "radiusRatio": 0.02, "fontSizeRatio": 0.02, "fontColor": "white", "hasMask": false, "transparent": true, "link": 'https://honghurumeng.github.io/Gobang-VS-AI', "icon": ai, "tooltip": "与电脑开始游戏" },
                { "id": "8", "name": "ppt", "showName": false, "color": "#000000", "radiusRatio": 0.04, "fontSizeRatio": 0.02, "fontColor": "white", "hasMask": false, "transparent": true, "link": 'https://github.com/Honghurumeng/pptx_builder', "icon": pptx, "tooltip": "通过xlsx及pptx模板批量生成文件" },
                { "id": "9", "name": "mail", "showName": false, "color": "#000000", "radiusRatio": 0.04, "fontSizeRatio": 0.02, "fontColor": "white", "hasMask": false, "transparent": true, "icon": mail, },
            ],
            //source    target    distanceRatio    color    strokeWidth    lineType    relativeDirection
            "links": [
                { "source": "1", "target": "9", "distanceRatio": 0.1, "color": "#FDBA5699", "strokeWidth": 2, "lineType": "curve", "relativeDirection": { "dx": 0, "dy": -1 }, },
                { "source": "1", "target": "3", "distanceRatio": 0.1, "color": "#FDBA5699", "strokeWidth": 2, "lineType": "curve" },
                { "source": "9", "target": "7", "distanceRatio": 0.05, "color": "#8298FF99", "strokeWidth": 1, "lineType": "curve" },
                { "source": "9", "target": "2", "distanceRatio": 0.05, "color": "#8298FF99", "strokeWidth": 1, "lineType": "curve" },
                { "source": "1", "target": "8", "distanceRatio": 0.1, "color": "#FDBA5699", "strokeWidth": 2, "lineType": "curve" },
                { "source": "1", "target": "4", "distanceRatio": 0.2, "color": "#FDBA5699", "strokeWidth": 2, "lineType": "curve", "relativeDirection": { "dx": -1, "dy": 0 }, },
                { "source": "4", "target": "5", "distanceRatio": 0.05, "color": "#8298FF99", "strokeWidth": 1, "lineType": "curve" },
                { "source": "4", "target": "6", "distanceRatio": 0.05, "color": "#8298FF99", "strokeWidth": 1, "lineType": "curve" },
            ]
        };

```