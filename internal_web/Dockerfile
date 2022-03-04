FROM nginx
COPY nginx.conf /etc/nginx/nginx.conf
COPY ssl/public.crt /www/internal-web/ssl/public.crt
COPY ssl/private.key /www/internal-web/ssl/private.key


### TimeZone 환경 변수 지정
ENV TZ Asia/Seoul

### TimeZone 설정
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
