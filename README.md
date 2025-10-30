# adsyoutube2graph TD
    A[Client] -->|HTTP Request| B[Web Server]
    B -->|API Call| C[Application Layer]
    C -->|Database Query| D[Database]
    C -->|Message| E[Message Queue]
    E -->|Trigger Event| F[Worker Service]
    F -->|Update| D
    B -->|Static Content| G[CDN]
    A -->|Direct Access| G
    
