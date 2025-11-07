---
title: 测试 keep_files=false 参数
date: 2025-11-07 22:30:00
tags:
  - keep_files
  - 关键参数
categories:
  - 测试
---

## 关键修复

- ✅ 使用 peaceiris/actions-gh-pages@v4
- ✅ 添加 `force_orphan: true`
- ✅ **新增** `keep_files: false` 参数

## 作用

`keep_files: false` 确保：
- 清空目标仓库的所有旧文件
- 完全替换为新的 public 目录内容
- 避免内容残留或冲突

## 测试目的

验证这次能否成功部署，显示实际的HTML内容而不是空页面。

