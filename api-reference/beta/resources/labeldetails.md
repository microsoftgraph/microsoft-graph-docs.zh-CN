---
title: labelDetails 资源类型
description: 代表信息保护标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6b475c96b3ecbc2caa0aa147e3fc8fd0253ac243
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084035"
---
# <a name="labeldetails-resource-type"></a>labelDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表信息保护标签的标签详细信息。 **labelDetails** 提供有关单个信息保护标签的信息。 可以由[evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)和[extractLabel](../api/informationprotectionlabel-extractLabel.md)返回

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| color       | String  | 用户界面针对标签应显示的颜色（如果已配置）。                               |
| 说明 | 字符串  | 管理员定义的标签说明。                                                                 |
| id          | 字符串  | 标签 ID 是 (GUID) 的全局唯一标识符。                                                          |
| isActive    | 布尔 | 指示标签是否处于活动状态。 应在用户界面中隐藏或禁用活动标签。 |
| 名称        | 字符串  | 标签的纯文本名称。                                                                             |
| sensitivity | Int32   | 标签的敏感度值，其中较小的是不敏感的。                                           |
| tooltip     | 字符串  | 应为用户界面中的标签显示的工具提示。                                      |

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

