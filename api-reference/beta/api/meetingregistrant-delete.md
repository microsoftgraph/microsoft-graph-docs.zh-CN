---
title: 删除 meetingRegistrant
description: 取消 meetingRegistrant 的 onlineMeeting 注册。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5529c31b6b5bb0df1b51cb62f808ff7f389e07b4
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369448"
---
# <a name="unenroll-meeting-registrant"></a>注销会议注册人

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表注册人取消[meetingRegistrant](../resources/meetingregistrant.md)的[onlineMeeting](../resources/onlinemeeting.md)注册。

仅在 **meetingRegistration 对象的 allowedRegistrant** 属性的值为 且注册人委派权限用于注册时 [](../resources/meetingregistration.md) `organization` 使用此方法。 当 **allowedRegistrant** 值为 时，注册人只能使用收到的电子邮件中的链接 `everyone` 取消注册。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetings.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | OnlineMeetings.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{userId}/onlineMeetings/{meetingId}/registration/registrants/{id}
```

>**注意：**
>
> - `userId` 是会议组织者的 objectID。
> - `meetingId`是 [onlineMeeting 对象的](../resources/onlineMeeting.md) **ID。**

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
  "name": "delete-registratrant-user"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/16664f75-11dc-4870-bec6-38c1aaa81431/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants/gWWckDBR6UOI8_yzWCzeNw,6pAAiSU1bkGqc8soJZw5Pg,3aMJxgQBxEufdo7_Qube_w,YgKy1Rtx-0SFjRbv-ww1ag,Cuzk8JP_iTTWqCOyVcalVA
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "name": "delete-registratrant-user",
}-->

```http
HTTP/1.1 204 No Content
```
