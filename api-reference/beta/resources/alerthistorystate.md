---
title: alertHistoryState 资源类型
description: 每次修补警报时, 更改都会保存在 alertHistoryState 的新对象中, 并将作为修改的警报的一部分返回。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: a5dda54101264ee2ec4d01a283f96a93f1d6e5e3
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366964"
---
# <a name="alerthistorystate-resource-type"></a>alertHistoryState 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

每次修补警报时, 更改都会保存在 alertHistoryState 的新对象中, 并将作为修改的警报的一部分返回。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|appId|String| 向警报提交更新 (修补程序) 的呼叫应用程序的应用程序 ID。 应从身份验证令牌中提取 appId, 并且调用应用程序不手动输入该 appId。 |
|assignedTo|String| 向其分配了警报的用户的 UPN (注意: alert。分配程序仅存储最后一个 value/UPN)。 |
|comments|String collection|登录用户输入的注释。|
|征求|String| 此更新中有关通知的分析师反馈。 可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。|
|status|字符串| 警报状态值 (如果已更新)。 可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`、`dismissed`。|
|updatedDateTime|DateTimeOffset| 通知更新的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|user|String| 更新了警报的已登录用户 (在用户/委派身份验证模式下) 中的 UPN。 |

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