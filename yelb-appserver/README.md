# Yelb Appserver

UI에서(또는 원하는 경우 컬을 통해) 사용되는 여러 API를 가지는 Ruby/Sinatra 애플리케이션입니다. 포트는 4567로 고정됩니다.
직접 빌드하거나, mreferre/yelb-appserver:0.7 이미지를 사용하면 됩니다.

## 환경변수 설명
SEARCH_DOMAIN을 설정했을 때 나머지 환경변수를 설정하면 오류가 생길 수 있습니다.
- SEARCH_DOMAIN : redis-server, yelb-db를 호출할 때 Base Domain을 설정합니다. (예시 : yelb.local로 설정했을 때 redis-server.yelb.local, yelb-db.yelb.local을 고정으로 호출합니다.)
- RACK_ENV : 배포 환경을 설정합니다. 데이터베이스 엔드포인트를 수정해야 한다면 반드시 "custom"으로 설정해야 합니다.
- REDIS_SERVER_ENDPOINT : REDIS 엔드포인트를 설정합니다. (예시 : redis-server.yelb.local)
- YELB_DB_SERVER_ENDPOINT : YELB_DB 엔드포인트를 설정합니다. (예시 : yelb-db.yelb.local)