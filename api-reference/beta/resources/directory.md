---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4eb1cbdcbf0a1256c2bf2bf0cec35479b8bbc2cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962621"
---
# <a name="directory-resource-type-deleted-items"></a>目录资源类型（已删除的项目）

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示目录中已删除的项目。 删除某个项目后，它会被添加到已删除项目“容器”中。 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。

目前，仅应用程序、组和用户资源支持已删除的项目[](application.md)功能。 [](group.md) [](user.md)

## <a name="methods"></a>Methods

| 方法         | 返回类型 | 说明 |
|:---------------|:------------|:------------|
|[Get deleted item](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | 获取已删除项目的属性。 |
|[Restore deleted item](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| 还原最近删除的项目。 |
|[List deleted items](../api/directory-deleteditems-list.md) |[directoryObject](directoryobject.md) 集合| 获取最近删除的项目列表。 |
|[Permanently delete an item](../api/directory-deleteditems-delete.md) | 无 | 永久删除项目。 |
|[列出用户拥有的已删除项目](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md) collection | 列出用户拥有的目录项。 |
|[列出 featureRolloutPolicies](../api/list-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) 集合 | 检索 featureRolloutPolicy 对象的列表。 |
|[创建 featureRolloutPolicy](../api/post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 创建新的 featureRolloutPolicy 对象。 |
| [获取 featureRolloutPolicy](../api/featurerolloutpolicy-get.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 检索 featurerolloutpolicy 对象的属性和关系。 |
| [更新 featureRolloutPolicy](../api/featurerolloutpolicy-update.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 更新 featurerolloutpolicy 对象的属性。 |
| [删除 featureRolloutPolicy](../api/featurerolloutpolicy-delete.md) | 无 | 删除 featureRolloutPolicy 对象。 |

## <a name="properties"></a>属性
| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 对象的唯一标识符；例如，12345678-9abc-def0-1234-56789abcde。 键。 不可为 null。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|DeletedItems|[directoryObject](directoryobject.md) 集合| 最近删除的项目。 只读。 可为 Null。|
|featureRolloutPolicies|[featureRolloutPolicy](featurerolloutpolicy.md) 集合| 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


