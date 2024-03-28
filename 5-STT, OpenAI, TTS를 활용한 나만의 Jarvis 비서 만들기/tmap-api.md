TMAP API 사용을 위한 준비 과정들

https://open2u.sktelecom.com/web/out/standard.cmd?nc_trId=WWO01N051X02&nc_target=out/wwo/WWO01N051X02.do

https://developers.sktelecom.com/

https://blog.naver.com/asmwj3/221329248020

-> 

https://openapi.sk.com/

### CURL Sample:
https://injae7034.github.io/kotlin/tmap-open-api-pedestrian/

**보행자 경로 요청**
```
curl --request POST \
     --url 'https://apis.openapi.sk.com/tmap/routes/pedestrian?version=1&callback=function' \
     --header 'accept: application/json' \
     --header 'appKey: -------' \
     --header 'content-type: application/json' \
     --data '
{
  "startX": 126.92365493654832,
  "startY": 37.556770374096615,
  "angle": 20,
  "speed": 30,
  "endPoiId": "10001",
  "endX": 126.92432158129688,
  "endY": 37.55279861528311,
  "passList": "126.92774822,37.55395475_126.92577620,37.55337145",
  "reqCoordType": "WGS84GEO",
  "startName": "%EC%B6%9C%EB%B0%9C",
  "endName": "%EB%8F%84%EC%B0%A9",
  "searchOption": "0",
  "resCoordType": "WGS84GEO",
  "sort": "index"
}
'
```

https://skopenapi.readme.io/reference/%EC%86%8C%EA%B0%9C

https://skopenapi.readme.io/reference/%EB%B3%B4%ED%96%89%EC%9E%90-%EA%B2%BD%EB%A1%9C%EC%95%88%EB%82%B4

**자동차경로 요청**

```
curl --request POST \
     --url 'https://apis.openapi.sk.com/tmap/routes?version=1&callback=function' \
     --header 'accept: application/json' \
     --header 'appKey: e8wHh2tya84M88aReEpXCa5XTQf3xgo01aZG39k5' \
     --header 'content-type: application/json' \
     --data '
{
  "tollgateFareOption": 16,
  "roadType": 32,
  "directionOption": 1,
  "endX": 129.07579349764512,
  "endY": 35.17883196265564,
  "endRpFlag": "G",
  "reqCoordType": "WGS84GEO",
  "startX": 126.98217734415019,
  "startY": 37.56468648536046,
  "gpsTime": "20191125153000",
  "speed": 10,
  "uncetaintyP": 1,
  "uncetaintyA": 1,
  "uncetaintyAP": 1,
  "carType": 0,
  "startName": "%EC%9D%84%EC%A7%80%EB%A1%9C%20%EC%9E%85%EA%B5%AC%EC%97%AD",
  "endName": "%ED%97%A4%EC%9D%B4%EB%A6%AC",
  "passList": "127.38454163183215,36.35127257501252",
  "gpsInfoList": "126.939376564495,37.470947057194365,120430,20,50,5,2,12,1_126.939376564495,37.470947057194365,120430,20,50,5,2,12,1",
  "detailPosFlag": "2",
  "resCoordType": "WGS84GEO",
  "sort": "index"
}
'
```
