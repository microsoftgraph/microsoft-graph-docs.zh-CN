---
title: unifiedRoleManagementPolicyExpirationRule 资源类型
description: 一种派生自 unifiedRoleManagementPolicyRule 资源类型的类型，该类型定义角色可通过直接分配或激活资格) 分配给主体 (的最长持续时间。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: db7e7956598c27a10a5aab7f6810cf72202f8afd
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898551"
---
# <a name="unifiedrolemanagementpolicyexpirationrule-resource-type"></a>unifiedRoleManagementPolicyExpirationRule 资源类型

命名空间：microsoft.graph

一种派生自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 资源类型的类型，该类型定义角色可通过直接分配或通过激活 eligibili 分配给主体 (的最大持续时间

## <a name="methods"></a>方法

无。


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|规则的标识符。 继承自 [entity](../resources/entity.md)。|
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

