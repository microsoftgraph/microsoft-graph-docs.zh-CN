---
title: accessPackageAssignment 资源类型
description: 访问包分配是一段时间内向特定主题分配访问包。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e188857a2cc92210d9298d588c7d411e16fb688a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720282"
---
# <a name="accesspackageassignment-resource-type"></a>accessPackageAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配是一段时间内向特定主题分配访问包。  例如，访问包分配可以说明，2019 年 1 月到 2019 年 7 月，用户 Alice 已通过访问包 Sales 分配访问权限。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignments](../api/accesspackageassignment-list.md) | [accessPackageAssignment](accesspackageassignment.md) 集合 | 检索 **accesspackageassignment 对象** 的列表。 |

>**注意：** 不能使用此方法创建或删除访问包分配。 相反，希望为用户请求访问包分配或者从用户中删除访问包分配的客户端可以创建[accessPackageAssignmentRequest。](../api/accesspackageassignmentrequest-post.md)

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageId|String|访问包的标识符。 只读。|
|assignmentPolicyId|String|访问包分配策略的标识符。 只读。|
|assignmentState|String|访问包分配的状态。 可能的值是 `Delivering` ， `Delivered` 或 `Expired` 。 只读。|
|assignmentStatus|String|有关分配生命周期详细信息。  可能的值包括 `Delivering` 、 `Delivered` 或 `NearExpiry1DayNotificationTriggered` `ExpiredNotificationTriggered` 。  只读。|
|catalogId|String|包含访问包的目录的标识符。 只读。|
|expiredDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|id|String| 只读。|
|isExtended|布尔|指示是否已扩展访问包分配。 只读。|
|targetId|String| 工作分配的主题的 ID。 只读。|
|schedule|[requestSchedule](requestschedule.md)| 访问分配何时就位。 只读。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| 只读。 可为 NULL。|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| 只读。 可为 NULL。|
|accessPackageAssignmentResourceRoles|[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合| 为此工作分配传递给目标用户的资源角色。 只读。 可为 NULL。|
|target|[accessPackageSubject](accesspackagesubject.md)| 访问包分配的主题。 只读。 可为 Null。|

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


