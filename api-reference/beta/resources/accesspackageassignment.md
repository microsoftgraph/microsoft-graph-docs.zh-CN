---
title: accessPackageAssignment 资源类型
description: 访问包分配是一种在一段时间内向特定主题分配访问包。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b394efdd7ac2cbc97ff1245af4e0d01d4392e3f4
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650620"
---
# <a name="accesspackageassignment-resource-type"></a>accessPackageAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD管理](entitlementmanagement-overview.md)中，访问包分配是一个在一段时间内向特定主题分配访问包。  例如，访问包分配可以说明在 2019 年 1 月到 2019 年 7 月期间，用户 Alice 已通过访问包 Sales 获得访问权限。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignments](../api/entitlementmanagement-list-accesspackageassignments.md) | [accessPackageAssignment](accesspackageassignment.md) 集合 | 检索 **accessPackageAssignment 对象** 的列表。 |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合|检索在登录用户上筛选的 **accessPackageAssignment** 对象列表。|
| [重新处理](../api/accesspackageassignment-reprocess.md) | 无 | 自动重新计算和强制执行特定访问包的用户分配。|

> [!NOTE]
> 若要为用户创建或删除访问包分配，请使用 [create an accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md)

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageId|String|访问包的标识符。 只读。|
|assignmentPolicyId|String|访问包分配策略的标识符。 只读。|
|assignmentState|String|访问包分配的状态。 可能的值是 `Delivering` 、 `Delivered` 或 `Expired` 。 只读。 支持 `$filter`（`eq`）。|
|assignmentStatus|String|有关分配生命周期详细信息。  可能的值包括 `Delivering` `Delivered` 、、 `NearExpiry1DayNotificationTriggered` 或 `ExpiredNotificationTriggered` 。  只读。|
|catalogId|String|包含访问包的目录的标识符。 只读。|
|expiredDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|id|String| 只读。|
|isExtended|Boolean|指示是否已扩展访问包分配。 只读。|
|targetId|String| 工作分配的主题 ID。 只读。|
|schedule|[requestSchedule](requestschedule.md)| 当访问分配就位时。 只读。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| 只读。 可为 NULL。 支持 `$filter` `eq` () **id** 属性和 `$expand` 查询参数进行查询。|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| 只读。 可为 NULL。 支持 `$filter` `eq` () **id** 属性上显示|
|accessPackageAssignmentResourceRoles|[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合| 为此分配的目标用户传递的资源角色。 只读。 可为 NULL。|
|target|[accessPackageSubject](accesspackagesubject.md)| 访问包分配的主题。 只读。 可为 NULL。 支持 `$expand`。 支持 `$filter` `eq` () **对象 Id 上的属性**。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "keyProperty": "id"
}-->

```json
{
   "id":"9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
   "catalogId":"cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
   "accessPackageId":"e3f47362-993f-4fcb-8a38-532ffca16150",
   "assignmentPolicyId":"63ebd106-8116-40e7-a0ab-01ae475d11bb",
   "targetId":"ab4291f6-66b7-42bf-b597-a05b29414f5c",
   "assignmentStatus":"ExpiredNotificationTriggered",
   "assignmentState":"Expired",
   "isExtended":false,
   "expiredDateTime":"2019-04-25T23:45:40.42Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
