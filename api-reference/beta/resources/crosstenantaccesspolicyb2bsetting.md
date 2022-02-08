---
title: crossTenantAccessPolicyB2BSetting 资源类型
description: 定义用于 B2B 协作的入站Azure Active Directory (Azure AD) 出站规则集。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyb2bsetting-resource-type"></a>crossTenantAccessPolicyB2BSetting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义用于 B2B 协作的入站Azure Active Directory (Azure AD) 出站规则集。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|应用程序|[crossTenantAccessPolicyTargetConfiguration](../resources/crosstenantaccesspolicytargetconfiguration.md)|以跨租户访问策略为目标的应用程序列表。|
|usersAndGroups|[crossTenantAccessPolicyTargetConfiguration](../resources/crosstenantaccesspolicytargetconfiguration.md)|针对跨租户访问策略的用户和组的列表。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyB2BSetting",
  "usersAndGroups": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyTargetConfiguration"
  },
  "applications": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyTargetConfiguration"
  }
}
```
