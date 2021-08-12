---
title: permissionGrantPolicy 资源类型
description: 指定可授权许可的条件。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 379496e1d13012bf31e67109ab7c405e20d7ebd2c1149f323448e9fa15faff41
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126380"
---
# <a name="permissiongrantpolicy-resource-type"></a>permissionGrantPolicy 资源类型

命名空间：microsoft.graph

用于指定许可授予条件的权限授予策略。

权限授予策略由 **包括** 条件集列表和 **排除** 条件集列表组成。 要使事件与权限授予策略相匹配，它必须与 *至少一个***包括** 条件集匹配，并且 *不与任何***排除** 条件集匹配。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出权限授予策略](../api/permissiongrantpolicy-list.md) | [permissionGrantPolicy](permissiongrantpolicy.md) 集合 | 检索 permissionGrantPolicy 对象列表。 |
|[创建权限授予策略](../api/permissiongrantpolicy-post-permissiongrantpolicies.md)| [permissionGrantPolicy](permissiongrantpolicy.md) | 创建新的 permissionGrantPolicy 对象。 |
|[Get permission grant policy](../api/permissiongrantpolicy-get.md) | [permissionGrantPolicy](permissiongrantpolicy.md) |读取 permissionGrantPolicy 对象的属性和关系。|
|[更新权限授予策略](../api/permissiongrantpolicy-update.md) | [permissionGrantPolicy](permissiongrantpolicy.md)  |更新 permissionGrantPolicy 对象。 |
|**包括条件集**| | |
|[列出包括条件集](../api/permissiongrantpolicy-list-includes.md) |[permissionGrantConditionSet](permissiongrantconditionset.md) 集合| 获取已 *包括* 在此权限授予策略中的条件集。|
|[添加包括条件集](../api/permissiongrantpolicy-post-includes.md) |[permissionGrantConditionSet](permissiongrantconditionset.md) | 从此权限授予策略中添加 *已包括* 的条件集。 |
|[删除包括条件集](../api/permissiongrantpolicy-delete-includes.md) | 无 | 删除已从此权限授予策略中 *排除* 的条件集。|
|**排除条件集**| | |
|[列出排除条件集](../api/permissiongrantpolicy-list-excludes.md) |[permissionGrantConditionSet](permissiongrantconditionset.md) 集合| 获取已从此权限授予策略中 *排除* 的条件集。|
|[添加排除条件集](../api/permissiongrantpolicy-post-excludes.md) |[permissionGrantConditionSet](permissiongrantconditionset.md) | 添加已从此权限授予策略中 *排除* 的条件集。 |
|[删除排除条件集](../api/permissiongrantpolicy-delete-excludes.md) | 无 | 删除已从此权限授予策略中 *排除* 的条件集。|

## <a name="properties"></a>属性

| 属性     | 类型 |说明|
|:---------------|:--------|:----------|
| id | String | 权限授予策略的唯一标识符。 **id** 前缀`microsoft-`保留用于内置权限授予策略，不能在自定义权限授予策略中使用。 仅允许使用字母、数字、连字符 (`-`) 和下划线 (`_`)。 键。 不可为 null。 创建时为必需项。 不可变。 |
| displayName | String |权限授予策略的显示名称。|
| 说明 |String| 权限授予策略的描述。|
| 包括 | [permissionGrantConditionSet](permissiongrantconditionset.md) 集合| 已 *包括* 在此权限授予策略中的条件集。 在 `GET` 时自动展开。|
| 排除 |[permissionGrantConditionSet](permissiongrantconditionset.md) 集合| 已从此权限授予策略中 *排除* 的条件集。 在 `GET` 时自动展开。|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|包括|[permissionGrantConditionSet](permissiongrantconditionset.md) 集合| 已 *包括* 在此权限授予策略中的条件集。 执行 GET 操作时将自动展开此导航。 |
|排除|[permissionGrantConditionSet](permissiongrantconditionset.md) 集合| 已从此权限授予策略中 *排除* 的条件集。 执行 GET 操作时将自动展开此导航。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
}-->

```json
{
  "id": "string (identifier)",
  "displayName": "string",
  "description": "string",
  "includes": "collection(microsoft.graph.permissionGrantConditionSet)",
  "excludes": "collection(microsoft.graph.permissionGrantConditionSet)"
}
```
