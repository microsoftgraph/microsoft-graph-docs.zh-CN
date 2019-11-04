---
title: recommendLabelAction 资源类型
description: 表示一个标签，应根据敏感信息类型向用户推荐针对该文件的应用程序。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f2a872c0aa64eb79e0b8755ddc6b3788f14055
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939374"
---
# <a name="recommendlabelaction-resource-type"></a>recommendLabelAction 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个标签，应根据所发现的敏感信息类型向用户推荐针对该文件的应用程序。 如果 Microsoft 信息保护标记策略设置为 "**推荐**" 和 "标签"，而不是 "强制" 标签，则[evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)可能会返回**recommendLabelAction** 。 用户或 appliation 可以选择忽略或接受建议。 

## <a name="properties"></a>属性

| 属性                    | 类型                                                                     | 描述                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| actionSource                | String                                                                   | 可能的值是：`manual`、`automatic`、`recommended`、`default`。 |
| actions                     | [informationProtectionAction](informationprotectionaction.md)集合 | 用户接受标签时要执行的操作。                                                                       |
| label                       | [labelDetails](labeldetails.md)                                          | 建议使用的标签。                                                                      |
| responsibleSensitiveTypeIds | Guid 集合                                                          | 导致提供建议的敏感信息类型 Guid。                                                                      |

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
