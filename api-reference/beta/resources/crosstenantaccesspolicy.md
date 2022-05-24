---
title: crossTenantAccessPolicy 资源类型
description: 跨租户访问策略表示跨租户访问设置的目录中的基本策略。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: beea220ebf3a0b12e40e56997c236b82fcb5d2fe
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653537"
---
# <a name="crosstenantaccesspolicy-resource-type"></a>crossTenantAccessPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示跨租户访问设置的目录中的基本策略。

继承自 [tenantRelationshipAccessPolicyBase](../resources/tenantrelationshipaccesspolicybase.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 crossTenantAccessPolicy](../api/crosstenantaccesspolicy-get.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|读取 [crossTenantAccessPolicy 对象的](../resources/crosstenantaccesspolicy.md) 属性和关系。|
|[更新 crossTenantAccessPolicy](../api/crosstenantaccesspolicy-update.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|更新 [crossTenantAccessPolicy 对象的](../resources/crosstenantaccesspolicy.md) 属性。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| displayName | String | 跨租户访问策略的显示名称。 继承自 [policyBase](../resources/policybase.md)。|
| allowedCloudEndpoints | String collection | 用于指定组织要与哪些 Microsoft 云协作。 默认情况下，此值为空。 此字段支持的值为： `microsoftonline.com`和 `microsoftonline.us``partner.microsoftonline.cn`. |
| 定义 (已弃用)  | String | 跨租户访问策略的原始 JSON 定义。 **已弃用。请勿使用。**|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|默认|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|定义组织与外部Azure Active Directory组织的交互方式的默认配置。|
|合作 伙伴|[crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 集合|为外部Azure Active Directory组织定义特定于合作伙伴的配置。|

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
  "displayName": "String",
  "definition": "String",
  "allowedCloudEndpoints": ["String"]
}
```
