---
name: Agnes AI 视频生成
description: 使用 Agnes AI API 生成视频和图片内容
author:
  name: LeeGoHai-Get
version: 1.0.0
---

# Agnes AI 视频生成 Skill

通过调用自建的 HTTP API 服务来生成 AI 视频和图片内容。

## ⚠️ 使用前必读

**调用任何工具之前，必须先询问用户提供 Agnes AI API Key。**
- 如果用户尚未提供 `api_key`，请主动询问，**不要使用占位符值**
- 获取到用户的 `api_key` 后，将其填入请求体的 `api_key` 字段
- 同时询问用户是否需要自定义 `base_url`（默认为 https://hzhy.store）

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
 "api_key": "用户的 Agnes AI API Key",
 "base_url": "https://hzhy.store"
}
