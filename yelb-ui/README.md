# Yelb Ui

사용자가 사이트를 이용할 수 있는 Angular2 애플리케이션입니다. 포트는 80으로 고정됩니다.
직접 빌드하거나, mreferre/yelb-ui:0.10 이미지를 사용하면 됩니다.

## 환경변수 설명
SEARCH_DOMAIN을 설정했을 때 나머지 환경변수를 설정하면 오류가 생길 수 있습니다.
- SEARCH_DOMAIN : yelb-appserver를 호출할 때 Base Domain을 설정합니다. (예시 : yelb.local로 설정했을 때 yelb-appserver.yelb.local을 고정으로 호출합니다.)
- YELB_APPSERVER_ENDPOINT : yelb-appserver 엔드포인트를 설정합니다. 프로토콜과 포트를 모두 포함한 주소여야 합니다. (예시 : http://yelb-appserver.yelb.local:4567)