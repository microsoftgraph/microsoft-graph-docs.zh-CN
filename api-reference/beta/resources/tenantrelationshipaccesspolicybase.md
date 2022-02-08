---
title: tenantRelationshipAccessPolicyBase 资源类型
description: 定义租户关系的基类型。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="tenantrelationshipaccesspolicybase-resource-type"></a>tenantRelationshipAccessPolicyBase 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义租户关系的基类型。 这是跨租户策略对象（包括 [crossTenantAccessPolicy](crosstenantaccesspolicy.md)）继承的抽象类型。

继承自 [policyBase](policybase.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| 定义 (弃)  | 字符串集合 | 跨租户访问策略的原始 JSON 定义。 **已弃用。请勿使用。** |
| description | String | 此策略的说明。 必需。 继承自 [policyBase](../resources/policybase.md)。 |
| displayName | 字符串集合 | 此策略的显示名称。 必需。 继承自 [policyBase](../resources/policybase.md)。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantRelationshipAccessPolicyBase",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.tenantRelationshipAccessPolicyBase",
  "definition": [
    "String"
  ],
  "description": "String",
  "displayName": "String"
}
```
