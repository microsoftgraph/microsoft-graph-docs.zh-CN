---
title: teamwork： sendActivityNotificationToRecipients
description: 批量向多个用户发送活动源通知。
author: eddie-lee-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dc0135fcbd7508a435e562c4b2c96cf68da09124
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695679"
---
# <a name="teamwork-sendactivitynotificationtorecipients"></a>teamwork： sendActivityNotificationToRecipients

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

批量向多个用户发送活动源通知。 

有关发送通知的更多详细信息和执行此操作的要求，请参阅[发送Teams活动通知](/graph/teams-send-activityfeednotifications)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | TeamsActivity.Send                          |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用                            | TeamsActivity.Send                          |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /teamwork/sendActivityNotificationToRecipients
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

| 参数          | 类型                                                         | 描述                                                  |
| :----------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| topic              | [teamworkActivityTopic](../resources/teamworkactivitytopic.md) | 通知的主题。 指定正在讨论的资源。 |
| activityType       | String                                                       | 活动类型。 必须在[Teams应用清单](/microsoftteams/platform/overview)中声明这一点。 |
| chainId            | Int64                                                        | 可选。 用于重写以前的通知。 在后续请求中使用相同的 `chainId` 方法来重写上一个通知。 |
| previewText        | [itemBody](../resources/itembody.md)                         | 通知的预览文本。 Microsoft Teams将只显示前 150 个字符。 |
| templateParameters | [keyValuePair](../resources/keyvaluepair.md) 集合      | 在Teams[应用清单](/microsoftteams/platform/overview)中对应`activityType`的活动源条目中定义的模板变量的值。 |
| teamsAppId         | String                                                       | 可选。 Teams与通知关联的Teams应用的应用 ID。 用于在为同一收件人用户安装具有相同 Azure AD 应用 ID 的多个应用时消除安装的应用的歧义。 |
| recipients         | [teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md) 集合 | 通知的收件人。 仅支持 [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) 类型的收件人。 单个请求中有 100 个收件人的上限。 |

将 **主题** 属性的值设置为`entityUrl``source`：

- [teamsCatalogApp](../resources/teamscatalogapp.md)

## <a name="response"></a>响应

如果成功，此操作返回 `202 Accepted` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-notify-multiple-users-about-pending-finance-approval-requests"></a>示例 1：通知多个用户有关挂起的财务审批请求

以下示例演示如何批量向多个用户发送活动源通知。 此示例通知多个利益干系人有关挂起的财务审批请求。

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "teamwork_sendactivitynotificationtorecipients_1"
}
-->

``` http
POST https://graph.microsoft.com/beta/teamwork/sendActivityNotificationToRecipients
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipients": [
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "ab88234e-0874-477c-9638-d144296ed04f"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
        }
    ],
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": false
}
-->

``` http
HTTP/1.1 202 Accepted
```

### <a name="example-2-notify-multiple-users-about-an-event-using-a-custom-topic"></a>示例 2：使用自定义主题通知多个用户有关事件的信息

如果想要链接未由 Microsoft Graph 表示的方面，或者想要自定义名称，则可以设置该`text`名称的`topic`源并传入自定义值。 `webUrl` 使用 `topic` 源时是必需的 `text`。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "teamwork_sendactivitynotificationtorecipients_2"
}
-->

``` http
POST https://graph.microsoft.com/beta/teamwork/sendActivityNotificationToRecipients
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "deploymentApprovalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ],
    "recipients": [
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "ab88234e-0874-477c-9638-d144296ed04f"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
        }
    ]
}
```

---


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": false
}
-->


``` http
HTTP/1.1 202 Accepted
```
