---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<style>
  /* 隐藏页面顶部的 CV 大标题，但保留浏览器标签页的标题 */
  h1.page__title {
    display: none !important;
  }
</style>

<div style="text-align: center; margin-bottom: 2em;">
  <h2 style="font-size: 16em; margin-bottom: -0.2em;">刘欣然</h2>
  <p style="margin-bottom: 0.5em; color: #555;">
    <i class="fas fa-mobile-alt" style="width: 16px; text-align: center; margin-right: 4px;"></i> 15903682174（微信同号）
    <span style="margin: 0 8px; color: #ccc;">|</span> 
    <i class="fas fa-envelope" style="width: 16px; text-align: center; margin-right: 4px;"></i> <a href="mailto:2103123944@qq.com">2103123944@qq.com</a>
    <span style="margin: 0 8px; color: #ccc;">|</span> 
    <i class="fas fa-globe" style="width: 16px; text-align: center; margin-right: 4px;"></i> <a href="https://Linsensn.github.io" target="_blank">个人主页</a>
    <span style="margin: 0 8px; color: #ccc;">|</span> 
    <i class="fab fa-github" style="width: 16px; text-align: center; margin-right: 4px;"></i> <a href="https://github.com/Linsensn" target="_blank">GitHub</a>
  </p>
  <p style="margin-bottom: 0.5em;"><strong>求职意向：后端 / AI 工程日常实习</strong></p>
  <p style="margin-top: 0.5em; color: #e74c3c;">
    到岗时间：可立即到岗，每周 5 天，可连续实习 8 个月以上
  </p>
</div>

<hr>

<details class="fold" open>
  <summary>教育背景</summary>
  <div>
    <h3 style="display: flex; justify-content: space-between; align-items: baseline; margin-top: 1em; margin-bottom: 0.5em;">
      <span>郑州大学（211） · 计算机科学与技术 · 本科</span>
      <span style="font-weight: normal; color: #666;"><code>2023.09 - 2027.07</code></span>
    </h3>
    <ul>
      <li><strong>学业与英语：</strong>GPA 3.67/4.0 | 专业排名 37/287（前 12.9%）| CET-4 (542)、CET-6 (545)</li>
      <li><strong>荣誉证书：</strong>校级二等奖学金、校级三好学生（2023-2024, 2024-2025）</li>
    </ul>

    <h3 style="display: flex; justify-content: space-between; align-items: baseline; margin-top: 1.5em; margin-bottom: 0.5em;">
      <span>大连理工大学（985） · 计算机技术 · 专业型硕士（推免拟录取）</span>
      <span style="font-weight: normal; color: #666;"><code>2027.09 - 2030.07（预计）</code></span>
    </h3>
  </div>
</details>

<hr>


<details class="fold" open>
  <summary>项目经历</summary>
  <div> 
    <div markdown="1">
      
