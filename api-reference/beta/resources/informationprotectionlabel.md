---
title: informationProtectionLabel 资源类型
description: 介绍信息保护标签，这些标签详细说明了如何正确地将敏感标签应用于信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b634166896932897b200d2eeb17a1e54aadb543
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021924"
---
# <a name="informationprotectionlabel-resource-type"></a>informationProtectionLabel 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍信息保护标签，这些标签详细说明了如何正确地将敏感标签应用于信息。 **InformationProtectionLabel**资源描述了适用于用户或租户的敏感度标签的配置。  

## <a name="methods"></a>方法

| 方法                                                                                              | 返回类型                                                               | 说明                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [列出 informationProtectionLabel](../api/informationprotectionpolicy-list-labels.md)                | [informationProtectionLabel](informationprotectionlabel.md) 集合 | 列出用户或租户的所有已配置的信息保护标签。                                                                                                |
| [获取 informationProtectionLabel](../api/informationprotectionlabel-get.md)                          | [informationProtectionLabel](informationprotectionlabel.md)               | 在给定特定标签 ID 的情况下，返回 **informationProtectionLabel**。                                                                                                  |
| [evaluateapplication](../api/informationprotectionlabel-evaluateapplication.md)                     | [informationProtectionAction](informationprotectionaction.md) 集合  | 给定 [contentInfo](contentinfo.md) 和 [labelingOptions](labelingoptions.md)的输入，计算一组操作需要应用标签。                      |
| [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) | [informationProtectionAction](informationprotectionaction.md) 集合  | 给定 [contentInfo](contentinfo.md) 和分类结果的输入，计算一组操作需要应用标签。                                  |
| [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)                             | [informationProtectionAction](informationprotectionaction.md) 集合  | 给定 [contentInfo](contentinfo.md) 和 [downgradeJustification](downgradejustification.md)的输入，计算要删除标签应采取的操作。 |
| [extractLabel](../api/informationprotectionlabel-extractlabel.md)                                   | [informationProtectionContentLabel](informationprotectioncontentlabel.md) | 给定 [contentInfo](contentinfo.md)的输入，返回有关元数据表示的 [informationProtectionLabel](informationprotectionlabel.md) 的详细信息。       |

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| color       | String  | UI 应为标签显示的颜色（如果已配置）。                              |
| description | String  | 管理员定义的标签说明。                                                    |
| id          | String  | 标签 ID 是 GUID (的全局唯一标识符)                                              |
| isActive    | Boolean | 指示标签是否处于活动状态。 应在 UI 中隐藏或禁用活动标签。 |
| name        | String  | 标签的纯文本名称。                                                                |
| 敏感度 | Int32   | 标签的敏感度值，其中较小的是不敏感的。                              |
| tooltip     | String  | 应为 UI 中的标签显示的工具提示。                                     |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String (identifier)",
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
  "description": "informationProtectionLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


