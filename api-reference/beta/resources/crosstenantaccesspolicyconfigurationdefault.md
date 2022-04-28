---
title: crossTenantAccessPolicyConfigurationDefault 资源类型
description: 为Azure AD B2B 协作和 B2B 直接连接的入站和出站设置定义的默认配置。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3fb4df32d047a695952a3ac0b91bb3188f90c190
ms.sourcegitcommit: e7cfc67ac8fa2ccf895ca7a8d5f640fb99237928
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65103012"
---
# <a name="crosstenantaccesspolicyconfigurationdefault-resource-type"></a>crossTenantAccessPolicyConfigurationDefault 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为Azure AD B2B 协作和 B2B 直接连接的入站和出站设置定义的默认配置。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md)|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|获取 B2B 协作和 B2B 直接连接入站和出站设置的默认配置。|
|[更新 crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-update.md)|无|更新 B2B 协作和 B2B 直接连接入站和出站设置的默认配置。|
|[重置为系统默认值](../api/crosstenantaccesspolicyconfigurationdefault-resettosystemdefault.md)|无|将跨租户访问策略的默认配置重置为系统默认设置。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| b2bCollaborationInbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |为通过Azure AD B2B 协作访问资源的其他组织的用户定义默认配置。 |
| b2bCollaborationOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |为组织中通过Azure AD B2B 协作出站访问其他组织中的资源的用户定义默认配置。 |
| b2bDirectConnectInbound  |[crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) | 为通过Azure AD B2B 直接连接访问资源的其他组织的用户定义默认配置。 |
| b2bDirectConnectOutbound | [crossTenantAccessPolicyB2BSetting](../resources/crosstenantaccesspolicyb2bsetting.md) |为组织中通过Azure AD B2B 直接连接出站访问其他组织中的资源的用户定义默认配置。 |
| inboundTrust | [crossTenantAccessPolicyInboundTrust](../resources/crosstenantaccesspolicyinboundtrust.md) | 确定用于信任来自外部Azure AD组织的其他条件访问声明的默认配置。 |
| isServiceDefault | Boolean | 如果 `true`将默认配置设置为系统默认配置。 如果 `false`已自定义默认设置。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationDefault",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyConfigurationDefault",
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
  "isServiceDefault": "Boolean"
}
```
