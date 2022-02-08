---
title: crossTenantAccessPolicyTargetConfiguration 资源类型
description: 定义跨租户访问策略设置配置的目标。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
---

# <a name="crosstenantaccesspolicytargetconfiguration-resource-type"></a>crossTenantAccessPolicyTargetConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义跨租户访问策略设置配置的目标。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| accessType| crossTenantAccessPolicyTargetConfigurationAccessType | 定义是允许访问还是阻止访问。 可能的值包括 `allowed`、`blocked`、`unknownFutureValue`。 |
|targets|[crossTenantAccessPolicyTarget](../resources/crosstenantaccesspolicytarget.md) 集合|指定是否以具有此规则的用户、组或应用程序为目标。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyTargetConfiguration"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.crossTenantAccessPolicyTargetConfiguration",
  "accessType": "String",
  "targets": [
    {
      "@odata.type": "microsoft.graph.crossTenantAccessPolicyTarget"
    }
  ]
}
```
