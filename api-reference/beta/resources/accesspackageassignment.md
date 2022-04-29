---
title: accessPackageAssignment 资源类型
description: 访问包分配是在一段时间内将访问包分配给特定主题。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0c7ad4cd5ac58f2fea227a2fdb84cfc938797446
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133382"
---
# <a name="accesspackageassignment-resource-type"></a>accessPackageAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD权利管理](entitlementmanagement-overview.md)中，访问包分配是在一段时间内分配给特定主题的访问包。  例如，访问包分配可以说明在 2019 年 1 月至 2019 年 7 月期间，用户 Alice 已通过访问包 Sales 分配访问权限。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignments](../api/entitlementmanagement-list-accesspackageassignments.md) | [accessPackageAssignment](accesspackageassignment.md) 集合 | 检索 **accessPackageAssignment 对象的** 列表。 |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合|检索已登录用户上筛选的 **accessPackageAssignment** 对象的列表。|
| [重新处理](../api/accesspackageassignment-reprocess.md) | 无 | 自动重新评估并强制执行特定访问包的用户分配。|
| [additionalAccess](../api/accesspackageassignment-additionalaccess.md) [accessPackageAssignment](../resources/accesspackageassignment.md) 集合|检索分配到不兼容访问包的用户的 **accessPackageAssignment** 对象列表。|

> [!NOTE]
> 若要为用户创建或删除访问包分配，请使用 [创建 accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md)

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageId|String|访问包的标识符。 只读。|
|assignmentPolicyId|String|访问包分配策略的标识符。 只读。|
|assignmentState|String|访问包分配的状态。 可能的值为`Delivering`或 `Delivered``Expired`. 只读。 支持 `$filter`（`eq`）。|
|assignmentStatus|String|有关分配生命周期的详细信息。  可能的值包括`Delivering`、`Delivered`或 `NearExpiry1DayNotificationTriggered``ExpiredNotificationTriggered`。  只读。|
|catalogId|String|包含访问包的目录的标识符。 只读。|
|expiredDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|id|String| 只读。|
|isExtended|Boolean|指示访问包分配是否已扩展。 只读。|
|targetId|String| 具有分配的主题的 ID。 只读。|
|schedule|[requestSchedule](requestschedule.md)| 当访问分配到位时。 只读。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| 只读。 可为 NULL。 支持 `$filter` 对 `eq` **id** 属性和 `$expand` 查询参数 () 。|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| 只读。 可为 NULL。 支持 `$filter` **id 属性上的** (`eq`) |
|accessPackageAssignmentResourceRoles|[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合| 为此分配传递给目标用户的资源角色。 只读。 可为 NULL。|
|target|[accessPackageSubject](accesspackagesubject.md)| 访问包分配的主题。 只读。 可为 NULL。 支持 `$expand`。 支持 `$filter` **objectId** 上的 (`eq`) 。 |

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
