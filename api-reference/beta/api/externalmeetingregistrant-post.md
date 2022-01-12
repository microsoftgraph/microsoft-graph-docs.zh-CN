---
title: 创建 externalMeetingRegistrant
description: 注册外部会议注册人。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b5c3bb05638325778188fcb265cb33198988d0a8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61832451"
---
# <a name="create-externalmeetingregistrant"></a>创建 externalMeetingRegistrant

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在启用了[externalMeetingRegistration](../resources/externalmeetingregistrant.md)的联机会议中注册[externalMeetingRegistrant。](../resources/externalmeetingregistration.md) 会议组织者通过提供外部注册系统中的唯一 **ID** 来注册某人，并获取此注册表的唯一 **joinWebUrl。**

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetings.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | OnlineMeetings.ReadWrite.All |

若要对此 API 使用应用程序权限，租户管理员必须创建应用程序[](/graph/cloud-communication-online-meeting-application-access-policy)访问策略，并授予用户授权策略中配置的应用，以代表该用户 (代表该用户获取联机会议和/或联机会议项目，请求路径) 中指定了用户 ID。

## <a name="http-request"></a>HTTP 请求

若要创建具有委派权限的外部会议注册表 () `/me` 应用程序 () `/users/{userId}/` 权限：

<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/{meetingId}/registration/registrants
POST /users/{userId}/onlineMeetings/{meetingId}/registration/registrants
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

- 如果 [externalMeetingRegistration](../resources/externalmeetingregistration.md)对象的 **allowedRegistrant** 属性的值为 ，则提供外部注册系统的 `organization` **ID、** 注册表用户的 **tenantId** 和 **Azure Active Directory。**
- 如果 [externalMeetingRegistration](../resources/externalmeetingregistration.md)对象的 **allowedRegistrant** 属性的值为 ，则 `everyone` 仅提供外部注册系统的 ID。

> [!IMPORTANT]
>
>- 外部 **注册** 系统的 ID 可以是任何形式的字符串。
>- 必须提供 **@odata.type** 属性以指定注册表类型。 有关详细信息，[请参阅以下示例。](#examples)

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [externalMeetingRegistrant](../resources/externalmeetingregistrant.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-enroll-a-registrant-when-the-meeting-registration-has-allowedregistrant-set-to-everyone"></a>示例 1：当会议注册允许Registrant 设置为"所有人"时注册注册

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "add-externalregistratrant-public"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "9d96988d-a66a-46ce-aad7-0b245615b297"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "add-externalregistratrant-public",
  "@odata.type": "microsoft.graph.externalMeetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NjliNTYxNjktNzAwNi00OTlhLWFmMWEtMGZhY2JjZGM5NmEy%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%2216664f75-11dc-4870-bec6-38c1aaa81431%22%2c%22prid%22%3a%229d96988d-a66a-46ce-aad7-0b245615b297%22%2c%22isPublic%22%3atrue%7d",
  "userId": null,
  "tenantId": null
}
```

### <a name="example-2-enroll-a-registrant-when-the-meeting-registration-has-allowedregistrant-set-to-organization"></a>示例 2：当会议注册将 allowedRegistrant 设置为"organization"时注册注册人

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "add-externalregistratrant-private"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
  "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde37",
  "userId": "cc515404-b55c-466e-b896-992c918ecc01"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "add-externalregistratrant-private",
  "@odata.type": "microsoft.graph.externalMeetingRegistrant"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration/registrants/$entity",
  "@odata.type": "#microsoft.graph.externalMeetingRegistrant",
  "id": "30494ab7-7338-4592-bfec-a4333be2a0a6",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NjliNTYxNjktNzAwNi00OTlhLWFmMWEtMGZhY2JjZGM5NmEy%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%2216664f75-11dc-4870-bec6-38c1aaa81431%22%2c%22prid%22%3a%2230494ab7-7338-4592-bfec-a4333be2a0a6%22%2c%22isPublic%22%3afalse%7d",
  "userId": "909c6581-5130-43e9-88f3-fcb3582cde37",
  "tenantId": "cc515404-b55c-466e-b896-992c918ecc01"
}
```
