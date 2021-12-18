---
title: 创建 externalMeetingRegistration
description: 为联机会议启用外部注册。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 98b919647ccc5bae5db22a62e7e1a31e621e8ef6
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2021
ms.locfileid: "61565145"
---
# <a name="create-externalmeetingregistration"></a>创建 externalMeetingRegistration

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用外部注册系统 [启用 onlineMeeting](../resources/onlinemeeting.md) 的注册。 联机会议只能启用一个注册。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetings.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | OnlineMeetings.ReadWrite.All |

若要对此 API 使用应用程序权限，租户管理员必须创建应用程序[](/graph/cloud-communication-online-meeting-application-access-policy)访问策略，并授予用户授权策略中配置的应用代表该用户获取联机会议和/或联机会议项目 (请求路径) 中指定了用户 ID。

## <a name="http-request"></a>HTTP 请求

若要创建具有委派会议 () `/me` 应用程序 () `/users/{userId}/` 权限：

<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/{meetingId}/registration
POST /users/{userId}/onlineMeetings/{meetingId}/registration
```

> [!TIP]
>
>- `userId`是会议组织者的 **objectId。**
>- `meetingId`是 [onlineMeeting 对象的](../resources/onlinemeeting.md) **ID。**

## <a name="request-headers"></a>请求标头

| 名称            | 说明               |
| :-------------- | :------------------------ |
| Authorization   | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [externalMeetingRegistration](../resources/externalmeetingregistration.md) 对象的 JSON 表示形式。

> [!IMPORTANT]
> 必须提供 **@odata.type** 属性以指定注册类型。 有关详细信息，[请参阅以下示例。](#example)

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [externalMeetingRegistration](../resources/externalmeetingregistration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create-externalregistration",
  "@odata.type": "microsoft.graph.externalMeetingRegistration"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalMeetingRegistration",
  "allowedRegistrant": "everyone"
}
```

### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "name": "create-externalregistration",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalMeetingRegistration"
}-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/$entity",
  "@odata.type": "#microsoft.graph.externalMeetingRegistration",
  "id": "f23714a3-a2f4-4b1d-96d2-bfe9097e7163",
  "allowedRegistrant": "everyone"
}
```
