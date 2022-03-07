FROM nginx
COPY nginx.conf /etc/nginx/nginx.conf
COPY server-https-common.conf /etc/nginx/server-https-common.conf
COPY ssl/public.crt /certs/public.crt
COPY ssl/private.key /certs/private.key


### TimeZone 환경 변수 지정
ENV TZ Asia/Seoul

### TimeZone 설정
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
