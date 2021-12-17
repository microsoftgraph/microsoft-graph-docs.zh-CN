---
title: 获取 meetingAttendanceReport
description: 获取联机会议的会议出席报告。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 89d94ea92be942ab35bf3a7e0bb4f85b4e7b9756
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545131"
---
# <a name="get-meetingattendancereport"></a>获取 meetingAttendanceReport

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取[onlineMeeting 的 meetingAttendanceReport。](../resources/meetingAttendanceReport.md) [](../resources/onlinemeeting.md) 每次联机会议结束时，都会为该会话生成一份与会者报告。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetingArtifact.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | OnlineMeetingArtifact.Read.All |

若要对此 API 使用应用程序权限，租户管理员必须创建应用程序访问策略，并授予用户权限。 这将授权策略中配置的应用代表该用户获取联机会议和/或联机会议项目 (请求路径中指定的用户 ID) 。 有关详细信息，请参阅 [允许应用程序代表用户访问联机会议](/graph/cloud-communication-online-meeting-application-access-policy)。

## <a name="http-request"></a>HTTP 请求

若要按 ID 获取具有委派 () 和应用 `/me` () `/users/{userId}` 报告：
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/attendanceReports/{reportId}
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports/{reportId}
```

若要获取具有委派访问权限的在线会议的最新会话的与会者报告， () `/me` 应用 () `/users/{userId}` 权限：
<!-- { "blockType": "ignored" }-->
```http
GET /me/onlineMeetings/{meetingId}/meetingAttendanceReport
GET /users/{userId}/onlineMeetings/{meetingId}/meetingAttendanceReport
```

> [!TIP]
>
>- `userId` 是 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中用户的对象 ID。 有关详细信息，请参阅 [允许应用程序代表用户访问联机会议](/graph/cloud-communication-online-meeting-application-access-policy)。
>- `meetingId`是 [onlineMeeting 对象的](../resources/onlinemeeting.md) **ID。**
>- `reportId`是 [meetingAttendanceReport 对象的](../resources/meetingAttendanceReport.md) **ID。**

> [!CAUTION]
>
>- 路径 `/meetingAttendanceReport` 已弃用。 今后，请使用 `/attendanceReports` 路径检索联机会议的会议出席报告。
>- 该 `/meetingAttendanceReport` 路径将保留在 beta 版中，实现向后兼容。 但是，若要获取相同的响应，您需要添加 `expand` 查询选项。 有关详细信息，请参阅可选 [查询参数](#optional-query-parameters) 部分。

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

> [!TIP]
> **attendanceRecords** 属性是默认情况下不返回的导航属性。 若要检索 **行中的 attendanceRecords，** 请使用 `$expand=attendanceRecords` 查询选项，如示例 [2 所示](#example-2-get-the-latest-attendance-report-for-an-online-meeting)。

## <a name="request-headers"></a>请求标头

| 名称            | 说明               |
| :-------------- | :------------------------ |
| Authorization   | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [meetingAttendanceReport](../resources/meetingAttendanceReport.md) 对象。

## <a name="example"></a>示例

### <a name="example-1-get-the-attendance-report-for-an-online-meeting-by-id"></a>示例 1：按 ID 获取联机会议的会议出席报告

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get-attendanceReport-by-id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports/2c2c2454-7613-4d6e-9c7c-4cf7a6cdce89?$expand=attendanceRecords
```

#### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "name": "get-attendanceReport-by-id",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/attendanceReports('c9b6db1c-d5eb-427d-a5c0-20088d9b22d7')",
  "id": "c9b6db1c-d5eb-427d-a5c0-20088d9b22d7",
  "totalParticipantCount": 1,
  "meetingStartDateTime": "2021-10-05T04:38:23.945Z",
  "meetingEndDateTime": "2021-10-05T04:43:49.77Z",
  "attendanceRecords": [
    {
      "emailAddress": "(email address)",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "(redacted)",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:52.2782182Z",
          "leaveDateTime": "2021-03-16T19:06:47.7218491Z",
          "durationInSeconds": 415
        },
        {
          "joinDateTime": "2021-03-16T19:09:23.9834702Z",
          "leaveDateTime": "2021-03-16T19:16:31.1381195Z",
          "durationInSeconds": 427
        },
        {
          "joinDateTime": "2021-03-16T19:20:27.7094382Z",
          "leaveDateTime": "2021-03-16T19:25:37.7121956Z",
          "durationInSeconds": 310
        }
      ]
    }
  ]
}
```

### <a name="example-2-get-the-latest-attendance-report-for-an-online-meeting"></a>示例 2：获取联机会议的最新与会者报告

以下示例显示请求获取联机会议的最新会话的会议出席报告。

#### <a name="request"></a>请求

以下请求使用委派权限。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attendance_report"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attendance-report-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attendance-report-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attendance-report-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attendance-report-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-attendance-report-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

以下请求使用应用程序权限。
<!-- { "blockType": "ignored" }-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport
```

#### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport",
  "name": "get_attendance_report"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('dc74d9bb-6afe-433d-8eaa-e39d80d3a647')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy')/meetingAttendanceReport/$entity",
  "attendanceRecords": [
    {
      "emailAddress": "email address",
      "totalAttendanceInSeconds": 1558,
      "role": "Organizer",
      "identity": {
        "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:46.598956Z",
          "leaveDateTime": "2021-03-16T19:25:45.4473057Z",
          "durationInSeconds": 1558
        }
      ]
    },
    {
      "emailAddress": "email address",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "(redacted)",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:52.2782182Z",
          "leaveDateTime": "2021-03-16T19:06:47.7218491Z",
          "durationInSeconds": 415
        },
        {
          "joinDateTime": "2021-03-16T19:09:23.9834702Z",
          "leaveDateTime": "2021-03-16T19:16:31.1381195Z",
          "durationInSeconds": 427
        },
        {
          "joinDateTime": "2021-03-16T19:20:27.7094382Z",
          "leaveDateTime": "2021-03-16T19:25:37.7121956Z",
          "durationInSeconds": 310
        }
      ]
    }
  ],
  "totalParticipantCount": 2
}
```
