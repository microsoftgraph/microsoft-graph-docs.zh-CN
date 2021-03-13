---
title: externalDomainFederation 资源类型
description: externalDomainFederation 类型将已配置的标识提供程序标识为已连接组织的标识源的非租户域。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: df88fef22c2acb86cadcfaed9a8f5be25da70f9d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760986"
---
# <a name="externaldomainfederation-resource-type"></a>externalDomainFederation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。 `@odata.type`该值指示此类型将已配置的标识提供程序标识为已连接组织的标识 `#microsoft.graph.externalDomainFederation` 源的域。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| displayName |String | 标识源的名称，通常也是域名。 只读。 |
| domainName |String | 域名。 只读。 |
| issuerUri |String | 传入联盟的 issuerURI。 只读。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

以下是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalDomainFederation",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String",
  "issuerUri": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalDomainFederation resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


