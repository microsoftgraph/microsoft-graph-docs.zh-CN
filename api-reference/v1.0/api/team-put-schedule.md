---
title: 创建或替换日程安排
description: 创建或替换 **schedule** 对象。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 84bad58447680f6c152c1490f1fe88727dd7803b1779b7c0f8ea952ed60fa90b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240608"
---
# <a name="create-or-replace-schedule"></a>创建或替换日程安排

命名空间：microsoft.graph

创建或替换 [schedule](../resources/schedule.md) 对象。

计划创建过程符合针对基于资源的长时间运行的操作的 One API 准则 ([RELO) 。 ](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)
当客户端使用 PUT 方法时，如果已设置计划，则操作将替换计划;否则，操作将在后台启动计划预配过程。

在计划预配期间，客户端可以使用 [GET 方法](schedule-get.md) 获取计划并查看 属性，了解 `provisionStatus` 预配的当前状态。 如果设置失败，客户端可以从 属性获取其他 `provisionStatusCode` 信息。

客户端还可以检查计划的配置。


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
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.  |

## <a name="request-body"></a>请求正文

在请求正文中，提供 schedule 对象的 JSON [表示](../resources/schedule.md) 形式。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/schedule.md) 代码和 schedule 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/v1/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```
---


### <a name="response"></a>响应

下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null,
  "timeClockEnabled": true,
  "openShiftsEnabled": true,
  "swapShiftsRequestsEnabled": true,
  "offerShiftRequestsEnabled": true,
  "timeOffRequestsEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates or replaces the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

