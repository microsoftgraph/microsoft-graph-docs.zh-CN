---
title: domainIdentitySource 资源类型
description: domainIdentitySource 类型将非租户域标识为已连接组织的标识源。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6fe969759e07e14af08d3d69e90726dce8512445
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242343"
---
# <a name="domainidentitysource-resource-type"></a>domainIdentitySource 资源类型

命名空间：microsoft.graph


在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。 `@odata.type`该值 `#microsoft.graph.domainIdentitySource` 指示此类型将域标识为已连接组织的标识源。

创建新的[connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md)时，如果调用方在 identitySources 集合中提供 domainIdentitySource，并且域对应于 Azure Active Directory 租户的注册域，则创建的生成的 connectedOrganization 将具有包含[azureActiveDirectoryTenant](azureactivedirectorytenant.md)类型的单个成员的 identitySources 集合。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|标识源的名称，通常也是域名。 只读。 |
|domainName|String|域名。 只读。 |

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainIdentitySource",
  "domainName": "String",
  "displayName": "String"
}
```

