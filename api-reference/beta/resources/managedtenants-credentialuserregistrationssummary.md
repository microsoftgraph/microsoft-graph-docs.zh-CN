---
title: credentialUserRegistrationsSummary 资源类型
description: 表示给定托管Azure Active Directory的凭据用户注册的摘要。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 43a3f5cd39e8c151c71f976042e9bb33ae527dc4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402068"
---
# <a name="credentialuserregistrationssummary-resource-type"></a>credentialUserRegistrationsSummary 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示给定托管Azure Active Directory的凭据用户注册的摘要。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 credentialUserRegistrationsSummaries](../api/managedtenants-managedtenant-list-credentialuserregistrationssummaries.md)|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) 集合|获取 [credentialUserRegistrationsSummary 对象](../resources/managedtenants-credentialuserregistrationssummary.md) 及其属性的列表。|
|[获取 credentialUserRegistrationsSummary](../api/managedtenants-credentialuserregistrationssummary-get.md)|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|读取 [credentialUserRegistrationsSummary 对象的属性和](../resources/managedtenants-credentialuserregistrationssummary.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符。 必填。 只读。|
|lastRefreshedDateTime|DateTimeOffset|实体上次在多租户管理平台中更新的日期和时间。 可选。 只读。|
|mfaAndSsprCapableUserCount|Int32|能够执行多重身份验证或自助服务密码重置的用户数。 可选。 只读。|
|mfaConditionalAccessPolicyState|String|强制执行多重身份验证的条件访问策略的状态。 可选。 只读。|
|mfaRegisteredUserCount|Int32|注册多重身份验证的用户数。 可选。 只读。|
|securityDefaultsEnabled|布尔|一个标志，指示是否已启用标识安全性默认值。 可选。 只读。|
|ssprEnabledUserCount|Int32|启用自助服务密码重置的用户数。 可选。 只读。|
|ssprRegisteredUserCount|Int32|注册自助服务密码重置的用户数。 可选。 只读。|
|tenantDisplayName|String|托管显示名称租户的租户。 必填。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。 必填。 只读。|
|totalUserCount|Int32|给定托管租户中的用户总数。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "mfaAndSsprCapableUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
