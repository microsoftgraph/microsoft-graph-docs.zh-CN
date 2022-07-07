---
title: 创建 onlineMeeting
description: 代表请求正文中指定的用户创建联机会议。
author: mkhribech
ms.localizationpriority: high
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9ecd517798f7eb868a283b834dfe9c1f79cdee6a
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645512"
---
# <a name="create-onlinemeeting"></a>创建 onlineMeeting

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表用户创建联机会议。

> [!TIP]
> 此 API 创建与用户日历中任何事件均不关联的独立会议；因此，通过此 API 创建的会议将不会显示在用户的日历上。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）           |
| :------------------------------------- | :---------------------------------------------------- |
| 委派（工作或学校帐户）     | OnlineMeetings.ReadWrite                              |
| 委派（个人 Microsoft 帐户） | 不支持。                                        |
| 应用程序                            | OnlineMeetings.ReadWrite.All*                         |

要对此 API 使用应用程序权限，租户管理员必须创建一个 [应用程序访问策略](/graph/cloud-communication-online-meeting-application-access-policy)，并将其授予用户，以授权策略中配置的应用代表该用户创建联机会议（使用请求路径中指定的用户 ID）。

## <a name="http-request"></a>HTTP 请求

若要创建具有委派 (`/me`) 和应用 (`/users/{userId}`) 权限的联机会议，请执行以下操作：
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings
POST /users/{userId}/onlineMeetings
```

> [!NOTE]
>- `userId` 是 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中用户的对象 ID。 有关详细信息，请参阅 [允许应用程序代表用户访问联机会议](/graph/cloud-communication-online-meeting-application-access-policy)。

## <a name="request-headers"></a>请求标头

| 名称            | 说明                 |
| :-------------- | :-------------------------- |
| Authorization   | Bearer {token}。必需。   |
| Content-type    | application/json. Required. |
| Accept-Language | 语言。 可选。         |

如果请求包含 `Accept-Language` HTTP 标头，`joinInformation` 的 `content` 将采用 `Accept-Language` 标头中指定的语言和区域设置变量中。 默认内容将为英语。

## <a name="request-body"></a>请求正文
在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。

> [!CAUTION]
>
> 当前不支持将 `presenter` 或 `coorganizer` 角色分配给未在Azure Active Directory中注册的用户。 有关详细信息，请参阅 [已知问题](/graph/known-issues#presenter-role-cannot-be-assigned-to-non-azure-ad-participants) 以了解更多详细信息。

## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-create-an-online-meeting-with-user-token"></a>示例 1：使用用户令牌创建联机会议

#### <a name="request"></a>请求

请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-user-token"
}-->
```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User Token Meeting"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-user-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-user-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-user-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-onlinemeeting-user-token-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-onlinemeeting-user-token-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-onlinemeeting-user-token-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f46-17cc-42e7-854-f03d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+125254478",
    "tollFreeNumber": "+1663588",
    "ConferenceId": "24299",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-b8da330?id=24299"
  },
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMdFpHRTNaR1F6WGhyZWFkLnYy",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDl4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%22bf-8f1-4af-9b-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d51-3ec-8c-374f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373734f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d1db47",
          "displayName": "Mario Rogers"
        }
      },
      "role": "presenter",
      "upn": "upn-value"
    }
  },
  "subject": "User Token Meeting",
  "joinMeetingIdSettings": {
    "isPasscodeRequired": false,
    "joinMeetingId": "1234567890",
    "passcode": null
  }
}
```
>**注意：** 如果指定了 'Accept-Language: ja' 来指示日语，则响应将包括以下内容。

```json
    "joinInformation": {
        "content": "data%3Atext%2Fhtml%2C%0A++%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A%09+%3C%2Fdiv%3E%0A++++%3Cdiv+class%3D%22me-email-text%22+style%3D%22color%3A%23252424%3Bfont-family%3A'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3B%22%3E%0A+++%3Cdiv+style%3D%22margin-top%3A+24px%3B+margin-bottom%3A+10px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-headline%22%0A++++++++++++++style%3D%22font-size%3A+18px%3Bfont-family%3A'Segoe+UI+Semibold'%2C'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3Btext-decoration%3A+underline%3Bcolor%3A+%236264a7%3B%22%0A++++++++++++++href%3D%22https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%252279a788bf-86f1-41af-91ab-000000000000%2522%252c%2522Oid%2522%253a%2522d4a060b5-a8fc-450c-837b-000000000000%2522%257d%22%0A++++++++++++++target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3EMicrosoft+Teams+%E4%BC%9A%E8%AD%B0%E3%81%AB%E5%8F%82%E5%8A%A0%3C%2Fa%3E%0A++++++%3C%2Fdiv%3E%0A%09+%3Cdiv%3E%0A++++%0A++++++%3Cdiv%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+14px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22%0A++++++++++href%3D%22tel%3A%2B16477490000%2C%2C11160000%26%2335%3B+%22+target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3E%2B16477490000%3C%2Fa%3E%0A++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%26nbsp%3B++(%E6%9C%89%E6%96%99)+%3C%2Fspan%3E%0A++++++%3C%2Fdiv%3E%0A++++%0A++%3C%2Fdiv%3E%0A%0A%09+%0A++++++%3Cdiv+style%3D%22margin-top%3A+10px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++++++%E4%BC%9A%E8%AD%B0+ID%3A%0A++++++++%3C%2Fspan%3E%0A++++++%3Cspan+style%3D%22font-size%3A+14px%3B%22%3E%0A++++++++111+000+00%23%0A++++++%3C%2Fspan%3E%0A++++%3C%2Fdiv%3E%0A++++%0A%09+%0A++++++++%3Cdiv+style%3D%22margin-bottom%3A+24px%3B%22%3E%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fdialin.teams.microsoft.com%2F8bf6e654-57eb-4b85-aeaf-36c84429b2fe%3Fid%3D11160000%22+rel%3D%22noreferrer+noopener%22%3E%E6%9C%80%E5%AF%84%E3%82%8A%E3%81%AE%E5%9B%BD%E3%81%AE%E9%9B%BB%E8%A9%B1%E7%95%AA%E5%8F%B7%E3%82%92%E6%A4%9C%E7%B4%A2%3C%2Fa%3E%0A+++++++++%7C%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fmysettings.lync.com%2Fpstnconferencing%22+rel%3D%22noreferrer+noopener%22%3E%0A++++++++PIN+%E3%82%92%E3%83%AA%E3%82%BB%E3%83%83%E3%83%88%3C%2Fa%3E%0A+++++++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Faka.ms%2FJoinTeamsMeeting%22+rel%3D%22noreferrer+noopener%22%3ETeams+%E3%81%AE%E8%A9%B3%E7%B4%B0%E3%82%92%E8%A1%A8%E7%A4%BA%3C%2Fa%3E%0A+++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fteams.microsoft.com%2FmeetingOptions%2F%3ForganizerId%3Dd4a060b5-a8fc-450c-837b-000000000000%26tenantId%3D79a788bf-86f1-41af-91ab-000000000000%26threadId%3D19_meeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%40thread.v2%26messageId%3D0%26language%3Dja%22+rel%3D%22noreferrer+noopener%22%3E%E4%BC%9A%E8%AD%B0%E3%81%AE%E3%82%AA%E3%83%97%E3%82%B7%E3%83%A7%E3%83%B3%3C%2Fa%3E%0A++++%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%E3%83%93%E3%83%87%E3%82%AA%E4%BC%9A%E8%AD%B0%E3%83%87%E3%83%90%E3%82%A4%E3%82%B9%E3%81%A7%E5%8F%82%E5%8A%A0%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A12px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22%22%3E000000000%40t.abcd.vc%3C%2Fa%3E+VTC+%E4%BC%9A%E8%AD%B0+ID%3A+0180300000%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A+12px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22https%3A%2F%2Fdialin.abcd.vc%2Fteams%2F%3Fkey%3D000000000%26conf%3D0180308922%22%3E%E4%BB%A3%E6%9B%BF+VTC+%E3%81%AE%E3%83%80%E3%82%A4%E3%83%A4%E3%83%AB%E6%96%B9%E6%B3%95%3C%2Fa%3E%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++%0A++++++%3C%2Fdiv%3E%0A++++++%3Cdiv+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++%0A++++++%3C%2Fdiv%3E%0A++++%0A+++++%3C%2Fdiv%3E%0A%09+%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A++%3C%2Fdiv%3E%22%2C%0A",
        "contentType": "Html"
    }
