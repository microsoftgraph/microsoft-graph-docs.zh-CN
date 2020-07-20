---
title: displayNameLocalization 资源类型
description: 使管理员能够自定义在共享 Microsoft 365 体验中使用的字符串。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8ae6c62acfacfccd22cc9985386762a2f61a2bc7
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050854"
---
# <a name="displaynamelocalization-resource-type"></a>displayNameLocalization 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使管理员能够自定义在共享 Microsoft 365 体验中使用的字符串。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName   |String       | 如果存在，则此字段的值包含已为**languageTag**字段中存在的语言设置的**displayName**字符串。|
|languageTag   |String       | 提供在其中提供了**displayName**字段的语言的语言区域性代码和友好名称。                  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.displayNameLocalization",
  "baseType": null
}-->

```json
{
  "displayName": "string",
  "languageTag": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "displayNameLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
