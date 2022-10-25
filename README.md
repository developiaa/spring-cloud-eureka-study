# 프로젝트 빌드
`mvn clean compile package`

# Docker 이미지 빌드
`docker build -t developiaa/discovery-service:1.0 .`

# Docker 이미지 업로드
`docker push developiaa/discovery-service:1.0`

# Docker 실행
`docker run -d -p 8888:8888 --network ecommerce-network -e "spring.rabbitmq.host=rabbitmq_docker" -e "spring.profiles.active=default" --name discovery-service developiaa/discovery-service:1.0`