```


### <a name="example-2-create-an-online-meeting-in-a-microsoft-teams-channel-with-a-user-token"></a>示例 2：使用用户令牌在 Microsoft Teams 频道中创建联机会议

#### <a name="request"></a>请求

请求示例如下所示。

>**注意：** 传递的用户令牌的对象 ID 应当是有效负载中由 **threadId** 表示的频道的成员。

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User meeting in Microsoft Teams channel.",
  "chatInfo": {
    "threadId":"19%3A3b5239894b776357c1dd79%40thread.skype"
  }
}
```
#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f40f86-17cc-42e7-85f4-f03880d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+12534478",
    "tollFreeNumber": "+18660588",
    "ConferenceId": "24229",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-49f-45b-bc69-b8a330?id=24229"
  },
  "chatInfo": {
    "threadId": "19%3A3b52398f3c5244b776357c1dd79%40thread.skype",
    "messageId": "1563302249053",
    "replyChainMessageId": null
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItHRTNaR1F6WGhyZWFkLnYy",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2288bf-86f1-41af-91ab-2011db47%22%2c%22Oid%22%3a%22fae72-d51-43ec-68c-3704f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "55ae72-d251-43ec-868c-373704f",
          "tenantId": "72f98f-86f1-41af-91ab-2d7db47",
          "displayName": "Mario Rogers"
        }
      },
      "role": "presenter",
      "upn": "upn-value"
    }
  },
  "subject": "User meeting in Microsoft Teams channel.",
  "joinMeetingIdSettings": {
    "isPasscodeRequired": false,
    "joinMeetingId": "1234567890",
    "passcode": null
  }
}
```

### <a name="example-3-create-a-microsoft-teams-live-event-with-a-user-token"></a>示例 3：使用用户令牌创建 Microsoft Teams 实时事件

#### <a name="request"></a>请求

请求示例如下所示。

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "subject":"User Token Live Event",
  "startDateTime":"2020-12-02T14:30:34.2444915+00:00",
  "endDateTime":"2020-12-02T15:00:34.2464912+00:00",
  "isBroadcast": true,
  "broadcastSettings": {
    "allowedAudience": "everyone",
    "isRecordingEnabled": true,
    "isAttendeeReportEnabled": true
  }
}
```

