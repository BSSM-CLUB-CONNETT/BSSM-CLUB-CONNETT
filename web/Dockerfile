# 1. Nginx 공식 이미지 사용
FROM nginx:latest

# 2. 서비스할 웹 파일(HTML, CSS 등)을 컨테이너 내부로 복사
COPY ./web/src /usr/share/nginx/html

# 3. 컨테이너가 외부로 노출할 포트 지정(run 할때 포트 지정해줘야함)
EXPOSE 80

# 4. Nginx 백그라운드 실행 방지 및 포어그라운드(foreground) 실행
CMD ["nginx", "-g", "daemon off;"]