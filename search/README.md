# 学校自讯

基于真实学生评价的高校信息搜索平台。

## 数据来源

所有数据来自 [CollegesChat/university-information](https://github.com/CollegesChat/university-information) 开源项目。

该项目由「高校生活」社区维护，通过问卷收集的方式，获取全国各高校在校生对学校生活的真实评价，涵盖以下维度：

- 宿舍条件（床型、空调、卫浴、限电等）
- 食堂餐饮（价格、卫生）
- 校园交通（地铁、共享单车）
- 作息制度（早晚自习、晨跑、门禁）
- 校园设施（超市、快递、网络）
- 学习环境（自习、电脑、校园卡）

> **免责声明**：本站内容均来源于问卷收集，仅供参考，请自行确定信息准确性和真实性。

## 项目结构

```
├── index.html            # 网页（可直接部署到 GitHub Pages）
├── universities.json     # 学校数据索引
├── universities/         # 各校评价详情（Markdown）
└── build_data.py         # 数据构建脚本
```

## 部署

1. Fork 或 clone 本仓库
2. 在 GitHub 仓库 Settings → Pages 中选择分支部署
3. 访问 `https://<用户名>.github.io/<仓库名>/`

## 本地运行

```bash
python build_data.py        # 生成 universities.json
python -m http.server 8080  # 启动本地服务
```

然后访问 `http://localhost:8080`

## 许可

数据版权归 [CollegesChat](https://github.com/CollegesChat) 所有，仅供学习交流使用。
