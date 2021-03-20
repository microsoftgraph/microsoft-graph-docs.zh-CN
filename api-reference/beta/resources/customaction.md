---
title: customAction 资源类型
description: 表示标签可能提供的任何自定义操作（如果由管理员配置）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1d9c88715cba6fc8faede1419b3c8809c3ec3f54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941804"
---
# <a name="customaction-resource-type"></a>customAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示标签可能提供的任何自定义操作（如果由管理员配置）。 可以通过 Office 365 安全与合规中心的 PowerShell 模块将自定义操作定义为 [信息ProtectionLabel](informationProtectionLabel.md) 的一部分。 使用应用程序必须理解这些操作。

## <a name="properties"></a>属性

| 属性   | 类型                                       | 说明                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| name       | String                                     | 自定义操作的名称。                           |
| properties | [keyValuePair](keyvaluepair.md) 集合 | 操作的属性，采用键值对格式。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "name": "String",
  "properties": [{"@odata.type": "microsoft.graph.keyValuePair"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

