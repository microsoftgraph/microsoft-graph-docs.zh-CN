---
title: governanceRoleSetting 资源类型
description: " 规则，依此类推。"
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508165"
---
# <a name="governancerolesetting-resource-type"></a>governanceRoleSetting 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表一组在需要时创建或修改角色分配评估针对每个角色定义的配置。 例如，角色设置可能包括"最大工作分配持续时间"规则"MFA 上激活需要"规则，以及等。

## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | [governanceRoleSetting](../resources/governancerolesetting.md)集合|列出角色设置对资源的集合。|
|[Get](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |读取属性和角色设置的关系。|
|[Update](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |更新角色设置对象。 |

## <a name="properties"></a>属性
|属性               |类型                                      |说明|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |RoleSetting 的 id。|
|resourceId           |String                                  |必需。 与关联的角色设置资源的 id。|
|roleDefinitionId     |String                                  |必需。 角色设置相关联的角色定义 id。|
|isDefault            |Boolean                                 |只读。 指示 roleSetting 是否是默认 roleSetting|
|lastUpdatedDateTime  |DateTimeOffset                          |只读。 上次更新时间角色设置的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|lastUpdatedBy        |String                                  |只读。 显示上次更新时间 roleSetting 的管理员名称。|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md)集合|管理员尝试添加合格的角色分配时计算规则设置。|
|adminMemberSettings  |[governanceRuleSetting](../resources/governancerulesetting.md)集合|管理员尝试添加直接成员角色分配时计算规则设置。|
|userEligibleSettings |[governanceRuleSetting](../resources/governancerulesetting.md)集合|当用户尝试添加合格的角色分配时计算规则设置。 此时不支持的设置。|
|userMemberSettings   |[governanceRuleSetting](../resources/governancerulesetting.md)集合|当用户尝试激活其角色分配时计算规则设置。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|只读。 此角色设置关联的资源。|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 角色定义的强制执行与此角色设置。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
