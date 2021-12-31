---
title: auditUserIdentity 资源类型
description: 一个开放类型，表示用户身份的详细信息及其主租户信息。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fc3d4f2de96c878184d38ed3eae4bf795875e35f
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647215"
---
# <a name="audituseridentity-resource-type"></a>auditUserIdentity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个开放类型，表示用户身份的详细信息及其主租户信息。

继承自 [userIdentity](../resources/useridentity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|用户的显示名称。 继承自 [标识](../resources/identity.md)。|
|homeTenantId|String|对于用户登录，用户是租户的标识符。|
|homeTenantName|String|对于用户登录，用户是租户成员的名称。 仅在主租户已同意允许用户Azure AD租户内容时填充。|
|id|String|用户的唯一标识符。 继承自 [标识](../resources/identity.md)。|
|ipAddress|String|为Azure AD客户端检测到的 IP 地址。 继承自 [userIdentity](../resources/useridentity.md)。|
|userPrincipalName|String|用户的用户主体名称 (UPN) 。 继承自 [userIdentity](../resources/useridentity.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditUserIdentity",
  "baseType": "microsoft.graph.userIdentity",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditUserIdentity",
  "displayName": "String",
  "id": "String (identifier)",
  "ipAddress": "String",
  "userPrincipalName": "String",
  "homeTenantId": "String",
  "homeTenantName": "String"
}
```

