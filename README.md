docker rm -f lab1-nginx 2>/dev/null || true && docker run --name lab1-nginx -p 8080:80 -v "$(pwd)/site:/usr/share/nginx/html:ro" -d lab1-web:latest


---

Abra em: http://localhost:8080/