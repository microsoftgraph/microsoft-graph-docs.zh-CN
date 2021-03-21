---
title: recommendLabelAction 资源类型
description: 表示应建议用户根据敏感信息类型向文件应用的标签。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 10d3ac687605ab648cdd3d68d6a3721c8fba2e30
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962572"
---
# <a name="recommendlabelaction-resource-type"></a>recommendLabelAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示应建议用户根据发现的敏感信息类型向文件应用的标签。 如果 Microsoft 信息保护标签策略设置为推荐和标签，而不是强制执行标签，[则 evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)可能会返回 **recommendLabelAction。**  用户或应用可以选择忽略或接受建议。 

## <a name="properties"></a>属性

| 属性                    | 类型                                                                     | 说明                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| actionSource                | String                                                                   | 可能的值是：`manual`、`automatic`、`recommended`、`default`。 |
| actions                     | [informationProtectionAction](informationprotectionaction.md) 集合 | 用户接受标签时要采取的操作。                                                                       |
| label                       | [labelDetails](labeldetails.md)                                          | 建议的标签。                                                                      |
| responsibleSensitiveTypeIds | Guid 集合                                                          | 导致给出建议的敏感信息类型 GUID。                                                                      |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recommendLabelAction",
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
  "description": "recommendLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


