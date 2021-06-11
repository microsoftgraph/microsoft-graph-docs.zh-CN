---
title: outOfOfficeSettings 资源类型
description: 表示联机会议的电话访问信息。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13f826babea1e6f9448d1ecb9b8100baaf962b20
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896632"
---
# <a name="outofofficesettings-resource-type"></a>outOfOfficeSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与用户状态相关的外出设置。 [](presence.md)

## <a name="properties"></a>属性

| 属性            | 类型    | 描述                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| message           | String  | 用户在 Outlook 客户端上配置的外出 (自动答复 (Out Office) ) 或 Teams client (Schedule out of office) 。 |
| isOutOfOffice      | Boolean  | 如此 如果：</br><ul><li>它当前位于在 Outlook 或 Teams 客户端上配置的外出时间窗口。</li><li>用户日历上当前有一个标记为"显示为外出"Office</li></ul></br>否则为 false。 |

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
