---
title: alertHistoryState 资源类型
description: 存储对警报所做的更改。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2bc1c1a58f6f7f073b6803adbee07b4b2990a0e1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722165"
---
# <a name="alerthistorystate-resource-type"></a>alertHistoryState 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

存储对警报所做的更改。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|appId|String| 提交更新的调用应用程序的应用程序 ID (PATCH) 警报。 appId 应从身份验证令牌中提取，调用应用程序不应手动输入。 |
|assignedTo|String| 警报已分配给用户的 UPN， (注意：alert.assignedTo 仅存储最后一个值/UPN) 。 |
|comments|字符串集合|登录用户输入的注释。|
|反馈|String| 分析员对此更新中警报的反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。|
|状态|String| 警报状态值 (更新) 。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`、`dismissed`。|
|updatedDateTime|DateTimeOffset| 警报更新的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|user|String| 更新警报的已登录用户的 UPN， (令牌获取的警报- 如果用户/委派身份验证模式) 。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

