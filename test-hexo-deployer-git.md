---
title: 测试 hexo-deployer-git 部署方案
date: 2025-11-07 22:20:00
tags:
  - hexo-deployer-git
  - 部署测试
categories:
  - 测试
---

## 关键修改

从 GitHub Action 改为 hexo-deployer-git：
- ✅ 移除 peaceiris/actions-gh-pages@v4
- ✅ 使用 hexo-deployer-git 直接推送
- ✅ 配置 DEPLOY_PAT_NEW token 认证

## 预期结果

这次应该能成功部署，网站应该显示内容而不是空页面！

