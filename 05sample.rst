广告请求和返回json示例
=============================

广告请求json示例
-----------------------------------------


.. code-block:: python
    :linenos:

    {
        "id":"任意填写，建议时间戳",
        "app":{
            "id":"媒体ID",
            "publisher":{
                "id":"开发者ID"
            }
        },
        "device":{
            "devicetype":"1",
            "make":"apple",
            "model":"iphone",
            "hwv":"7",
            "os":"1",
            "osv":"11.0.1",
            "size":"640x960",
            "pixel_ratio":"1",
            "screen_density":"1",
            "screen_orientation":"1",
            "ua":"Mozilla/5.0 (iPhone; U; CPU iPhone OS 4_3_2 like Mac OS X; en-us) AppleWebKit/533.17.9 (KHTML, like Gecko) Version/5.0.2 Mobile/8H7 Safari/6533.18.5",
            "ip":"xxx.xxx.xxx.xxx",
            "ifa":"ifa",
            "ifa_md5":"ifa_md5",
            "android_id":"android_id",
            "android_id_md5":"android_id_md5",
            "imei":"imei",
            "imei_md5":"imei_md5",
            "mac":"mac",
            "mac_md5":"mac_md5",
            "duid":"duid",
            "duid_md5":"duid_md5"
        },
        "network":{
            "type":"1",
            "operator":"1",
            "cellular_id":"1",
            "wifis":[
                {
                    "mac":"1",
                    "rssi":"1"
                }
            ]
        },
        "adpos":[
            {
                "pos_id":"广告位ID",
                "capacity":"1"
            }
        ]
    }

广告返回json示例
-----------------------------------------

.. code-block:: python
    :linenos:


    {
    "success":true,
    "id":"0922",
    "nbr":0,
    "bidid":"932916559284809546",
    "ads":[
        {
            "id":"932916559406522191",
            "price":0.1,
            "cost_type":2,
            "pos_id":"10000",
            "interaction_type":1,
            "creative_elements":{
                "image":"https://saascdn.xxxx.cn/c-34a29424-f13b-402c-aa5d-02a910940adb.jpg"
            },
            "site_url":"http://www.adxing.com",
            "click_tracking_url":"https://mmptr.limei.com/mtx/c?id=932916559406522191",
            "imp_tracking_urls":[
                "http://www.adxing.com",
                "https://mbptr.adxing.cn/at/i?id=932916559406s522191",
                "https://mmptr.adxing.com/mtx/i?id=932916559406522191"
            ]
        }
     ]
    }
