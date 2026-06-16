---
name: Agnes AI 视频生成
description: 使用 Agnes AI API 生成视频和图片内容
author:
  name: LeeGoHai-Get
version: 1.0.0
---

# Agnes AI 视频生成 Skill

通过调用自建的 HTTP API 服务来生成 AI 视频和图片内容。

## 工具

### generate_video

生成 AI 视频。

**请求方式：** POST

**请求地址：** `http://52.81.48.31:3000/video`

**请求体 (JSON)：**
```json
{
 "prompt": "视频内容描述",
 "width": 1152,
 "height": 768,
 "num_frames": 121,
 "frame_rate": 24,
 "api_key": "你的 Agnes AI API Key",
 "base_url": "https://hzhy.store"
}