#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了可读性，此处显示的答复对象已缩短。 所有属性都将通过实际调用返回。

```json
{
  "id": "dc17674c-81d9-4adb-bfb2-8fa442e4622_19:meeting_MGQ4MDDYxODYzMmY2@thread.v2",
  "creationDateTime": "2020-12-02T14:30:34.2444915Z",
  "startDateTime": "2020-09-29T22:35:31.389759Z",
  "endDateTime": "2020-12-02T15:00:34.2464912Z",
  "joinWebUrl": "(redacted)",
  "subject": "User Token Live Event",
  "autoAdmittedUsers": "EveryoneInCompany",
  "isEntryExitAnnounced": true,
  "allowedPresenters": "organization",
  "videoTeleconferenceId": "(redacted)",
  "participants": {
    "organizer": {
      "upn": "(redacted)",
      "role": "producer",
      "identity": {
        "user": {
          "id": "dc174c-81d9-4adb-bfb2-8f6a4622",
          "displayName": null,
          "tenantId": "909581-5130-43e9-88f3-fccde38",
          "identityProvider": "AAD"
        }
      }
    },
    "attendees": [
      {
        "upn": "(redacted)",
        "role": "producer",
        "identity": {
          "user": {
            "id": "dc174c-81d9-4adb-bfb2-8442e4622",
            "displayName": null,
            "tenantId": "909581-5130-43e9-88f3-fcb3cde38",
            "identityProvider": "AAD"
          }
        }
      }
    ],
    "producers": [
      {
        "upn": "(redacted)",
        "role": "producer",
        "identity": {
          "user": {
            "id": "d7674c-81d9-4adb-bfb2-8f6a4622",
            "displayName": null,
            "tenantId": "909c81-5130-43e9-88f3-fcbcde38",
            "identityProvider": "AAD"
          }
        }
      }
    ],
    "contributors": []
  },
  "lobbyBypassSettings": {
    "scope": "organization",
    "isDialInBypassEnabled": false
  },
  "isBroadcast": true,
  "broadcastSettings": {
    "allowedAudience": "organization",
    "isRecordingEnabled": true,
    "isAttendeeReportEnabled": true
  },
  "joinMeetingIdSettings": {
    "isPasscodeRequired": false,
    "joinMeetingId": "1234567890",
    "passcode": null
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

### <a name="example-4-create-an-online-meeting-that-requires-a-passcode"></a>示例 4：创建需要密码的联机会议

以下示例演示如何向会议添加密码。 使用 **joinMeetingId** 加入会议时，将使用该密码。 有关详细信息，请参阅 [joinMeetingIdSettings](../resources/joinmeetingidsettings.md)。
#### <a name="request"></a>请求

请求示例如下所示。

>**注意:** 将自动生成密码，并且不支持自定义密码。

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User meeting",
  "joinMeetingIdSettings": {
    "isPasscodeRequired": true
  }
}
```

