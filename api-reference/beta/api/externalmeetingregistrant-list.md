---
title: 列出 externalMeetingRegistrants
description: 获取 onlineMeeting 的 externalMeetingRegistrants 列表。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c232d26a57481f0cab4542f8f769522bc75e9bc1
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565143"
---
# <a name="list-externalmeetingregistrants"></a>列出 externalMeetingRegistrants

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [onlineMeeting 的 externalMeetingRegistrants](../resources/externalmeetingregistrant.md) [列表](../resources/onlinemeeting.md)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetings.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | OnlineMeetings.ReadWrite.All |

若要对此 API 使用应用程序权限，租户管理员必须创建应用程序[](/graph/cloud-communication-online-meeting-application-access-policy)访问策略，并授予用户授权策略中配置的应用，以代表该用户 (代表该用户获取联机会议和/或联机会议项目，请求路径) 中指定了用户 ID。

## <a name="http-request"></a>HTTP 请求

若要获取具有委派权限的所有外部会议注册 () `/me` 应用程序 () `/users/{userId}/` 权限：

<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/registration/registrants
GET /users/{userId}/onlineMeetings{meetingId}/registration/registrants
```

> [!TIP]
>
>- `userId`是会议组织者的 **objectId。**
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

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [externalMeetingRegistrant](../resources/externalmeetingregistrant.md) 对象集合。 **joinWebUrl** 属性将为 `null` 。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "list-externalregistratrants"
}-->

```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
```

### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "name": "list-externalregistratrants",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalMeetingRegistrant",
  "isCollection": true
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants",
  "value": [
    {
        "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
        "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
        "joinWebUrl": null,
        "userId": null,
        "tenantId": null
    },
    {
        "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
        "id": "e264916d-f65d-48ec-9c04-c2107fd5b61f",
        "joinWebUrl": null,
        "userId": null,
        "tenantId": null
    }
  ]
}
```
