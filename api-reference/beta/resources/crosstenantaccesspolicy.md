---
title: crossTenantAccessPolicy 资源类型
description: 跨租户访问策略表示跨租户访问设置的目录中的基本策略。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicy-resource-type"></a>crossTenantAccessPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示跨租户访问设置的目录中的基本策略。

继承自 [tenantRelationshipAccessPolicyBase](../resources/tenantrelationshipaccesspolicybase.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 crossTenantAccessPolicy](../api/crosstenantaccesspolicy-get.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|读取 [crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md) 对象的属性和关系。|
|[更新 crossTenantAccessPolicy](../api/crosstenantaccesspolicy-update.md)|[crossTenantAccessPolicy](../resources/crosstenantaccesspolicy.md)|更新 [crossTenantAccessPolicy 对象](../resources/crosstenantaccesspolicy.md) 的属性。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| displayName | String | 跨显示名称访问策略的组。 继承自 [policyBase](../resources/policybase.md)。|
| lastModifiedDateTime | DateTimeOffset | 上次修改跨租户访问策略的时间表示为使用 ISO 8601 格式且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
| 定义 (弃)  | String | 跨租户访问策略的原始 JSON 定义。 **已弃用。请勿使用。**|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|default|[crossTenantAccessPolicyConfigurationDefault](../resources/crosstenantaccesspolicyconfigurationdefault.md)|定义组织与外部组织之间的交互方式的默认Azure Active Directory配置。|
|合作伙伴|[crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) 集合|为外部组织定义特定于合作伙伴Azure Active Directory配置。|

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
  "lastModifiedDateTime": "String (timestamp)",
  "definition": "String"
}
```
