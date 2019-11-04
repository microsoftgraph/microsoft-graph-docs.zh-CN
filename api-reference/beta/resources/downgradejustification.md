---
title: downgradeJustification 资源类型
description: 表示有关执行降级的原因的用户输入。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aacc32ac86df4eda087f49dbb3dca05a356e8080
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939423"
---
# <a name="downgradejustification-resource-type"></a>downgradeJustification 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关执行降级的原因的用户输入。 根据 Office 安全与合规中心中的标签策略配置，可能需要降级理由。

## <a name="properties"></a>属性

| 属性             | 类型    | 描述                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| isDowngradeJustified | Boolean | 指示降级是还是未两端对齐。                                              |
| justificationMessage | 字符串  | 指示降级的原因的消息。 该邮件将显示在 "管理日志" 中。 |

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