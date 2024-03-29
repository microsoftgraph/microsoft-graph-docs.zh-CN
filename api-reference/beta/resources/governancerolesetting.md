---
title: governanceRoleSetting 资源类型
description: 表示每个角色定义上的一组配置，这些配置在创建或修改角色分配时需要对其进行评估。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: d5e441b35cd4b6ccdb52710508bd8afe5955d860
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399466"
---
# <a name="governancerolesetting-resource-type"></a>governanceRoleSetting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

表示每个角色定义上的一组配置，这些配置在创建或修改角色分配时需要对其进行评估。 例如，角色设置可能包括“最大分配持续时间”规则、“激活时所需的 MFA”规则等。

## <a name="methods"></a>方法

| 方法          | 返回类型 |Description|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | [governanceRoleSetting](../resources/governancerolesetting.md) 集合|列出资源上的角色设置集合。|
|[Get](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |读取角色设置的属性和关系。|
|[更新](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |更新角色设置对象。 |

## <a name="properties"></a>属性
|属性               |类型                                      |说明|
|:--------------------|:---------------------------------------|:----------|
|id                   |字符串                                  |roleSetting 的 ID。|
|resourceId           |String                                  |必填。 与角色设置关联的资源的 ID。|
|roleDefinitionId     |字符串                                  |必填。 与角色设置关联的角色定义的 ID。|
|isDefault            |Boolean                                 |只读。 指示 roleSetting 是否为默认 roleSetting|
|lastUpdatedDateTime  |DateTimeOffset                          |只读。 上次更新角色设置的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|lastUpdatedBy        |String                                  |只读。 上次更新 roleSetting 的管理员的显示名称。|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) 集合|管理员尝试添加符合条件的角色分配时评估的规则设置。|
|adminMemberSettings  |[governanceRuleSetting](../resources/governancerulesetting.md) 集合|管理员尝试添加直接成员角色分配时评估的规则设置。|
|userEligibleSettings |[governanceRuleSetting](../resources/governancerulesetting.md) 集合|当用户尝试添加符合条件的角色分配时评估的规则设置。 此设置目前不受支持。|
|userMemberSettings   |[governanceRuleSetting](../resources/governancerulesetting.md) 集合|当用户尝试激活其角色分配时评估的规则设置。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|资源|[governanceResource](../resources/governanceresource.md)|只读。 此角色设置的关联资源。|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|只读。 使用此角色设置强制执行的角色定义。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "suppressions": []
}
-->


