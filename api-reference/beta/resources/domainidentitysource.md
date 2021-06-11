---
title: domainIdentitySource 资源类型
description: domainIdentitySource 类型将非租户域标识为已连接组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2c558213b7198da65eaacdbf0ac42915f3638c56
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896170"
---
# <a name="domainidentitysource-resource-type"></a>domainIdentitySource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。 `@odata.type`该值 `#microsoft.graph.domainIdentitySource` 指示此类型将域标识为已连接组织的标识源。

创建新的[connectedOrganization](../api/connectedorganization-post.md)时，如果调用方在 identitySources 集合中提供 domainIdentitySource，并且域对应于 Azure Active Directory 租户的注册域，则创建的生成的 connectedOrganization 将具有包含[azureActiveDirectoryTenant](azureactivedirectorytenant.md)类型的单个成员的 identitySources 集合。

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


