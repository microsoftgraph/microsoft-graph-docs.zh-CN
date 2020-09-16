---
title: 删除 onlineMeeting
description: 删除联机会议。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 051db73f098272bc97fe3477e6bd8dd3f49eddf5
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843266"
---
# <a name="delete-onlinemeeting"></a>删除 onlineMeeting

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 [onlineMeeting](../resources/onlinemeeting.md) 对象。

## <a name="permissions"></a>权限

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | OnlineMeetings.ReadWrite                    |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | OnlineMeetings.ReadWrite.All*                |

> [!IMPORTANT]
> \* 管理员必须创建 [应用程序访问策略](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md) ，并向用户授予该策略中配置的应用程序，以便代表该用户删除联机会议 (在已创建的 reuqest 路径) 中指定的用户 ID。

## <a name="http-request"></a>HTTP 请求

使用委派令牌时的请求
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/{meetingId}
```

使用应用程序令牌时请求：
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/users/{userId}/onlineMeetings/{meetingId}
```

> **注意：**
>
> - `userId` 是 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中用户的对象 ID。 有关更多详细信息，请参阅 [应用程序访问策略](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md)。
> - `meetingId`是[onlineMeeting 实体](../resources/onlinemeeting.md)的**id** 。

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
下面为请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
