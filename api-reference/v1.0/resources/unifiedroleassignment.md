---
title: unifiedRoleAssignment 资源类型
description: 一角色分配是角色定义与特定作用域的主体之间的链接，用于授予访问权限。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: fd6323fa0eb99f440551916cbc535fa64a359275
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148502"
---
# <a name="unifiedroleassignment-resource-type"></a>unifiedRoleAssignment 资源类型

命名空间：microsoft.graph

A 角色分配 is used to grant access to resources. 它表示分配给主体角色的角色 (例如，用户或角色可分配组) 作用域。

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|[列出 unifiedRoleAssignments](../api/rbacapplication-list-roleassignments.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md) 集合| 获取 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象及其属性的列表。|
|[创建 unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|创建新的 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。|
|[获取 unifiedRoleAssignment](../api/unifiedroleassignment-get.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|读取 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象的属性和关系。|
|[删除 unifiedRoleAssignment](../api/unifiedroleassignment-delete.md)|无|删除 [unifiedRoleAssignment](../resources/unifiedroleassignment.md) 对象。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 对象的唯一角色分配。 键，不可为 null，只读。 继承自 [实体](entity.md)。|
|roleDefinitionId|String| 分配所针对的角色定义的标识符。 只读。 支持 $filter (`eq` `in` 、) 。|
|principalId|String| 分配授予的主体的标识符。 支持 $filter (`eq` `in` 、) 。|
|directoryScopeId|String|表示工作分配范围的目录对象的标识符。  此属性或 **appScopeId** 是必需的。 工作分配的范围决定了已授予主体访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。 支持 $filter (`eq` `in` 、) 。|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。  此属性或 **directoryScopeId** 是必需的。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定目录对象，例如管理单元。 支持 $filter (`eq` `in` 、) 。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|principal|[directoryObject](directoryobject.md)| 引用分配的主体。 只读。 支持 `$expand`。|
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|分配用于的 roleDefinition。  支持 `$expand`。 roleDefinition.Id 自动展开。
|directoryScope|[directoryObject](directoryobject.md)|分配范围的目录对象。 只读。 支持 `$expand`。|
|appScope|[appScope](appscope.md)|只读属性，当分配范围特定于应用时，具有特定于应用的范围的详细信息。 包含实体。 支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "id": "String (identifier)",
  "appScopeId": "String",
  "condition": "String",
  "directoryScopeId": "String",
  "principalId": "String",
  "roleDefinitionId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
