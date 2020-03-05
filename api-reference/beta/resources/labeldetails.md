---
title: labelDetails 资源类型
description: 代表信息保护标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cf031459004e0c0d56b5b09145ed897a9f960142
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523007"
---
# <a name="labeldetails-resource-type"></a>labelDetails 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表信息保护标签的标签详细信息。 **labelDetails**提供有关单个信息保护标签的信息。 可以由[evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)和[extractLabel](../api/informationprotectionlabel-extractLabel.md)返回

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| color       | String  | 用户界面针对标签应显示的颜色（如果已配置）。                               |
| 说明 | String  | 管理员定义的标签说明。                                                                 |
| id          | String  | 标签 ID 是一个全局唯一标识符（GUID）。                                                          |
| isActive    | 布尔 | 指示标签是否处于活动状态。 应在用户界面中隐藏或禁用活动标签。 |
| name        | 字符串  | 标签的纯文本名称。                                                                             |
| sensitivity | Int32   | 标签的敏感度值，其中较小的是不敏感的。                                           |
| tooltip     | String  | 应为用户界面中的标签显示的工具提示。                                      |

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