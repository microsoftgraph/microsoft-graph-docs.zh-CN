---
title: parentLabelDetails 资源类型
description: 表示信息保护父标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8f1ebe58c3968e0f912806eb6f339bcfd499b57a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679898"
---
# <a name="parentlabeldetails-resource-type"></a>parentLabelDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示信息保护父标签的标签详细信息。 **parentLabelDetails** 提供有关单个信息保护标签的信息。 可通过[evaluateRemoval、evaluateApplication](../api/informationprotectionlabel-evaluateremoval.md)和[extractLabel 返回](../api/informationprotectionlabel-extractLabel.md)[](../api/informationprotectionlabel-evaluateapplication.md)

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| color       | String  | 用户界面应为标签显示的颜色（如果已配置）。                               |
| 说明 | String  | 管理员定义的标签说明。                                                                 |
| id          | String  | 标签 ID 是 GUID (全局唯) 。                                                          |
| isActive    | Boolean | 指示标签是否处于活动状态。 应在用户界面中隐藏或禁用活动标签。 |
| name        | String  | 标签的纯文本名称。                                                                             |
| sensitivity | Int32   | 标签的敏感度值，其中 lower 不太敏感。                                           |
| tooltip     | String  | 应在用户界面中为标签显示的工具提示。                                      |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parentLabelDetails",
  "baseType": null
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "parentLabelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->