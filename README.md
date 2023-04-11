# Test case
1. 레디스 실행
   - docker run --name my-redis -d -p 6379:6379 redis
2. 스프링부트 서비스 두 개 실행
   - jar 로 빌드 (gradle bootJar)
   - jar 파일 위치는 build/libs/PubSubChat-0.0.1-SNAPSHOT.jar
   - java -Dserver.port=8080 -jar PubSubChat-0.0.1-SNAPSHOT.jar
   - java -Dserver.port=8081 -jar PubSubChat-0.0.1-SNAPSHOT.jar
3. 콘솔에서 채팅 테스트 가능