---
title: crossTenantAccessPolicyTargetConfiguration 资源类型
description: 定义跨租户访问策略设置配置的目标。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5480a471a1114da710d9efaa859b7a6fbcb1749f
ms.sourcegitcommit: a30eea2fa59087088f50e58706b91c0eb5b7a802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66604577"
---
# <a name="crosstenantaccesspolicytargetconfiguration-resource-type"></a>crossTenantAccessPolicyTargetConfiguration 资源类型

命名空间：microsoft.graph

定义跨租户访问策略设置配置的目标。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| accessType| crossTenantAccessPolicyTargetConfigurationAccessType | 定义是允许还是阻止访问。 可能的值包括 `allowed`、`blocked`、`unknownFutureValue`。 |
|targets|[crossTenantAccessPolicyTarget](../resources/crosstenantaccesspolicytarget.md) 集合|指定是使用此规则以用户、组还是应用程序为目标。|

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
