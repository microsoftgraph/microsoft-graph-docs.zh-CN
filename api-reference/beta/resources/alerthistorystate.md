---
title: alertHistoryState 资源类型
description: 存储对警报所做的更改。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: cf8043b4409b29220841e2706649050003b09f34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004277"
---
# <a name="alerthistorystate-resource-type"></a>alertHistoryState 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

存储对警报所做的更改。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|appId|String| 向警报提交更新 (PATCH) 的调用应用程序的应用程序 ID。 应从身份验证令牌中提取 appId，并且调用应用程序不手动输入该 appId。 |
|assignedTo|String| 用户的 UPN 已将警报分配给 (注意： alert。分配仅存储最后一个 value/UPN) 。 |
|comments|字符串集合|登录用户输入的注释。|
|反馈|String| 此更新中有关通知的分析师反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。|
|状态|String| 如果) 更新，则通知状态值 (。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`、`dismissed`。|
|updatedDateTime|DateTimeOffset| 通知更新的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|user|String| 更新了警报的已登录用户的 UPN (从持有者令牌中获取-如果在用户/委派身份验证模式中) 。 |

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

