---
title: privateLinkDetails 资源类型
description: 提供有关租户中专用链接Azure AD详细信息
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8392b9a1a0e86a1f12a17d96c3fa7e8d06f7437b
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647222"
---
# <a name="privatelinkdetails-resource-type"></a>privateLinkDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供有关与登录事件关联的 Azure 专用链接的详细信息。 有关 Azure 专用链接详细信息，请参阅 [什么是 Azure 专用链接？](/azure/private-link/private-link-overview) 



## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|policyId|String|专用链接策略的唯一标识符。 |
|policyName|String|Azure AD 中专用链接策略的名称。 |
|policyTenantId|String|专用链接策略Azure AD租户的租户标识符。|
|resourceId|String|Azure 资源管理器 (ARM) 链接策略资源的路径。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.privateLinkDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privateLinkDetails",
  "policyId": "String",
  "policyName": "String",
  "resourceId": "String",
  "policyTenantId": "String"
}
```
