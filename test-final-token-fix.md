---
title: 测试 token 修复 - hexo-deployer-git
date: 2025-11-07 22:25:00
tags:
  - 最终测试
  - token修复
categories:
  - 测试
---

## 关键修复

- ✅ workflow 中传递 DEPLOY_PAT_NEW 环境变量
- ✅ 使用 `hexo deploy --token "$DEPLOY_PAT_NEW"`
- ✅ 移除 _config.yml 错误的 token 配置

## 预期结果

这次应该能成功部署！

