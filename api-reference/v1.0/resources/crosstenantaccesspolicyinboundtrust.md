---
title: crossTenantAccessPolicyInboundTrust 资源类型
description: 定义要通过跨租户访问策略配置从其他组织接受的条件访问声明。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fef57d6a1ae940677d7d5412838223618d9aae66
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604628"
---
# <a name="crosstenantaccesspolicyinboundtrust-resource-type"></a>crossTenantAccessPolicyInboundTrust 资源类型

命名空间：microsoft.graph

定义要通过跨租户访问策略配置从其他 Azure AD 组织接受的条件访问声明。 这些配置可以在默认配置、特定于合作伙伴的配置中进行配置，也可以在两者中进行配置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| isCompliantDeviceAccepted | Boolean | 指定是否信任来自外部 Azure AD 组织的合规设备。 |
| isHybridAzureADJoinedDeviceAccepted | 布尔 | 指定是否信任外部 Azure AD 组织中加入混合 Azure AD 的设备。 |
| isMfaAccepted | 布尔 | 指定外部 Azure AD 组织中的 MFA 是否受信任。|

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
