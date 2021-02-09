---
title: informationProtectionLabel 资源类型
description: 描述信息保护标签，详细介绍了如何向信息正确应用敏感度标签。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 694015f819d1c1afc9fe9feb23c67c92c05eed70
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153622"
---
# <a name="informationprotectionlabel-resource-type"></a>informationProtectionLabel 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述信息保护标签，详细介绍了如何向信息正确应用敏感度标签。 **informationProtectionLabel** 资源描述适用于用户或租户的敏感度标签的配置。  

## <a name="methods"></a>方法

| 方法                                                                                              | 返回类型                                                               | 说明                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [列出 informationProtectionLabel](../api/informationprotectionpolicy-list-labels.md)                | [informationProtectionLabel](informationprotectionlabel.md) 集合 | 列出用户或租户的所有配置的信息保护标签。                                                                                                |
| [获取 informationProtectionLabel](../api/informationprotectionlabel-get.md)                          | [informationProtectionLabel](informationprotectionlabel.md)               | 给定一个特定的标签 ID，返回 **informationProtectionLabel**。                                                                                                  |
| [evaluateapplication](../api/informationprotectionlabel-evaluateapplication.md)                     | [informationProtectionAction](informationprotectionaction.md) 集合  | 给定 [contentInfo](contentinfo.md) 和 [labelingOptions](labelingoptions.md)的输入，计算应用标签需要的操作集。                      |
| [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) | [informationProtectionAction](informationprotectionaction.md) 集合  | 给定 [contentInfo 的输入](contentinfo.md) 和分类结果，计算应用标签需要的操作集。                                  |
| [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)                             | [informationProtectionAction](informationprotectionaction.md) 集合  | 在给定 [contentInfo](contentinfo.md) 和 [downgradeJustification](downgradejustification.md)的输入后，计算删除标签应采取的操作。 |
| [extractLabel](../api/informationprotectionlabel-extractlabel.md)                                   | [informationProtectionContentLabel](informationprotectioncontentlabel.md) | 给定 [contentInfo 的输入](contentinfo.md)，返回元数据表示 [的信息ProtectionLabel](informationprotectionlabel.md) 的详细信息。       |

## <a name="properties"></a>属性

| 属性    | 类型    | 说明                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| color       | String  | UI 应为标签显示的颜色（如果已配置）。                              |
| 说明 | String  | 由管理员定义的标签说明。                                                    |
| id          | String  | 标签 ID 是 GUID (全局)                                              |
| isActive    | 布尔 | 指示标签是否处于活动状态。 应在 UI 中隐藏或禁用活动标签。 |
| 名称        | String  | 标签的纯文本名称。                                                                |
| 敏感度 | Int32   | 标签的敏感度值，其中较低值不太敏感。                              |
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


