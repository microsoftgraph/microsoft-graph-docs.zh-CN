---
title: schedule： share
description: 与计划成员共享计划时间范围。
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ee2469ed3e8f534caf0b8cbb1e8b9c31541a032a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019648"
---
# <a name="schedule-share"></a>schedule： share

命名空间：microsoft.graph

与 [计划成员](../resources/schedule.md) 共享计划时间范围。
使指定团队成员[（](../resources/shift.md)包括员工[](../resources/openshift.md)和经理）可查看计划指定时间范围内班次、开放临时和[](../resources/schedule.md) [timeOff](../resources/timeoff.md)项目的集合。
计划[中的](../resources/shift.md)[每个班次、openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md) [实例都支持](../resources/schedule.md)草稿版本和项目的共享版本。 草稿版本仅由经理查看，而员工和经理可查看共享版本。 对于指定[](../resources/shift.md)时间范围内的每个班次[、openshift](../resources/openshift.md)和[timeOff](../resources/timeoff.md)实例，共享操作从草稿版本更新共享版本，以便除经理外，员工还可以查看有关项目的最新信息。 **notifyTeam** 参数进一步指定哪些员工可以查看项目。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Schedule.ReadWrite.All、Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Schedule.ReadWrite.All |

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
| notifyTeam            |`Boolean`             |指示整个团队是应收到此操作的可见通知，还是只收到分配有已共享的班次的员工。 必需。       |
| startDateTime         |`DateTimeOffset`   |按计划共享班次的开始时间。 必需。   |
| endDateTime           |`DateTimeOffset`   | 在计划前共享班次的结束时间。   |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/share
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-share-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>响应

下面展示了示例响应。 

<!-- {
  "blockType": "response",
  "truncated": true
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

