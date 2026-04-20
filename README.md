# 每日内容推送自动化

中年觉醒 + 心理健康每日关怀，推送到飞书群。

## 功能

- **每天 07:15** (北京时间) 自动推送两条内容

### 中年觉醒主题
- 周一：职场感悟
- 周二：家庭关系
- 周三：健康提醒
- 周四：成长思考
- 周五：财务思考
- 周六：情感共鸣
- 周日：周末放松

### 心理健康主题
- 周一：早安能量
- 周二：情绪释放
- 周三：生活感悟
- 周四：正向鼓励
- 周五：深度陪伴
- 周六：周末预告
- 周日：下周预告

## 配置

### 1. 设置 GitHub Secrets

在 GitHub 仓库 Settings → Secrets 中添加：

| Name | Value |
|------|-------|
| `FEISHU_WEBHOOK` | 飞书 Webhook URL |

### 2. 启用 Actions

在 GitHub 仓库 Actions 页面启用 workflow。

## 本地测试

```bash
pip install requests pytz
python scripts/send_middle_age.py
python scripts/send_mental_health.py
```
