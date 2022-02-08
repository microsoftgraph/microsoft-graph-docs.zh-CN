---
title: crossTenantAccessPolicyConfigurationPartner 资源类型
description: 为 B2B 协作和 B2B 直接连接的入站和出站Azure AD定义的特定于合作伙伴的配置。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicyconfigurationpartner-resource-type"></a>crossTenantAccessPolicyConfigurationPartner 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为 B2B 和 B2B 直接连接协作的入站和出站Azure AD合作伙伴特定的配置。

对于任何特定于合作伙伴的属性，即 `null`，这些设置将继承在默认跨租户访问设置 [中配置的行为](../resources/crosstenantaccesspolicyconfigurationdefault.md)。

继承自 [crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
| [列出合作伙伴](../api/crosstenantaccesspolicy-list-partners.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 集合 | 获取所有特定于合作伙伴的配置的列表。 |
| [创建 crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicy-post-partners.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | 创建新的特定于合作伙伴的配置。 |
| [获取 crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-get.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | 读取特定于合作伙伴的配置设置。 |
| [更新 crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-update.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | 更新特定于合作伙伴的配置的属性。 |
| [删除 crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-delete.md) | None | 删除特定于合作伙伴的配置。 |

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为其他组织的用户定义合作伙伴特定的配置，这些用户通过 B2B 协作Azure AD你的资源。 继承自 [crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md)。 |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为贵组织中通过 B2B 协作出站访问另一个组织中资源Azure AD配置。 继承自 [crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md)。 |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为其他组织的用户定义合作伙伴特定的配置，这些用户通过 Azure B2B 直接连接访问你的资源。 继承自 [crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md)。 |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为贵组织中出站以通过 B2B 直接连接访问另一Azure AD合作伙伴特定的配置。 继承自 [crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md)。 |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | 确定用于信任来自外部组织的其他条件访问声明的合作伙伴Azure AD配置。 继承自 [crossTenantAccessPolicyConfigurationBase](../resources/crosstenantaccesspolicyconfigurationbase.md)。 |
| isServiceProvider | Boolean | 标识特定于合作伙伴的配置是否是组织的云服务提供商。 |
| tenantId | String | 合作伙伴组织的租户Azure AD标识符。 只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "baseType": "microsoft.graph.crossTenantAccessPolicyConfigurationBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "tenantId": "String",
  "inboundTrust": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyInboundTrust"
  },
  "b2bCollaborationOutbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bCollaborationInbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bDirectConnectOutbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "b2bDirectConnectInbound": {
    "@odata.type": "microsoft.graph.crossTenantAccessPolicyB2BSetting"
  },
  "isServiceProvider": "Boolean"
}
```
