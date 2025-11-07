---
title: 测试删除操作顺序修复
date: 2025-11-07 22:40:00
tags:
  - 删除操作
  - 部署修复
categories:
  - 测试
---

## 关键修复 (删除操作相关)

### 删除顺序：
1. ✅ `hexo clean` - 清理旧缓存
2. ✅ `hexo generate` - 生成新文件  
3. ✅ **新增** 验证步骤 - 检查 public/index.html
4. ✅ `deploy` - 部署到目标仓库

### 部署配置：
- ✅ `force_orphan: true` - 清空目标分支
- ✅ `keep_files: false` - 删除所有旧文件
- ✅ `publish_branch_force: true` - 强制推送
- ✅ `cname: godream.show` - 保留域名
- ✅ `allow_empty_commit: false` - 阻止空提交

## 验证点

现在部署应该：
- ✅ 正确执行删除操作
- ✅ 部署实际内容而不是空文件
- ✅ 保持域名配置

