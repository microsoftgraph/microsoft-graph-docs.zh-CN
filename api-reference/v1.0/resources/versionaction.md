---
author: daspek
title: versionAction 资源类型
description: VersionAction 对象提供有关导致新项版本的活动的信息。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4fbeb09d0fd2f209d436578e29ae7bf1fd404c3c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139552"
---
# <a name="versionaction-resource-type"></a>versionAction 资源类型

命名空间：microsoft.graph

[**itemActivity**][activity]上存在 **versionAction** 资源指示活动导致创建新版本。

>**注意：** 项目活动记录当前仅适用于SharePoint OneDrive for Business。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| newVersion    | string | 此操作创建的新版本的名称。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.versionAction"
}-->

```json
{
  "newVersion&quot;: &quot;string"
}
```

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

