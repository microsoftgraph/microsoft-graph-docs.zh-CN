---
title: 获取日程安排
description: 检索**schedule**对象的属性和关系。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fe5f2d72d43398893b366e4aa2632700df6649c6
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155171"
---
# <a name="get-schedule"></a>获取日程安排

命名空间：microsoft.graph

检索[schedule](../resources/schedule.md)对象的属性和关系。

计划创建过程符合[基于资源的长时间运行的操作（RELO）的一个 API 指南](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)。
当客户端使用[PUT 方法](team-put-schedule.md)时，如果设置了计划，该操作将更新计划;否则，该操作将在后台启动计划设置过程。

在计划设置过程中，客户端可以使用 GET 方法获取计划，并查看设置`provisionStatus`的当前状态的属性。 如果设置失败，客户端可以从`provisionStatusCode`属性获取其他信息。

客户端也可以检查计划的配置。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 请参阅 all、Group、Group. all、Schedule、Group、Group。所有    |
|委派（个人 Microsoft 帐户） | 不支持。    |s
|Application | Schedule. All、Schedule、All |

> **注意**：此 API 支持管理员权限。 全局管理员可以访问他们不是其成员的组。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法不支持 OData 查询参数来自定义响应。

## <a name="request-headers"></a>请求头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[schedule](../resources/schedule.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule
```
---


### <a name="response"></a>响应

下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
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
  "description": "Get the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
