---
title: 更新 onlineMeeting
description: 更新联机会议的属性。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 728c6bf9c6ae4cee619abca7f7d3a592585473c1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023224"
---
# <a name="update-onlinemeeting"></a>更新 onlineMeeting

命名空间：microsoft.graph

更新指定的 [onlineMeeting 对象](../resources/onlinemeeting.md) 的属性。

请参阅 [请求正文](#request-body) 部分，了解支持更新的属性列表。

## <a name="permissions"></a>权限

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | OnlineMeetings.ReadWrite                    |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | OnlineMeetings.ReadWrite.All                |

若要对此 API 使用应用程序权限，租户管理员必须创建应用程序[](/graph/cloud-communication-online-meeting-application-access-policy)访问策略，并授予用户授权策略中配置的应用，以代表该用户 (使用请求路径) 中指定的用户 ID 更新联机会议。

## <a name="http-request"></a>HTTP 请求

若要使用具有委派权限的会议 ID 更新指定的 **onlineMeeting， ()** `/me` 应用 () `/users/{userId}/` 权限：
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
>
> - `userId` 是 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中用户的对象 ID。 有关详细信息，请参阅应用程序 [访问策略](/graph/cloud-communication-online-meeting-application-access-policy)。
> - `meetingId`是 [onlineMeeting 对象的](../resources/onlinemeeting.md) **ID。**

## <a name="request-headers"></a>请求头

| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-type  | application/json. Required. |

## <a name="request-body"></a>请求正文

下表列出了可更新的属性。 在请求正文中，仅包括需要更新的属性，但以下例外：

- 调整联机会议开始或结束日期/时间始终需要请求正文中的 **startDateTime** 和 **endDateTime** 属性。
- **参与者** 属性的 **组织者** 字段无法更新。 创建会议后，无法修改会议的组织者。
- 调整 **参与者属性** 的 **attendees** 字段（如向会议添加或删除与会者）始终需要请求正文中与会者的完整列表。

最后一列指示更新此属性是否将生效进行中的会议。

| 属性                    | 类型                                                       | 说明                                                                         | 是否适用于进行中的会议？    |
|-----------------------------|------------------------------------------------------------|-------------------------------------------------------------------------------------|------------------------------|
| startDateTime               | 日期时间                                                   | 会议开始时间（UTC）。                                                      | 否                           |
| endDateTime                 | 日期时间                                                   | 会议结束时间（UTC）。                                                        | 否                           |
| subject                     | String                                                     | 联机会议的主题。                                                  | 否                           |
| participants                | [meetingParticipants](../resources/meetingparticipants.md) | 与联机会议关联的参与者。 仅与会者可以更新。 | 否                           |
| isEntryExitAnnounced        | 布尔                                                    | 呼叫者加入或离开时是否宣布。                              | 是                          |
| lobbyBypassSettings         | [lobbyBypassSettings](../resources/lobbyBypassSettings.md) | 指定哪些参与者可以绕过会议厅。                          | 是                          |
| allowedPresenters           | onlineMeetingPresenters                                    | 指定可在会议中成为演示者的人。                                      | 是 |
| allowAttendeeToEnableCamera | 布尔                                                    | 指示与会者是否可以打开其相机。                               | 是                          |
| allowAttendeeToEnableMic    | 布尔                                                    | 指示与会者是否可以打开其麦克风。                           | 是                          |
| allowMeetingChat            | meetingChatMode                                            | 指定会议聊天的模式。                                                 | 是                          |
| allowTeamworkReactions      | 布尔                                                    | 指示是否Teams会议的反应。                      | 是                          |

> [!NOTE]
>
>- 有关 **allowedPresenters** 和 **allowMeetingChat** 的可能值的列表，请参阅 [onlineMeeting](../resources/onlinemeeting.md)。
>- 将 **allowedPresenters** 的值更新为 时，在请求正文中包括指定与会者的角色设置为 `roleIsPresenter`  `presenter` 的完整与会者列表。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [onlineMeeting](../resources/onlinemeeting.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a>示例 1：更新 startDateTime、endDateTime 和 subject

#### <a name="request"></a>请求

> **注意：** 会议 ID 已缩短，可读。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-start-end-subject-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "role": "presenter",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"+1-900-555-0100",
      "tollFreeNumber":"+1-800-555-0100",
      "dialinUrl":"url"
   }
}
```

#### <a name="example-2-update-the-lobbybypasssettings"></a>示例 2：更新 lobbyBypassSettings
> **注意：** 会议 ID 已缩短，可读。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-lobbybypasssettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
    "creationDateTime":"2020-07-03T00:23:39.444642Z",
    "startDateTime":"2020-09-09T21:33:30.8546353Z",
    "endDateTime":"2020-09-09T22:03:30.8566356Z",
    "joinWebUrl":"(redacted)",
    "subject":"Patch Meeting Subject",
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                    "displayName": null,
                    "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                    "identityProvider": "AAD"
                }
            }
        },
        "attendees": [],
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


