# 世界天气查询 World Weather Checker

一个使用 Python 编写的命令行天气查询工具，可以查询世界各地城市的当前天气和未来 1–7 天预报。

## 功能

- 按城市名称搜索世界各地的地点
- 可选指定国家/地区，帮助区分同名城市
- 显示当前天气、气温、体感温度、湿度、风速和降水量
- 显示未来 1–7 天的天气、最高/最低气温和降水概率
- 无需申请 API Key

## 环境要求

- Python 3.9 或更高版本
- 网络连接

## 安装

```bash
git clone https://github.com/YOUR-USERNAME/world-weather-checker.git
cd world-weather-checker
python -m pip install -r requirements.txt
```

## 运行

交互式查询：

```bash
python weather_app.py
```

直接查询城市：

```bash
python weather_app.py --city Singapore
python weather_app.py --city Tokyo --country Japan
python weather_app.py --city London --country GB --days 5
```

`--days` 支持 1 到 7，默认显示 3 天预报。搜索结果存在多个匹配地点时，程序会让你选择。

## 数据来源与说明

天气和地理编码数据由 [Open-Meteo](https://open-meteo.com/) 提供。查询需要网络连接；如果请求失败，请稍后重试或检查网络。天气预报仅供参考。

## 上传到 GitHub

1. 在 GitHub 新建一个仓库，例如 `world-weather-checker`。
2. 将 `weather_app.py`、`requirements.txt` 和 `README.md` 上传到仓库。
3. 或在本地项目文件夹运行：

```bash
git init
git add weather_app.py requirements.txt README.md
git commit -m "Add world weather checker"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/world-weather-checker.git
git push -u origin main
```

将 `YOUR-USERNAME` 替换成你的 GitHub 用户名。第一次使用 Git 时，可能需要先安装 Git 并完成 GitHub 身份验证。
