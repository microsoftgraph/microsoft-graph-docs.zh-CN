---
title: outOfOfficeSettings 资源类型
description: 表示联机会议的电话访问信息。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 018852150ef833d8cb114892790f911b4aad8fe0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960375"
---
# <a name="outofofficesettings-resource-type"></a>outOfOfficeSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与用户状态相关的外出设置。 [](presence.md)

## <a name="properties"></a>属性

| 属性            | 类型    | 描述                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| message           | String  | 用户在 Outlook 客户端上配置的外出邮件 (自动答复 (外出) ) 或 Teams 客户端 (计划外出) 。 |
| isOutOfOffice      | Boolean  | 如此 如果：</br><ul><li>它当前处于 Outlook 或 Teams 客户端上配置的外出时间窗口。</li><li>用户日历上当前存在标记为"显示为外出"的事件</li></ul></br>否则为 false。 |

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
