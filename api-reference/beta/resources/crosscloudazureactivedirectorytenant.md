---
title: crossCloudAzureActiveDirectoryTenant 资源类型
description: crossCloudAzureActiveDirectoryTenant 类型将不同云中的另一个Azure Active Directory租户标识为已连接组织的标识源。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8086a5311626a520b96146205076b04547c0cfce
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694411"
---
# <a name="crosscloudazureactivedirectorytenant-resource-type"></a>crossCloudAzureActiveDirectoryTenant 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [connectedOrganization](connectedOrganization.md) 对象的标识源中使用。 该 `@odata.type` 值 `#microsoft.graph.crossCloudAzureActiveDirectoryTenant` 指示此类型将不同云中的另一个 Azure AD 租户标识为已连接组织的标识源。


## <a name="properties"></a>属性

| 属性                     | 类型                      | 描述 |
| :--------------------------- | :------------------------ | :---------- |
| cloudInstance | String | 租户所在的云的 ID、其中`microsoftonline.com``microsoftonline.us`一个或 `partner.microsoftonline.cn`。 只读。 |
| displayName |String | Azure Active Directory租户的名称。 只读。 |
| tenantId |字符串 | Azure Active Directory 租户 ID。 只读。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.crossCloudAzureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String",
  "cloudInstance": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "crossCloudAzureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