> 以下代码全部开源，源码详见我的 <a href="https://github.com/Linsensn" target="_blank">GitHub</a> 或者每个项目最后有直达链接。
> 完整技术细节、量化指标、项目演示请跳转项目页面查看：<a href="/portfolio/">项目经历</a>
      
    </div>

    <!-- 项目一 -->
    <h3 style="display: flex; justify-content: space-between; align-items: baseline; margin-top: 1.5em; margin-bottom: 0.5em;">
      <span>WebAR 轻量化实景追踪系统 ｜ <span class="highlight-text">算法与技术总负责人</span></span>
      <span style="font-weight: normal; color: #666;"><code>2025.09 - 2026.01</code></span>
    </h3>
    <p><strong>项目背景：</strong>面向图书馆实景图书检索业务，在云端 <strong>2C4G 无 GPU</strong> 严苛硬件约束下，作为 <strong>7 人团队技术负责人</strong>，完成整套 WebAR 智能导引系统，实现浏览器端无需 APP 即可完成书脊检测、文本识别、检索导航。</p>
    <ul>
      <li><strong>算法与轻量化：</strong>采集标注自建书脊 YOLO、OCR 数据集，完成 YOLOv8-Nano 训练；使用 ONNX 常量折叠、ConvBN 算子融合做轻量化；设计 IoM 嵌套过滤、透视坐标逆映射、多尺度预处理，构建 <strong>SQL-Levenshtein-LLM 三级检索状态机</strong>。</li>
      <li><strong>后端与工程化：</strong>搭建 FastAPI 分层后端，基于 SQLAlchemy + Alembic 落实 Code-First 数据库；Redis 轨迹缓存屏障，配置 LRU、TTL 过期策略；SSE 流式响应、Pydantic 契约校验、异常拦截；Docker 容器化部署，配置健康探针、模型预加载规避 OOM。</li>
      <li><strong>团队管理：</strong>制定 Issue 驱动开发、Git 分支、PR 评审质控门禁，统一团队数据库迁移、接口定义、代码注释全套开发规范。</li>
      <li><strong>量化成果：</strong>模型 mAP50 达到 <span class="highlight-text">0.978</span>，实现<strong>纯 CPU 毫秒级推理</strong>；依靠缓存、异步限流策略保障高并发图像请求下系统<strong>零宕机</strong>；完成整套端到端 WebAR 业务闭环，容器化可直接部署上线。</li>
    </ul>
    <p style="margin-top: -0.5em;"><strong>技术栈：</strong>YOLOv8-Nano、ONNX、PaddleOCR、FastAPI、SQLAlchemy、Alembic、Redis、Docker、JWT · <i class="fab fa-github"></i> <a href="https://github.com/Linsensn/bookway" target="_blank">GitHub 源码</a> · <a href="https://gitee.com/bookway-studio/bookway" target="_blank">Gitee 源码</a></p>

    <br>

    <!-- 项目二 -->
    <h3 style="display: flex; justify-content: space-between; align-items: baseline; margin-top: 2em; margin-bottom: 0.5em;">
      <span>基于大语言模型的多模态 Agent 交互系统 ｜ <span class="highlight-text">算法与技术总负责人</span></span>
      <span style="font-weight: normal; color: #666;"><code>2026.05 - 2026.07</code></span>
    </h3>
    <p><strong>项目背景：</strong>面向学生自主备考场景，搭建多模态智能伴学 Agent 平台，实现异构学习资料解析、大模型对话答疑、智能出题、错题回溯完整业务闭环；作为团队技术总监负责后端架构设计、核心模块编码与团队开发规范落地。</p>
    <ul>
      <li><strong>后端架构：</strong>基于 FastAPI 搭建分层后端，实现全局异常拦截与统一业务响应码；采用 Alembic 落地 Code-First ORM 迁移，制定规约解决多人迁移版本分叉问题；基于 JWT 完成微信 OAuth 鉴权，搭建<strong>学生/管理员 RBAC 角色权限隔离体系</strong>。</li>
      <li><strong>多模态解析与交互：</strong>开发多模态解析中间件，通过 OpenCV 自适应切片、PyMuPDF/antiword、PaddleOCR 降级兜底兼容图片/PDF/Word 素材；封装异步客户端实现 <strong>DeepSeek/GLM 多模型动态路由</strong>，结合 Pydantic 强校验、<strong>SSE 流式响应</strong>与会话持久化保障交互。</li>
      <li><strong>量化成果：</strong>完成整套 Agent 后端底座，支持多格式学习素材上传解析、流式 AI 问答、自动生成测验题库；实现学生会话树形管理、管理员批量管控，解决多模型调用、异构文档解析的工程痛点，容器化交付完整业务后端。</li>
    </ul>
    <p style="margin-top: -0.5em;"><strong>技术栈：</strong>FastAPI、Alembic、JWT、OpenCV、PaddleOCR、DeepSeek、GLM、Pydantic、SSE、Docker · <i class="fab fa-github"></i> <a href="https://github.com/Linsensn/LiteKnow" target="_blank">GitHub 源码</a></p>

    <br>

    <!-- 项目三 -->
    <h3 style="display: flex; justify-content: space-between; align-items: baseline; margin-top: 2em; margin-bottom: 0.5em;">
      <span>基于大语言模型的高并发推理与微调系统 ｜ <span class="highlight-text">算法与技术总负责人</span></span>
      <span style="font-weight: normal; color: #666;"><code>2026.06 - 2026.08</code></span>
    </h3>
    <p><strong>项目背景：</strong>针对电商评论分析场景，解决大模型处理欲扬先抑、欲抑先扬等复杂情感文本时，易被关键词误导产生极性识别反转，以及多模型交叉验证显存溢出、I/O 阻塞问题，基于 Llama3-8B 与 4.5 万条数据集构建高并发评测系统。</p>
    <ul>
      <li><strong>模型微调与评测：</strong>搭建自动化实验流水线，完成多量级数据集消融实验与多架构横向对比；通过混淆矩阵分析 4bit 量化、DoRA 机制带来的模型行为变化。</li>
      <li><strong>推理优化与工程落地：</strong>底层实现<strong>“单基座常驻 + 多 Adapter 毫秒级热插拔”</strong>规避权重重复加载；设计强校验异常拦截、逆向惩罚状态机抑制模型输出发散，开发交互式多模型并发评测工具。</li>
      <li><strong>量化成果：</strong>模型整体准确率达到 <span class="highlight-text">91.54%</span>，F1 分数 <span class="highlight-text">0.9129</span>；大幅降低多模型切换显存开销，实现可交互的大模型批量评测能力。</li>
    </ul>
    <p style="margin-top: -0.5em;"><strong>技术栈：</strong>PyTorch、Llama-3、4bit 量化、DoRA、LoRA、QLoRA、Adapter 热插拔、大模型并发评测 · <i class="fab fa-github"></i> <a href="https://github.com/Linsensn/llama3-sentiment-concurrent" target="_blank">GitHub源码</a></p>
  </div>
