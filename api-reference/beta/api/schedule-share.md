---
title: 日程安排：共享
description: 与 schedule 成员共享计划时间范围。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5fce02b8f18a2745b06d1782ecadb7bc7bd3adc0
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44154239"
---
# <a name="schedule-share"></a>日程安排：共享

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与 schedule 成员共享[计划](../resources/schedule.md)时间范围。
在指定的团队成员（包括员工和经理）可查看的[日程安排](../resources/schedule.md)的指定时间范围内，创建[shift](../resources/shift.md)、 [openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md)项目的集合。
[计划](../resources/schedule.md)中的每个[shift](../resources/shift.md)、 [openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md)实例都支持项目的草稿版本和共享版本。 草稿版本仅由经理查看，并且共享版本可供员工和经理查看。 对于每个[shift](../resources/shift.md)、 [openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md)实例在指定的时间范围内，共享操作将从草稿版本更新共享版本，因此，除了经理之外，员工还可以查看有关该项目的最新信息。 **NotifyTeam**参数会进一步指定哪些员工可以查看该项目。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | 计划的所有写。 * |

>\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。

> **注意**：此 API 支持管理员权限。 全局管理员可以访问他们不是其成员的组。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.  |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

|参数                   |类型           |说明  |
|-----------------------|-------------------|--------------|
| notifyTeam            |`Boolean`             |指示整个团队是否应获取有关此操作的可见通知，或仅获取已分配有班次的员工。 必填。       |
| startDateTime         |`DateTimeOffset`   |共享日程上的班次的开始时间。 必填。   |
| endDateTime           |`DateTimeOffset`   | 在日程上共享班次的结束时间。   |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Shares a time-range of the schedule with the schedule members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
