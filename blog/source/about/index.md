---
title: 了解更多
cover_image: /images/dzc-txt.png
---

---

# 殿镇村


殿镇村原名殿紫头，得名于唐贞观6年（公元632年），位于终南山下，是个古老而又充满勃勃生机的千年古村，因村南建有元始台（又名玉清宫殿），村西有西周时老子骑青牛出函谷关后著书《道德经》的所在地楼观台（紫气东来），合称殿紫头，在解放之前殿紫头是通往陕南的驿馆要道，因殿紫头为山货、木材和药材集中交易的集镇而闻名关中，故名殿镇，上世纪80年代殿镇村移民聚居，素有九省十八县之称，2023年殿镇村在创建“周至县和美乡村建设”中取得第一名的优异成绩并且村集体经济突破50万元名列全镇前茅。

### 下图为殿镇村村口

![村口](/images/cunkou.jpg)

# 地理位置

<div id="amap-about"></div>
<style type="text/css">
    #amap-about {
        width: 100%;
        height: 600px;
        border-radius: 10px;
        box-shadow: 0 12px 24px rgba(0, 0, 0, 0.3);
    }
    .custom-content-marker {
        position: relative;
        width: 25px;
        height: 34px;
    }
    .custom-content-marker img {
        width 100%;
        height: 100%;
    }
</style>

</style>
<script type="text/javascript">
    window._AMapSecurityConfig = {
        securityJsCode: "889aaea037bb5774e13dc396b367489e",
    };
</script>
<script src="https://webapi.amap.com/loader.js"></script>
<script type="text/javascript">
    AMapLoader.load({
        key: "420df2b9a87474b7aa4e0ecb0016f672",
        version: "2.0",
    })
    .then((AMap) => {
        const map = new AMap.Map("amap-about", {
            zoom: 10,
            center: [108.677873,34.171358],
            viewMode: '2D',
            mapStyle: "amap://styles/fresh"
        });
        //异步加载控件
        AMap.plugin('AMap.HawkEye',function(){ 
            var hwakEye = new AMap.HawkEye({
                width: '200px',
                height: '200px',
            });
            map.addControl(hwakEye); //添加控件
        });
        AMap.plugin('AMap.Scale',function(){ 
            var scale = new AMap.Scale();
            map.addControl(scale); //添加控件
        });
        AMap.plugin('AMap.MapType',function(){ 
            var mapType = new AMap.MapType();
            map.addControl(mapType); //添加控件
        });
        const marker = new AMap.Marker({
            position: [108.352553,34.066937],
            content: `<div class="custom-content-marker">
                <img src="//a.amap.com/jsapi_demos/static/demo-center/icons/poi-marker-red.png">
            </div>`,
            offset: [-13, -30],
        });
        map.add(marker);
        function moveToMarker(){
            map.setZoomAndCenter(12, [108.352553,34.066937], false, 1000);
        }
        document.querySelector(".custom-content-marker").onclick = moveToMarker;
    })
    .catch((e) => {
        console.error(e); //加载错误提示
    });
</script>