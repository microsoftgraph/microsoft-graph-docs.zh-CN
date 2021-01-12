---
title: outOfOfficeSettings 资源类型
description: 表示联机会议的电话访问信息。
author: elvinyang-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4e3e179ec752cfffc4ae4711d9fd0bc541f1506d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796730"
---
# <a name="outofofficesettings-resource-type"></a>outOfOfficeSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与用户状态相关的外出设置。 [](presence.md)

## <a name="properties"></a>属性

| 属性            | 类型    | 描述                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| message           | String  | 用户在 Outlook 客户端上配置的外出邮件 (自动答复 (外出) ) 或 Teams 客户端 (计划外出) 。 |
| isOutOfOffice      | 布尔  | 如此 如果：</br><ul><li>它当前处于 Outlook 或 Teams 客户端上配置的外出时间窗口。</li><li>用户日历上当前有一个标记为"外出"的事件</li></ul></br>否则为 false。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.outOfOfficeSettings"
}-->
```json
{
  "message": "String",
  "isOutOfOffice": "Boolean"
}
```
