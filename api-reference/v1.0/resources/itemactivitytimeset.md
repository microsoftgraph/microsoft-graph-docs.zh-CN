---
author: daspek
title: itemActivityTimeSet 资源类型
description: itemActionSet 对象提供有关在项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1e69ac8c539dcce56f369adec3d0e634afeeece06cc0b043b48e10f681d12ad8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130077"
---
# <a name="itemactivitytimeset-resource-type"></a>itemActivityTimeSet 资源类型

命名空间：microsoft.graph

**itemActivityTimeSet** 资源提供有关 [项目上的活动][activity]何时发生的信息。

>**注意：** 项目活动记录当前仅适用于SharePoint OneDrive for Business。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称    | 类型           | 说明
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | 在观察到要发生活动时。
| recordedDateTime | DateTimeOffset | 在服务上记录观察时。

对于离线协作方案来说，**观察** 和 **记录** 时间差异尤为重要。
如果用户在离线时对文件添加注释，则会将他们添加注释的时间设置为 **observedDateTime**。
稍后，当用户重新连接到云并上传更改后，则会将稍后的时间设置为 **recordedDateTime**。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka&quot;: &quot;observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->

