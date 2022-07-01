---
title: tenantRelationshipAccessPolicyBase 资源类型
description: 定义租户关系的基础类型。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d7fb506e09c88de18eb22153bc3608514ef19177
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604643"
---
# <a name="tenantrelationshipaccesspolicybase-resource-type"></a>tenantRelationshipAccessPolicyBase 资源类型

命名空间：microsoft.graph

定义租户关系的基础类型。 这是由跨租户策略对象（包括 [crossTenantAccessPolicy](crosstenantaccesspolicy.md)）继承的抽象类型。

继承自 [policyBase](policybase.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| 定义 (已弃用)  | String collection | 跨租户访问策略的原始 JSON 定义。 **已弃用。请勿使用。** |
| 说明 | String | 此策略的说明。 必需。 继承自 [policyBase](../resources/policybase.md)。 |
| displayName | String collection | 此策略的显示名称。 必需。 继承自 [policyBase](../resources/policybase.md)。 |

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
