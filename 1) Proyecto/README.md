# Redes de Streaming con Yolo v8 con conectividad a switch y router

La aqruitectura que deben desarrollar los estudiantes es:

<div align="center">
<pre>
┌─────────────────────┐
│ 1. Fuente de video  │
│  (Cámara IP / RTSP  │
│   / archivo MP4)    │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 2. Captura y        │
│    decodificación   │
│    (OpenCV/FFmpeg)  │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 3. Preprocesamiento │
│  (resize, normalize,│
│   tensor)           │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 4. Inferencia       │
│    YOLOv8           │
│  (detección/segmen- │
│   tación/pose)      │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 5. Post-procesado   │
│  (NMS, tracking,    │
│   conteo, alertas)  │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 6. Codificación y   │
│    empaquetado      │
│  (H.264/H.265, RTMP │
│   / RTSP / WebRTC)  │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 7. Switch (Capa 2)  │
│  VLANs, QoS,        │
│  trunk, STP         │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 8. Router (Capa 3)  │
│  Enrutamiento, NAT, │
│  firewall, VPN      │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 9. Cliente/         │
│    Visualizador     │
│  (VLC, navegador,   │
│   dashboard)        │
└─────────────────────┘
</pre>
</div>



     

