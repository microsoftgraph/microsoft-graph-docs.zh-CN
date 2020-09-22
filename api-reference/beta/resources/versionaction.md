---
author: daspek
description: itemActivity 上存在 VersionAction 资源指示活动导致要创建一个新版本。
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0f16858c8b62f327019d2523488827fa6b20dced
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057739"
---
# <a name="versionaction-resource-type"></a>VersionAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[**itemActivity**][activity] 上存在 **VersionAction** 资源指示活动导致要创建一个新版本。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| newVersion    | string | 此操作创建的新版本的名称。

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->


