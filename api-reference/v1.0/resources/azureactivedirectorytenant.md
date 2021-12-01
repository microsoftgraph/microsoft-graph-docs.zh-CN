---
title: azureActiveDirectoryTenant 资源类型
description: azureActiveDirectoryTenant 类型将另一Azure Active Directory租户标识为已连接组织的标识源。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 35c517d23b59756d59412e5b898e6b222cc0f8db
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242379"
---
# <a name="azureactivedirectorytenant-resource-type"></a>azureActiveDirectoryTenant 资源类型

命名空间：microsoft.graph


在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。 该值 `@odata.type` `#microsoft.graph.azureActiveDirectoryTenant` 指示此类型将另一Azure Active Directory租户标识为已连接组织的标识源。

创建新的[connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md)时，如果调用方在 identitySources 集合中提供 domainIdentitySource，并且域对应于 Azure Active Directory 租户的注册域，则创建的生成的 connectedOrganization 将具有包含[azureActiveDirectoryTenant](azureactivedirectorytenant.md)类型的单个成员的 identitySources 集合。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|租户的名称Azure Active Directory。 只读。 |
|tenantId|String|租户的 ID Azure Active Directory租户。 只读。 |

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
  "tenantId": "String",
  "displayName": "String"
}
```