#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4086-17cc-42e7-85f4-f03880d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+12525478",
    "tollFreeNumber": "+18690588",
    "ConferenceId": "2999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22fa0-499f-435b-bc69-b8dea330?id=2999"
  },
  "chatInfo": {
    "threadId": "19%3A3b523985568b776357c1dd79%40thread.skype",
    "messageId": "15629053",
    "replyChainMessageId": null
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "MSpkYzE3Njc0Yy04MWQ5LTRhFpHRTNaR1F6WGhyZWFkLnYy",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3iMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%22f8bf-86f1-41af-91ab-2011db47%22%2c%22Oid%22%3a%20fae72-d251-43ec-86c-377304f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "5e72-d251-43ec-868c-3732704f",
          "tenantId": "72fbf-86f1-41af-91ab-2d71db47",
          "displayName": "Mario Rogers"
        }
      },
      "role": "presenter",
      "upn": "upn-value"
    }
  },
  "subject": "User meeting",
  "joinMeetingIdSettings": {
    "isPasscodeRequired": true,
    "joinMeetingId": "1234567890",
    "passcode": "123abc"
  }
}
```


### <a name="example-5-create-an-online-meeting-that-does-not-require-a-passcode"></a>示例 5：创建不需要密码的联机会议

当 **isPasscodeRequired** 设置为 `false` 或未在请求中指定 **joinMeetingIdSettings** 时，生成的联机会议将没有密码。
#### <a name="request"></a>请求

请求示例如下所示。

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User meeting in Microsoft Teams channel.",
  "joinMeetingIdSettings": {
    "isPasscodeRequired": false
  }
}
```

或

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User meeting in Microsoft Teams channel."
}
```

#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
    "messageId": "1563302249053",
    "replyChainMessageId": null
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Tyler Stein"
        }
      },
      "role": "presenter",
      "upn": "upn-value"
    }
  },
  "subject": "User meeting in Microsoft Teams channel.",
  "joinMeetingIdSettings": {
    "isPasscodeRequired": false,
    "joinMeetingId": "1234567890",
    "passcode": null
  }
}
```
