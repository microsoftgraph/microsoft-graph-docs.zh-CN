---
title: alertHistoryState 资源类型
description: 存储对警报所做的更改。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1a7975d870389be5163a8f230f6a6cc4cd1425c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461045"
---
# <a name="alerthistorystate-resource-type"></a>alertHistoryState 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

存储对警报所做的更改。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|appId|字符串| 向警报提交更新 (修补程序) 的呼叫应用程序的应用程序 ID。 应从身份验证令牌中提取 appId, 并且调用应用程序不手动输入该 appId。 |
|assignedTo|String| 向其分配了警报的用户的 UPN (注意: alert。分配程序仅存储最后一个 value/UPN)。 |
|comments|String collection|登录用户输入的注释。|
|征求|字符串| 此更新中有关通知的分析师反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。|
|status|字符串| 警报状态值 (如果已更新)。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved` 或 `dismissed`。|
|updatedDateTime|DateTimeOffset| 通知更新的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|user|字符串| 更新了警报的已登录用户 (在用户/委派身份验证模式下) 中的 UPN。 |

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