---
title: delegatedAdminRelationshipCustomerParticipant 资源类型
description: 表示委派管理员关系中客户的标识详细信息。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 738ae13f0a999cecc7d1b24bb5ef2fec81302441
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589592"
---
# <a name="delegatedadminrelationshipcustomerparticipant-resource-type"></a>delegatedAdminRelationshipCustomerParticipant 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示委派管理员关系中客户的标识详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|客户显示名称设置的客户租户Azure AD。 只读|
|tenantId|String|客户Azure AD的已分配租户 ID。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipCustomerParticipant"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipCustomerParticipant",
  "tenantId": "String",
  "displayName": "String"
}
```