</details>

<hr>

<details class="fold" open>
  <summary>专业技能</summary>
  <div>
    <ul>
      <li><strong>编程语言：</strong>熟练 <strong>Python</strong>、<strong>C/C++</strong>；可独立完成算法原型、后端业务接口开发。</li>
      <li><strong>AI 工程与模型：</strong>熟悉 PyTorch；掌握 YOLO 检测、ONNX 模型轻量化算子融合；拥有数据集构建标注、<strong>LoRA 微调、4bit 量化、Adapter 热插拔</strong>实战经验；实践 LangChain Agent、OCR 识别、多模态文档解析。</li>
      <li><strong>后端服务开发：</strong>熟练 FastAPI 分层后端开发；掌握 OAuth 微信鉴权、RBAC 权限隔离、<strong>SSE 大模型流式输出</strong>、Pydantic 强校验；熟练 Alembic 完成 Code-First 数据库迁移；具备全局异常拦截、统一 API 契约设计能力。</li>
      <li><strong>存储中间件：</strong>熟悉 MySQL 索引设计；熟练 Redis，可落地 TTL 过期、LRU 淘汰、业务轨迹缓存屏障，做服务算力保护。</li>
      <li><strong>运维 & 团队协作：</strong>熟悉 Docker 容器化部署、健康探针配置；熟悉 Linux、GitFlow、PR 评审流程；了解结构化日志、全链路请求追踪。</li>
    </ul>
  </div>
</details>

<hr>

<details class="fold" open>
  <summary>竞赛与荣誉</summary>
  <div markdown="1">

| 类别 | 奖项名称 | 级别 / 时间 |
| --- | --- | --- |
| 学科竞赛 | 第十六届蓝桥杯 C/C++ 程序设计大学 A 组三等奖（河南赛区） | 省级 · 2025-05 |
| 创业竞赛 | "挑战杯"大学生创业计划竞赛铜奖（问生医药智能问答平台） | 校级 · 2026-04 |
| 荣誉称号 | 校级三好学生、优秀学生奖学金二等奖 | 校级 · 2023-2025 |
| 社会实践 | 寒假社会实践一等奖（数字助老）、思政实践成果展示特等奖 | 校级 · 2024-2025 |

  </div>
</details>
