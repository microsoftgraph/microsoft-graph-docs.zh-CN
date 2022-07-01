---
title: crossTenantAccessPolicy 资源类型
description: 跨租户访问策略表示跨租户访问设置的目录中的基本策略。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2fb0f51f661938a3ee25edb4519fd5e8bc16987b
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604636"
---
# <a name="crosstenantaccesspolicy-resource-type"></a>crossTenantAccessPolicy 资源类型

命名空间：microsoft.graph

表示跨租户访问设置的目录中的基本策略。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 crossTenantAccessPolicy](../api/crosstenantaccesspolicy-get.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|读取 [crossTenantAccessPolicy 对象的](../resources/crosstenantaccesspolicy.md) 属性和关系。|
|[更新 crossTenantAccessPolicy](../api/crosstenantaccesspolicy-update.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|更新 [crossTenantAccessPolicy 对象的](../resources/crosstenantaccesspolicy.md) 属性。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| displayName | String | 跨租户访问策略的显示名称。 继承自 [policyBase](../resources/policybase.md)。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|默认|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|定义组织如何与外部 Azure Active Directory 组织交互的默认配置。|
|合作 伙伴|[crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 集合|为外部 Azure Active Directory 组织定义特定于合作伙伴的配置。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicy",
  "baseType": "microsoft.graph.tenantRelationshipAccessPolicyBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicy",
  "displayName": "String"
}
```
