---
title: crossTenantAccessPolicyConfigurationPartner 资源类型
description: 为Azure AD B2B 协作和 B2B 直接连接的入站和出站设置定义的特定于合作伙伴的配置。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 73849d18cce7639e82e5b56a37f46ce7705b707f
ms.sourcegitcommit: e7cfc67ac8fa2ccf895ca7a8d5f640fb99237928
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65103030"
---
# <a name="crosstenantaccesspolicyconfigurationpartner-resource-type"></a>crossTenantAccessPolicyConfigurationPartner 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为Azure AD B2B 和 B2B 直接连接协作的入站和出站设置定义的特定于合作伙伴的配置。

对于任何特定于合作伙伴的属性， `null`这些设置将继承在 [默认跨租户访问设置](../resources/crosstenantaccesspolicyconfigurationdefault.md)中配置的行为。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
| [列出合作伙伴](../api/crosstenantaccesspolicy-list-partners.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 集合 | 获取所有特定于合作伙伴的配置的列表。 |
| [创建 crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicy-post-partners.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | 创建新的特定于合作伙伴的配置。 |
| [获取 crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-get.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | 读取特定于合作伙伴的配置设置。 |
| [更新 crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-update.md) | [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) | 更新特定于合作伙伴的配置的属性。 |
| [删除 crossTenantAccessPolicyConfigurationPartner](../api/crosstenantaccesspolicyconfigurationpartner-delete.md) | 无 | 删除特定于合作伙伴的配置。 |

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为通过Azure AD B2B 协作访问资源的其他组织的用户定义特定于合作伙伴的配置。 |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为组织中通过Azure AD B2B 协作出站访问其他组织中的资源的用户定义特定于合作伙伴的配置。 |
| b2bDirectConnectInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为通过 Azure B2B 直接连接访问资源的其他组织的用户定义特定于合作伙伴的配置。 |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为组织中通过Azure AD B2B 直接连接出站访问其他组织中的资源的用户定义特定于合作伙伴的配置。 |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | 确定特定于合作伙伴的配置，以便信任外部Azure AD组织中的其他条件访问声明。 |
| isServiceProvider | Boolean | 标识特定于合作伙伴的配置是否为组织的云服务提供商。 |
| tenantId | 字符串 | 合作伙伴Azure AD组织的租户标识符。 只读。 键。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "tenantId",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationPartner",
  "tenantId": "String (identifier)",
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
