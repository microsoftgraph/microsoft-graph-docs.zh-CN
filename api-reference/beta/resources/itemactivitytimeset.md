---
author: daspek
description: ItemActivityTimeSet 资源提供有关项上某个活动发生时间的信息。
ms.date: 09/14/2017
title: ItemActivityTimeSet
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: eb0477255783b3aba7aaa61a0e9ece868c1882d1
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724323"
---
# <a name="itemactivitytimeset-resource-type"></a>ItemActivityTimeSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemActivityTimeSet** 资源提供有关项上某个 [活动][activity]发生时间的信息。

[activity]: itemactivity.md

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

## <a name="properties"></a>属性

| 属性         | 类型           | 说明                                       |
| :--------------- | :------------- | :------------------------------------------------ |
| observedDateTime | DateTimeOffset | 在观察到要发生活动时。     |
| recordedDateTime | DateTimeOffset | 在服务上记录观察时。 |

对于离线协作方案来说，**观察** 和 **记录** 时间差异尤为重要。
如果用户在离线时对文件添加注释，则会将他们添加注释的时间设置为 **observedDateTime**。
稍后，当用户重新连接到云并上传更改后，则会将稍后的时间设置为 **recordedDateTime**。

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
