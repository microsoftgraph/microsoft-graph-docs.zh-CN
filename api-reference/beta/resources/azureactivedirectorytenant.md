---
title: azureActiveDirectoryTenant 资源类型
description: azureActiveDirectoryTenant 类型将另一个 Azure Active Directory 租户标识为已连接组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: acd59c82f1968cbb161b74d1e7c1a551b6b2e397
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759907"
---
# <a name="azureactivedirectorytenant-resource-type"></a>azureActiveDirectoryTenant 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。 该值 `@odata.type` `#microsoft.graph.azureActiveDirectoryTenant` 指示此类型将另一个 Azure Active Directory 租户标识为已连接组织的标识源。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| displayName |String | Azure Active Directory 租户的名称。 只读。 |
| tenantId |String | Azure Active Directory 租户的 ID。 只读。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

以下是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "azureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


