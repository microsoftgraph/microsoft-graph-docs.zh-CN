---
title: conditionalAccessPolicy 资源类型
description: 表示 Azure Active Directory 条件访问策略。 条件访问策略是定义访问方案的自定义规则。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 990ddea3cdea724011d2a495b9c588aaf6a24215
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721691"
---
# <a name="conditionalaccesspolicy-resource-type"></a>conditionalAccessPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory 条件访问策略。 条件访问策略是定义访问方案的自定义规则。 有关详细信息，请参阅条件 [访问文档](/azure/active-directory/conditional-access/)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 conditionalAccessPolicies](../api/conditionalaccessroot-list-policies.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) 集合 | 获取组织的所有 conditionalAccessPolicies 对象。 |
| [创建 conditionalAccessPolicy](../api/conditionalaccessroot-post-policies.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | 创建新的 conditionalAccessPolicy 对象。 |
| [获取 conditionalAccessPolicy](../api/conditionalaccesspolicy-get.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | 读取 conditionalAccessPolicy 对象的属性和关系。 |
| [更新 conditionalAccessPolicy](../api/conditionalaccesspolicy-update.md) | [conditionalAccessPolicy](conditionalaccesspolicy.md) | 更新 conditionalAccessPolicy 对象。 |
| [删除 conditionalAccessPolicy](../api/conditionalaccesspolicy-delete.md) | 无 | 删除 conditionalAccessPolicy 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|conditions|[conditionalAccessConditionSet](conditionalaccessconditionset.md)| 指定应用策略时必须满足的规则。 必需。 |
|createdDateTime|DateTimeOffset| 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
|说明|String| 未使用。 |
|displayName|String| 指定显示名称AccessPolicy 对象的属性。 |
|grantControls|[conditionalAccessGrantControls](conditionalaccessgrantcontrols.md)| 指定传递策略必须实现的授予控制。 |
|id|String| 指定 conditionalAccessPolicy 对象的标识符。 只读。|
|modifiedDateTime| DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
|sessionControls|[conditionalAccessSessionControls](conditionalaccesssessioncontrols.md)| 指定登录后强制执行的会话控件。 |
|state|string| 指定 conditionalAccessPolicy 对象的状态。 可取值为：`enabled`、`disabled`、`enabledForReportingButNotEnforced`。 必填。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "keyProperty": "id"
}-->

```json
{
  "conditions": {"@odata.type": "microsoft.graph.conditionalAccessConditionSet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "grantControls": {"@odata.type": "microsoft.graph.conditionalAccessGrantControls"},
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)",
  "sessionControls": {"@odata.type": "microsoft.graph.conditionalAccessSessionControls"},
  "state": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
