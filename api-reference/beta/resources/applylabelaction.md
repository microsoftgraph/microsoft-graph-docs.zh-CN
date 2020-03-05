---
title: applyLabelAction 资源类型
description: 代表应用或更新标签应执行的一组操作。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a2e30856aed08cd27916d43c79e52548657023d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508252"
---
# <a name="applylabelaction-resource-type"></a>applyLabelAction 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表应用或更新标签应执行的一组操作。 当标签求值操作的结果是应应用标签时，将返回**applyLabelAction** 。 该`actions`属性包含一个[informationProtectionAction](informationProtectionaction.md)集合，该集合描述了要*应用*标签的完整操作集，包括删除旧元数据、内容标记和保护。

## <a name="properties"></a>属性

| 属性                    | 类型                                                                     | 说明                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| actionSource                | String                                                                   | 可能的值是：`manual`、`automatic`、`recommended`、`default`。                                                                                                                             |
| actions                     | [informationProtectionAction](informationprotectionaction.md)集合 | 使用应用程序标记文档应采取的特定操作的集合。 有关完整列表，请参阅[informationProtectionAction](informationprotectionaction.md) 。 |
| label                       | [labelDetails](labeldetails.md)                                          | 描述要应用的标签的详细信息的对象。                                                                                                                                          |
| responsibleSensitiveTypeIds | Guid 集合                                                          | 如果标签是自动分类的结果，请提供将导致返回的标签的敏感信息类型 Guid 的列表。                                         
## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applyLabelAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "actionSource": "String",
  "actions": [{"@odata.type": "microsoft.graph.informationProtectionAction"}],
  "label": {"@odata.type": "microsoft.graph.labelDetails"},
  "responsibleSensitiveTypeIds": ["Guid"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applyLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->