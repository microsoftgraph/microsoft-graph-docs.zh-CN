---
title: 列出 meetingAttendanceReports
description: 获取联机会议与会者报告的列表。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b4585cd36fbbe3efed087b9538dacef18f9c9d2e
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225324"
---
# <a name="list-meetingattendancereports"></a>列出 meetingAttendanceReports

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [onlineMeeting 的 meetingAttendanceReport](../resources/meetingAttendanceReport.md) [对象列表](../resources/onlinemeeting.md)。 每次联机会议结束时，会生成该会话的与会者报告。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetingArtifact.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application | OnlineMeetingArtifact.Read.All |

若要对此 API 使用应用程序权限，租户管理员必须创建应用程序访问 [策略，并](/graph/cloud-communication-online-meeting-application-access-policy) 授予用户权限。 这将授权策略中配置的应用代表该用户获取联机会议和/或联机会议项目 (请求路径中指定的用户 ID) 。

## <a name="http-request"></a>HTTP 请求

若要获取具有委派权限的在线会议的所有与会者报告 () `/me` 应用 () `/users/{userId}` 权限：
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/attendanceReports
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports
```

> [!TIP]
>
>- `userId` 是 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中用户的对象 ID。 有关详细信息，请参阅应用程序 [访问策略](/graph/cloud-communication-online-meeting-application-access-policy)。
>- `meetingId`是 [onlineMeeting 对象的](../resources/onlinemeeting.md) **ID。**

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称            | 说明               |
| :-------------- | :------------------------ |
| Authorization   | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [meetingAttendanceReport](../resources/meetingAttendanceReport.md) 对象列表。

> [!TIP]
> **attendanceRecords** 属性在响应中为空。

## <a name="example"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-attendanceReports"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attendancereports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attendancereports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attendancereports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attendancereports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "name": "get-attendanceReports",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/attendanceReports",
  "value": [
    {
      "id": "c9b6db1c-d5eb-427d-a5c0-20088d9b22d7",
      "totalParticipantCount": 1,
      "meetingStartDateTime": "2021-10-05T04:38:23.945Z",
      "meetingEndDateTime": "2021-10-05T04:43:49.77Z",
      "attendanceRecords": []
    },
    {
      "id": "2c2c2454-7613-4d6e-9c7c-4cf7a6cdce89",
      "totalParticipantCount": 2,
      "meetingStartDateTime": "2021-10-04T23:13:31.658Z",
      "meetingEndDateTime": "2021-10-04T23:18:57.563Z",
      "attendanceRecords": []
    }
  ]
}
```
