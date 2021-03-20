---
title: downgradeJustification 资源类型
description: 表示有关执行降级的原因的用户输入。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: bc7336469f93de9e6d2b07fe73df9dce2eafd47f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941797"
---
# <a name="downgradejustification-resource-type"></a>downgradeJustification 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关执行降级的原因的用户输入。 根据 Office 安全与合规中心中的标签策略配置，可能需要降级理由。

## <a name="properties"></a>属性

| 属性             | 类型    | 说明                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| isDowngradeJustified | Boolean | 指示降级是否两端对齐。                                              |
| justificationMessage | String  | 指明理由降级的消息。 该消息将显示在管理日志中。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.downgradeJustification",
  "baseType": null
}-->

```json
{
  "isDowngradeJustified": true,
  "justificationMessage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "downgradeJustification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

