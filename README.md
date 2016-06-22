LotteryCard
=======
H5刮奖,

need support canvas

##使用说明

var card = new CardCover(
        {
            id: 'cardContainer',
            coverImg: 'images/cover.png',
            width:300,
            height:144,
            percentClear:80,
            drawPercentCallback: drawPercent
        }
);
card.init();

function drawPercent(percent) {
    drawPercentNode.innerHTML = percent + '%';
}

##构造方法参数解释

`id`:刮奖容器,必须

`coverImg`:涂层内容

`width`:刮奖区域宽度,默认为300px,可空

`height`:刮奖区域高度,默认为100px,可空

`percentClear`:刮开的区域百分比 达到多少清空涂层,默认100,可空

`drawPercentCallback`:刮开的区域百分比回调函数,可空


