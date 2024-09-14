# 低成本高空气象气球/低空卫星解决方案

摆了三年又三年可算熬来了毕设。既来之则安之，不如玩点好玩的。

故而有此滑稽选题。 高空气象气球或近地轨道卫星早已是成熟的解决方案，因此本仓库毫无经济价值、创新价值，唯一承载的职能就是实现把探头放上天、实时回传以及存活的越久越好。

## 包括但不限于：

- 使用究极无敌落后方案折腾新鲜事物（史称关公骑木马）
    - EG : 走AI TEXT-TO-VOICE 来实现32进制信息明文传输(?)

- 经济节省形方案。电子垃圾为主，图吧禁片。

- 稳定性无要求，多活一秒赚一秒。

## 基础结构与部件：

- ### 硬件【无线409MHz通信方案）

    - 气象气球/低空卫星
        - 气象气球 45 R
        - 主控：小米 4 （赛博垃圾王） 30 R
        - 通讯：宝峰 Uv 3代 5W
    
    - 地面基站
        - 主控 OrangePi Zero / RaspberryPi Zero /Rockchip 1068
        - 通讯: 
            - WLAN 有线直连
            - RTL2832U SDR Adapter

- ### 控制系统

    - Web 数据采集
        - Browser WebRtc interface
        - Browser GPS interface
        - Browser 陀螺仪 interface
        - Browser 水平仪 interface
        - Browser 气压计 interface
    - 数字转模拟通信
        - SSTV
        - BASE32 明文
    - 数据总服
        - Express
    - Dashboard / Miniapp
        - Nextjs

## TODO : 

    - Web 数据采集测试、开发
    - 数字转模拟信号测试
    - 陆地长程通讯测试