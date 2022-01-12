---
title: 删除 externalMeetingRegistrant
description: 从联机会议中删除 externalMeetingRegistrant。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9699a08517a2b4be495671abb76de00b0204f2e5
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860015"
---
# <a name="delete-externalmeetingregistrant"></a>删除 externalMeetingRegistrant

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会议组织者从启用了[externalMeetingRegistration](../resources/externalmeetingregistrant.md)的联机会议中删除[externalMeetingRegistrant。](../resources/externalmeetingregistration.md)

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetings.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | OnlineMeetings.ReadWrite.All |

若要对此 API 使用应用程序权限，租户管理员必须创建应用程序[](/graph/cloud-communication-online-meeting-application-access-policy)访问策略，并授予用户授权策略中配置的应用，以代表该用户 (代表该用户获取联机会议和/或联机会议项目，请求路径) 中指定了用户 ID。

## <a name="http-request"></a>HTTP 请求

若要删除具有委派权限的外部会议 () `/me` 应用程序 () `/users/{userId}/` 权限：

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onlineMeetings/{meetingId}/registration/registrants/{registrantId}
DELETE /users/{userId}/onlineMeetings/{meetingId}/registration/registrants/{registrantId}
```

> [!TIP]
>
> - `userId`是会议组织者的 **objectId。**
> - `meetingId`是 [onlineMeeting 对象的](../resources/onlinemeeting.md) **ID。**
> - `registrantId`是 [externalMeetingRegistrant 对象的](../resources/externalmeetingregistrant.md) **ID。**

## <a name="request-headers"></a>请求标头

| 名称            | 说明               |
| :-------------- | :------------------------ |
| Authorization   | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法仅返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "delete-externalregistratrant"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants/9d96988d-a66a-46ce-aad7-0b245615b297
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "name": "delete-externalregistratrant"
}-->

```http
HTTP/1.1 204 No Content
```
