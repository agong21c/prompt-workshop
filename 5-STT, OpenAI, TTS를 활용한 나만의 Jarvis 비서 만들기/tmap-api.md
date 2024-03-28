TMAP API 사용을 위한 준비 과정들

https://open2u.sktelecom.com/web/out/standard.cmd?nc_trId=WWO01N051X02&nc_target=out/wwo/WWO01N051X02.do

https://developers.sktelecom.com/

https://blog.naver.com/asmwj3/221329248020

-> 

https://openapi.sk.com/

### CURL Sample:
https://injae7034.github.io/kotlin/tmap-open-api-pedestrian/

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
