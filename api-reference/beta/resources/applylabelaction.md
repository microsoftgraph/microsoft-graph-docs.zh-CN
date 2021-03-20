---
title: applyLabelAction 资源类型
description: 表示应用或更新标签时应该采取的一组操作。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e53a2796c7cd4f0b8c0a415ca4bc38ffefeb609e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945737"
---
# <a name="applylabelaction-resource-type"></a>applyLabelAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示应用或更新标签时应该采取的一组操作。 当标签评估操作的结果是应应用标签时，将返回 **applyLabelAction。** 属性 `actions` 包含[一个 informationProtectionAction](informationProtectionaction.md)集合，该集合描述要应用标签的完整操作集，包括删除旧元数据、内容标记和保护。

## <a name="properties"></a>属性

| 属性                    | 类型                                                                     | 说明                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| actionSource                | String                                                                   | 可能的值是：`manual`、`automatic`、`recommended`、`default`。                                                                                                                             |
| actions                     | [informationProtectionAction](informationprotectionaction.md) 集合 | 使用应用程序为文档添加标签时应执行的特定操作的集合。 有关[完整列表，请参阅 informationProtectionAction。](informationprotectionaction.md) |
| label                       | [labelDetails](labeldetails.md)                                          | 描述要应用的标签的详细信息的对象。                                                                                                                                          |
| responsibleSensitiveTypeIds | Guid 集合                                                          | 如果标签是自动分类的结果，则提供导致返回标签的敏感信息类型 GUID 列表。                                         
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

