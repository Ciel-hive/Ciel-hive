---
title: "VsCode使用"
date: 2020-07-01
category: Software
tags: [VsCode]
excerpt: VsCode使用
---

# 模板代码创建
1. 快捷键：`Ctrl+Shift+p` 搜索snippet,或者`管理->用户代码片段`
2. 输入模板名生成json文件，以markdown为例(markdown.json):
	```
	{
		"markdown template": {
			"prefix": "md",
			"body": [
				"---",
				"title: \"TODO\"",
				"date: $CURRENT_YEAR-$CURRENT_MONTH-$CURRENT_DATE",
				"category: TODO",
				"tags: [TODO]",
				"excerpt: TODO",
				"---"
			],
			"description": "markdown template"
		}
	}
	```
3. `Ctrl+p`搜索settings.json,启用markdown的快速提示
	```
	{
		"[markdown]":{
			"editor.quickSuggestions": true
		}
	}
	```