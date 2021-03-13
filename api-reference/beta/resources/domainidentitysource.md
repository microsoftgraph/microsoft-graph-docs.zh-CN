---
title: domainIdentitySource 资源类型
description: domainIdentitySource 类型将非租户域标识为已连接组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ae616c98b2ca20ec4e5d9c7aceeba5bdeb538e81
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759662"
---
# <a name="domainidentitysource-resource-type"></a>domainIdentitySource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。 `@odata.type`该值 `#microsoft.graph.domainIdentitySource` 指示此类型将域标识为已连接组织的标识源。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| displayName |String | 标识源的名称，通常也是域名。 只读。 |
| domainName |String | 域名。 只读。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

以下是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


