# Start React Native

## React Native Packages 설치

1. 명령프롬프트 관리자 권한으로 실행후 npm install --global expo-cli 설치.\
2. 설치할 폴더로 이동후 npx create-expo-app my-app(폴더명)  →  설치후 VSCODE 실행
3. VSCODE 터미널에서 expo login 으로 로그인 해준다.  →  npm start

### `Design`

import { StatusBar } from 'expo-status-bar'\
StatusBar style="Auto" => 디바이스의 상단 메뉴 조절(시간, 배터리 등등...)\
contentContainerStyle : 모든 하위 보기를 래핑하는 스크롤 보기 콘텐츠 컨테이너에 적용됩니다.\
horizontal : ScrollView 안에 View 들을 (horizontal)가로로 정렬한다.\
pagingEnabled : true인 경우 스크롤할 때 스크롤 보기가 스크롤 보기 크기의 배수에서 멈춥니다. 수평 페이지 매김에 사용할 수 있습니다.\
showsHorizontalScrollIndicator : pagingEnabled 될때 true 인경우 가로 스크롤 표시기를 표시합니다.\
const { width: SCREEN_WIDTH } = Dimensions.get("window") : 디바이스의 width를 찾는다.

### `Location`

유저의 위치를 받아오기 위한 API\
https://docs.expo.dev/versions/v46.0.0/sdk/location/ \
Teminal : expo install expo-location 설치.

import * as Location from "expo-location"; \
location => https://docs.expo.dev/versions/v46.0.0/sdk/location/ 참조. \