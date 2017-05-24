# wis-startup-2017
이 repo는 2017년 5월 24일 진행된 WIS 2017 - 스타트업 개발사를 위한 인공지능과 머신러닝 기반 추천 및 예측 서비스 구축 발표에 대한 코드와 sample 예제 코드를 포함

- WIS 2017 conference : http://onoffmix.com/event/100628
- Short URL : http://aka.ms/wis2017   
- Github URL : https://github.com/CloudBreadPaPa/wis-startup-2017
- Slideshare : <준비중>

## 발표자료
전체 발표자료는 이 repo의 doc 폴더에서 pdf로 다운로드 가능  

## 발표 소스코드
speech sample code는 speech-code 폴더 하위에서 다운로드 가능  

```
SpeechSample.exe https://speech.platform.bing.com/recognize zira.wav
또는 코드의 언어를 한글로 변경 후 수행 테스트  
SpeechSample.exe https://speech.platform.bing.com/recognize fake.wav
```

한글로 변경하는 코드
```
/* URI Params. Refer to the README file for more information. */
requestUri += @"?scenarios=smd";                                  // websearch is the other main option.
requestUri += @"&appid=D4D52672-91D7-4C74-8AD8-42B1D98141A5";     // You must use this ID.
//requestUri += @"&locale=en-US";                                   // We support several other 
languages.  Refer to README file.
// 여기를 변경
requestUri += @"&locale=ko-KR";                                   // We support several other languages.  Refer to README file.
requestUri += @"&device.os=wp7";
requestUri += @"&version=3.0";
requestUri += @"&format=json";
requestUri += @"&instanceid=565D69FF-E928-4B7E-87DA-9A750B96D9E3";
requestUri += @"&requestid=" + Guid.NewGuid().ToString();
```

EOF