# Agnes AI 视频生成

## 描述

使用 Agnes AI API 生成视频内容

## 工具

### generate_video

生成视频

**参数：**
- `prompt` (string, required): 视频描述
- `width` (number, optional): 宽度，默认 1152
- `height` (number, optional): 高度，默认 768
- `num_frames` (number, optional): 帧数，默认 121
- `frame_rate` (number, optional): 帧率，默认 24

## 配置

需要在请求头中提供：
- `X-API-Key`: Agnes AI API Key
- `X-Base-Url`: API 基础地址（可选，默认 https://apihub.agnes-ai.com）

## 端点

- `POST /video` - 生成视频
- `POST /image` - 生成图片
- `GET /health` - 健康检查
