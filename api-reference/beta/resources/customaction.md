---
title: customAction 资源类型
description: 表示标签可能提供的任何自定义操作（如果由管理员配置）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c71454a6647604d4155fc80c72ec48d22d85d03
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050008"
---
# <a name="customaction-resource-type"></a>customAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示标签可能提供的任何自定义操作（如果由管理员配置）。 自定义操作可能是通过 Office 365 安全与合规中心的 PowerShell 模块定义为 [informationProtectionLabel](informationProtectionLabel.md) 的一部分。 操作必须由使用中的应用程序理解。

## <a name="properties"></a>属性

| 属性   | 类型                                       | 说明                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| name       | String                                     | 自定义操作的名称。                           |
| properties | [keyValuePair](keyvaluepair.md) 集合 | 操作的属性（按键值对格式）。 |

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

