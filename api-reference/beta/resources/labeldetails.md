---
title: labelDetails 资源类型
description: 表示信息保护标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: eb66e395d18b7887942753abdebd91d398844290
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579289"
---
# <a name="labeldetails-resource-type"></a>labelDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示信息保护标签的标签详细信息。 **labelDetails** 提供有关单个信息保护标签的信息。 继承自 [parentLabelDetails](parentlabeldetails.md)。 可通过[evaluateRemoval、evaluateApplication](../api/informationprotectionlabel-evaluateremoval.md)和[extractLabel 返回](../api/informationprotectionlabel-extractLabel.md)[](../api/informationprotectionlabel-evaluateapplication.md)

## <a name="properties"></a>属性

| 属性    | 类型                                         | 说明                                                                                                  |
| :---------- | :------------------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| color       | String                                       | 用户界面应为标签显示的颜色（如果已配置）。                               |
| 说明 | String                                       | 管理员定义的标签说明。                                                                 |
| id          | String                                       | 标签 ID 是 GUID (全局唯) 。                                                         |
| isActive    | 布尔                                      | 指示标签是否处于活动状态。 应在用户界面中隐藏或禁用活动标签。 |
| name        | String                                       | 标签的纯文本名称。                                                                             |
| sensitivity | Int32                                        | 标签的敏感度值，其中 lower 不太敏感。                                           |
| tooltip     | String                                       | 应在用户界面中为标签显示的工具提示。                                      |
| 父级      | parentLabelDetails | 与子标签关联的父标签。                                                              |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelDetails",
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
  "description": "labelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

