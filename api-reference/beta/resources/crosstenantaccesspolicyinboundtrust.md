---
title: crossTenantAccessPolicyInboundTrust 资源类型
description: 定义您希望通过跨租户访问策略配置接受其他组织的条件访问声明。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyinboundtrust-resource-type"></a>crossTenantAccessPolicyInboundTrust 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义您希望通过跨租户访问策略配置接受Azure AD组织的条件访问声明。 可以在默认配置和/或特定于合作伙伴的配置中配置这些配置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| isCompliantDeviceAccepted | Boolean | 指定是否信任来自外部组织的Azure AD设备。 |
| isHybridAzureADJoinedDeviceAccepted | Boolean | 指定是否信任Azure AD外部Azure AD加入的设备的混合设备。 |
| isMfaAccepted | 布尔 | 指定是否信任来自外部Azure AD MFA。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyInboundTrust"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyInboundTrust",
  "isMfaAccepted": "Boolean",
  "isCompliantDeviceAccepted": "Boolean",
  "isHybridAzureADJoinedDeviceAccepted": "Boolean"
}
```
