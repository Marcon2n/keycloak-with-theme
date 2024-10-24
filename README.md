Sử dụng Keycloakify để build theme

Sau đó lấy file jar build để vào folder (sửa lại tên file trong dockerfile) và chạy lệnh để tạo Image Keycloak và run

buid command
docker build -t {IMAGE_NAME} .

run command
docker run -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin -p 8080:8080 {IMAGE_NAME}
