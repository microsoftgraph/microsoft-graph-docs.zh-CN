---
title: displayNameLocalization 资源类型
description: 使管理员能够自定义共享体验中使用的Microsoft 365字符串。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a45c64d8cb80d94a702cfd4be57012949a7c86e3
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696532"
---
# <a name="displaynamelocalization-resource-type"></a>displayNameLocalization 资源类型

使管理员能够自定义共享体验中使用的Microsoft 365字符串。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName   |String       | 如果存在此参数，则此字段的值包含为 **languageTag** 字段中显示的语言设置的 **displayName** 字符串。|
|languageTag   |String       | 提供已在其中提供 **displayName** 字段的语言的语言区域性代码和友好名称。                  |

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


