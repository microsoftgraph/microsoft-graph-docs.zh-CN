---
title: informationProtectionLabel 资源类型
description: 介绍信息保护标签，这些标签详细说明了如何正确地将敏感标签应用于信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 528238d904ac9807027dd51a8c59ed03570c7bc3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938742"
---
# <a name="informationprotectionlabel-resource-type"></a>informationProtectionLabel 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍信息保护标签，这些标签详细说明了如何正确地将敏感标签应用于信息。 **InformationProtectionLabel**资源描述了适用于用户或租户的敏感度标签的配置。  

## <a name="methods"></a>方法

| 方法                                                                                              | 返回类型                                                               | 说明                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [列出 informationProtectionLabel](../api/informationprotectionpolicy-list-labels.md)                | [informationProtectionLabel](informationprotectionlabel.md)集合 | 列出用户或租户的所有已配置的信息保护标签。                                                                                                |
| [获取 informationProtectionLabel](../api/informationprotectionlabel-get.md)                          | [informationProtectionLabel](informationprotectionlabel.md)               | 在给定特定标签 ID 的情况下，返回**informationProtectionLabel**。                                                                                                  |
| [evaluateapplication](../api/informationprotectionlabel-evaluateapplication.md)                     | [informationProtectionAction](informationprotectionaction.md)集合  | 给定[contentInfo](contentinfo.md)和[labelingOptions](labelingoptions.md)的输入，计算一组操作需要应用标签。                      |
| [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) | [informationProtectionAction](informationprotectionaction.md)集合  | 给定[contentInfo](contentinfo.md)和分类结果的输入，计算一组操作需要应用标签。                                  |
| [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)                             | [informationProtectionAction](informationprotectionaction.md)集合  | 给定[contentInfo](contentinfo.md)和[downgradeJustification](downgradejustification.md)的输入，计算要删除标签应采取的操作。 |
| [extractLabel](../api/informationprotectionlabel-extractlabel.md)                                   | [informationProtectionContentLabel](informationprotectioncontentlabel.md) | 给定[contentInfo](contentinfo.md)的输入，返回有关元数据表示的[informationProtectionLabel](informationprotectionlabel.md)的详细信息。       |

## <a name="properties"></a>属性

| 属性    | 类型    | 描述                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| color       | String  | UI 应为标签显示的颜色（如果已配置）。                              |
| description | String  | 管理员定义的标签说明。                                                    |
| id          | String  | 标签 ID 是一个全局唯一标识符（GUID）                                             |
| isActive    | Boolean | 指示标签是否处于活动状态。 应在 UI 中隐藏或禁用活动标签。 |
| name        | 字符串  | 标签的纯文本名称。                                                                |
| sensitivity | Int32   | 标签的敏感度值，其中较小的是不敏感的。                              |
| tooltip     | 字符串  | 应为 UI 中的标签显示的工具提示。                                     |

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
