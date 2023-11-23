# StoreMicroservices-proto

# to generate grpc code from proto files for order service
protoc --proto_path=proto --go_out=./golang/order --go_opt=paths=source_relative --go-grpc_out=./golang/order --go-grpc_opt=paths=source_relative order.proto

# to generate grpc code from proto files for payment service
protoc --proto_path=proto --go_out=./golang/payment --go_opt=paths=source_relative --go-grpc_out=./golang/payment --go-grpc_opt=paths=source_relative payment.proto

