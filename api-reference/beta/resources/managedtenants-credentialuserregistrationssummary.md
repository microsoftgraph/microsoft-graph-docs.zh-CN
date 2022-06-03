---
title: credentialUserRegistrationsSummary 资源类型
description: 表示给定托管租户的 Azure Active Directory 凭据用户注册摘要。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 587925f16ab66cb6870102078ad2f885731c4832
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883857"
---
# <a name="credentialuserregistrationssummary-resource-type"></a>credentialUserRegistrationsSummary 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示给定托管租户的 Azure Active Directory 凭据用户注册摘要。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 credentialUserRegistrationsSummaries](../api/managedtenants-managedtenant-list-credentialuserregistrationssummaries.md)|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) 集合|获取 [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) 对象及其属性的列表。|
|[获取 credentialUserRegistrationsSummary](../api/managedtenants-credentialuserregistrationssummary-get.md)|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|读取 [credentialUserRegistrationsSummary 对象的](../resources/managedtenants-credentialuserregistrationssummary.md) 属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此实体的唯一标识符。 必需项。 只读。|
|lastRefreshedDateTime|DateTimeOffset|上次在多租户管理平台中更新实体的日期和时间。 可选。 只读。|
|mfaAndSsprCapableUserCount|Int32|能够执行多重身份验证或自助密码重置的用户数。 可选。 只读。|
|mfaConditionalAccessPolicyState|String|强制执行多重身份验证的条件访问策略的状态。 可选。 只读。|
|mfaExcludedUserCount|Int32|多重身份验证排除安全组中的用户数 (Microsoft 365 Lighthouse - MFA 排除项) 。 可选。 只读。|
|mfaRegisteredUserCount|Int32|注册多重身份验证的用户数。 可选。 只读。|
|securityDefaultsEnabled|Boolean|指示是否启用标识安全默认值的标志。 可选。 只读。|
|ssprEnabledUserCount|Int32|为自助密码重置启用的用户数。 可选。 只读。|
|ssprRegisteredUserCount|Int32|注册自助服务密码重置的用户数。 可选。 只读。|
|tenantDisplayName|String|托管租户的显示名称。 必需项。 只读。|
|tenantId|String|托 [管租户](../resources/managedtenants-tenant.md)的 Azure Active Directory 租户标识符。 必需项。 只读。|
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
  "mfaExcludedUserCount": "Integer",
  "ssprEnabledUserCount": "Integer",
  "mfaRegisteredUserCount": "Integer",
  "ssprRegisteredUserCount": "Integer",
  "totalUserCount": "Integer",
  "securityDefaultsEnabled": "Boolean",
  "mfaConditionalAccessPolicyState": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
