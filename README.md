# GrpcService
實作 MSDB 上的 gRPC 範例


* 建立 gRPC Server
    ```
    dotnet new grpc -o GrpcGreeter
    code -r GrpcGreeter
    ```
* 套件  
    ```
    Install-Package Google.Protobuf  
    Install-Package Grpc.Tools  
    ```
* 建立 gRPC Client
    ```
    dotnet new console -o GrpcGreeterClient  
    code -r GrpcGreeterClient
    ```
* 套件  
    ```
    Install-Package Grpc.Net.Client  
    Install-Package Google.Protobuf  
    Install-Package Grpc.Tools  
    ```
    
### GrpcGreeter 專案檔：  
* greet.proto： Protos/greet.proto 檔案定義 Greeter gRPC，並用來產生 gRPC 伺服器資產。 
* Services 資料夾：包含服務的執行 Greeter 。
* appSettings.json：包含設定資料，例如 Kestrel 所使用的通訊協定。
* Program.cs：包含 gRPC 服務的進入點。
* Startup.cs：包含設定應用程式行為的程式碼。

參考資料

