---
title: delegatedAdminRelationshipCustomerParticipant 资源类型
description: 表示委派管理关系中客户的标识详细信息。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 228681c0ade8f7b0db7ad3901e402049288cefd7
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704422"
---
# <a name="delegatedadminrelationshipcustomerparticipant-resource-type"></a>delegatedAdminRelationshipCustomerParticipant 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示委派管理关系中客户的标识详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|按Azure AD设置的客户租户的显示名称。 只读|
|tenantId|字符串|客户租户Azure AD分配的租户 ID。|

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

