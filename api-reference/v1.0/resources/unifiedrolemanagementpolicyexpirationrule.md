---
title: unifiedRoleManagementPolicyExpirationRule 资源类型
description: 一种派生自 unifiedRoleManagementPolicyRule 资源类型的类型，该类型定义角色可通过直接分配或激活资格) 分配给主体 (的最大持续时间。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2a48a9b84090b0d241e310ec4f8eada07e538d1d
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134024"
---
# <a name="unifiedrolemanagementpolicyexpirationrule-resource-type"></a>unifiedRoleManagementPolicyExpirationRule 资源类型

命名空间：microsoft.graph

一种派生自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 资源类型的类型，该类型定义角色可通过直接分配或激活资格) 分配给主体 (的最长持续时间。

## <a name="methods"></a>方法

无。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|规则的标识符。 继承自 [entity](../resources/entity.md)。|
|isExpirationRequired|Boolean|指示是否需要过期，或者它是永久活动分配还是资格。 |
|maximumDuration|期限| 资格或分配所允许的最长持续时间不是永久性的。 如果 **isExpirationRequired** 为 .，则 `true`为必需。 |
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|定义过期规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。 支持 `$filter`（`eq`、`ne`）。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isExpirationRequired": "Boolean",
  "maximumDuration": "String (duration)"
}
```

