---
title: domainIdentitySource 资源类型
description: DomainIdentitySource 类型将非租户域标识为连接的组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 134f0ae3c382c879b48d468545dd40f2d6bd101b
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510156"
---
# <a name="domainidentitysource-resource-type"></a>domainIdentitySource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[connectedOrganization](connectedOrganization.md)的标识源中使用。 `@odata.type`该值 `#microsoft.graph.domainIdentitySource` 指示此类型将域标识为连接的组织的标识源。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| displayName |String | 标识源的名称，通常也是域名。 只读。 |
| domainName |String | 域名称。 只读。 |

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
