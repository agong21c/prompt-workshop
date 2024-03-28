TMAP API 사용을 위한 준비 과정들

https://openapi.sk.com/

* SKTelecom 가입자는 T-world 계정으로 접속 가능

### [SK open API 소개](https://skopenapi.readme.io/reference/%EC%86%8C%EA%B0%9C)

### [로그인/회원가입](https://skopenapi.readme.io/reference/%EB%A1%9C%EA%B7%B8%EC%9D%B8%ED%9A%8C%EC%9B%90%EA%B0%80%EC%9E%85)

### [상품 사용 신청하기](https://openapi.sk.com/products/detail?svcSeq=60&menuSeq=127)
![API 사용 요금](https://openapi.sk.com/upload/service/products_img/2022/10/20/prd_img_1666253058912_0_1_ko.png)

### [TMAP 소개](https://skopenapi.readme.io/reference/t-map-%EC%86%8C%EA%B0%9C)


**보행자 경로 안내** [Link](https://skopenapi.readme.io/reference/%EB%B3%B4%ED%96%89%EC%9E%90-%EA%B2%BD%EB%A1%9C%EC%95%88%EB%82%B4)

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

**자동차 경로안내** [Link](https://skopenapi.readme.io/reference/%EC%9E%90%EB%8F%99%EC%B0%A8-%EA%B2%BD%EB%A1%9C%EC%95%88%EB%82%B4)

```
curl --request POST \
     --url 'https://apis.openapi.sk.com/tmap/routes?version=1&callback=function' \
     --header 'accept: application/json' \
     --header 'appKey: -------'' \
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

**경로안내 샘플예제** [Link](https://skopenapi.readme.io/reference/%EA%B2%BD%EB%A1%9C%EC%95%88%EB%82%B4-%EC%83%98%ED%94%8C%EC%98%88%EC%A0%9C)

[OpenWeatherMap API Key](https://icedhotchoco.tistory.com/entry/OpenWeatherMap-%EB%82%A0%EC%94%A8-API)

