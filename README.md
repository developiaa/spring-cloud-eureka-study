# 프로젝트 빌드
`mvn clean compile package`

# Docker 이미지 빌드
`docker build -t developiaa/discovery-service:1.0 .`

# Docker 이미지 업로드
`docker push developiaa/discovery-service:1.0`

# Docker 실행
`docker run -d -p 8761:8761 --network ecommerce-network -e "spring.cloud.config.uri=http://config-service:8888" --name discovery-service developiaa/discovery-service:1.0`
