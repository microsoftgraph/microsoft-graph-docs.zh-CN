---
title: 使用 Microsoft Graph API 指定教育作业通知的默认频道
description: 使用 Microsoft Graph中的教育 API 指定Microsoft Teams作业通知的默认 **频道。**
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 927641417a3153eab398a31dee19255071a0937e
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443458"
---
# <a name="specify-the-default-channel-for-education-assignment-notifications-using-the-microsoft-graph-api"></a>使用 Microsoft Graph API 指定教育作业通知的默认频道

本文介绍如何使用 Microsoft Graph中的教育 API 来指定Microsoft Teams作业通知的默认 **频道。** 指定默认通道涉及到为 [educationAssignment](/graph/api/resources/educationassignment) 生成 **notificationChannelUrl** 字符串属性。 此属性的默认值为 `null`。

## <a name="prerequisites"></a>先决条件

生成属性之前，请确定工作分配对应的团队和频道名称。

若要确定该工作分配的团队，请在Teams左侧菜单中Teams，然后选择相应的团队。

![从导航元素中Teams的屏幕截图](./images/notificationchannel-team.png)

确定所选团队中相应的频道。

![在团队中选择的频道的屏幕截图](./images/notificationchannel-channel.png)

## <a name="build-the-notificationchannelurl-property-value"></a>生成 notificationChannelUrl 属性值

以下步骤介绍如何构建属性值。

### <a name="step-1---get-the-team-id-based-on-your-team-name"></a>步骤 1 - 根据团队名称获取团队 ID
若要查找团队 ID，请通过团队名称提出 GET 请求。 如果已有团队 ID，请跳过此步骤。

#### <a name="request-example"></a>请求示例
下面为请求示例。

```http
GET https://graph.microsoft.com/v1.0/teams?$filter=displayName eq 'English Fall ''21'
```

#### <a name="response-example"></a>响应示例
以下示例显示了相应的响应。

```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams",
    "@odata.count": 1,
    "value": [
        {
            "id": "72a7baec-c3e9-4213-a850-f62de0adad5f",
            "createdDateTime": null,
            "displayName": "English Fall '21",
            "description": "English Fall '21",
            "internalId": null,
            "classification": null,
            "specialization": null,
            "visibility": null,
            "webUrl": null,
            "isArchived": null,
            "isMembershipLimitedToOwners": null,
            "memberSettings": null,
            "guestSettings": null,
            "messagingSettings": null,
            "funSettings": null,
            "discoverySettings": null
        }
    ]
}
```

### <a name="step-2---get-the-channel-id-based-on-channel-name-and-team-id"></a>步骤 2 - 根据频道名称和团队 ID 获取频道 ID
使用上一步获取的团队 ID 和频道名称提出 GET 请求。 如果你已拥有频道 ID，请跳过此步骤。

#### <a name="request-example"></a>请求示例
下面为请求示例。

```http
GET https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels?$filter=displayName eq 'General'
```

#### <a name="response-example"></a>响应示例
以下示例显示了相应的响应。

```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('72a7baec-c3e9-4213-a850-f62de0adad5f')/channels",
    "@odata.count": 1,
    "value": [
        {
            "id": "19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2",
            "createdDateTime": "2021-08-25T12:33:49.124Z",
            "displayName": "General",
            "description": "English Fall '21",
            "isFavoriteByDefault": null,
            "email": "",
            "webUrl": "https://teams.microsoft.com/l/channel/19%3Ajb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1%40thread.tacv2/General?groupId=72a7baec-c3e9-4213-a850-f62de0adad5f&tenantId=b6338c92-533e-4f6d-a327-994263712399",
            "membershipType": "standard"
        }
    ]
}
```

### <a name="step-3---construct-the-value-for-the-notificationchannelurl-property"></a>步骤 3 - 构造 notificationChannelUrl 属性的值
使用下列格式生成 **notificationChannelUrl** 属性的值： 

> `https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}` 

将 和 `{team-id}` `{channel-id}` 占位符替换为下表中描述的值。

| 占位符 | 说明 | 示例 |
|:--|:--|:--|
| `{team-id}` | 步骤 1 中响应的团队 ID。 这是当前工作分配所属的团队。 | 72a7baec-c3e9-4213-a850-f62de0adad5f |
| `{channel-id}` | 步骤 2 中获取的响应正文中的项目 ID。 | 19：jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2 |

以下示例显示了基于 **此格式的 notificationChannelUrl** 。

```http
https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2
```

### <a name="step-4---assign-the-value-to-the-notificationchannelurl-property-for-the-assignment"></a>步骤 4 - 将值分配给分配的 notificationChannelUrl 属性

现在，你已成功生成 url，是时候将值分配给属性了。 可以通过更新 educationAssignment 或 **educationAssignmentDefaults** 资源来执行此操作。

#### <a name="example-1-update-an-educationassignment"></a>示例 1：更新 educationAssignment

##### <a name="request"></a>请求
下面展示了示例请求。

```http
PATCH https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/4679bc1b-90c5-45af-ae1a-d5357672ed39
Content-type: application/json

{
    "displayName": "Property update",
    "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2"
}
```

##### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments/$entity",
    "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
    "displayName": "Property update",
    "closeDateTime": null,
    "dueDateTime": "2021-09-10T00:00:00Z",
    "assignDateTime": null,
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "resourcesFolderUrl": null,
    "createdDateTime": "2021-09-03T23:57:14.6088791Z",
    "lastModifiedDateTime": "2021-09-04T15:01:35.3361649Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2",
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%224679bc1b-90c5-45af-ae1a-d5357672ed39%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
    "addToCalendarAction": "studentsAndPublisher",
    "addedStudentAction": "none",
    "id": "4679bc1b-90c5-45af-ae1a-d5357672ed39",
    "instructions": {
        "content": "Read chapter 5 and write your review",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 50
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
    },
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    }
}
```

#### <a name="example-2-update-educationassignmentdefaults"></a>示例 2：更新 educationAssignmentDefaults

##### <a name="request"></a>请求

``` http
PATCH https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentDefaults
Content-Type: application/json

{
  "addToCalendarAction": "studentsOnly",
  "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2"
}
```

##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentDefaults"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "addedStudentAction": "assignIfOpen",
  "addToCalendarAction": "studentsOnly",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/v1.0/teams/72a7baec-c3e9-4213-a850-f62de0adad5f/channels/19:jb2-ckDy2jONyW6ElO1phAVD5cTjuswYgoumI0oxrUw1@thread.tacv2"
}
```

## <a name="see-also"></a>另请参阅

* [更新 educationAssignmentDefaults](/graph/api/educationassignmentdefaults-update)
* [更新 educationAssignment](/graph/api/educationassignment-update)
