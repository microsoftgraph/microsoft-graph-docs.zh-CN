---
author: daspek
title: renameAction 资源类型
description: renameAction 对象提供有关重命名项目的活动的信息。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: d513ae68a2f438483930dd51c40fa06bed626d5b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084158"
---
# <a name="renameaction-resource-type"></a>renameAction 资源类型

命名空间：microsoft.graph

[**itemActivity**][activity]上 **存在 renameAction** 资源指示活动重命名了项目。

>**注意：** 项目活动记录当前仅适用于SharePoint OneDrive for Business。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | 项的原名称。
| newName       | string | 项目的新名称。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName&quot;: &quot;string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->

