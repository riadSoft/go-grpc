# go-grpc
Ejemplo de servicios GRPC con Go, Servidor Cliente

Instalar los componentes necesarios:
```Go
instalar protoc
go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2
En archlinux
yay -S protobuf  
yay -S protoc-gen-go-grpc 
yay -S protoc-gen-go
Crear el archivo proto
Para crear los archivos ejecutar el comando
protoc --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative proto/todo.proto

