---
title: 更新 meetingRegistration
description: 更新与联机会议关联的会议注册的详细信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4ea7c340818e561f08f4daddab9c071300711357
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113166"
---
# <a name="update-meetingregistration"></a>更新 meetingRegistration

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表组织者更新与[onlineMeeting](../resources/onlinemeeting.md)联系的[meetingRegistration](../resources/meetingregistration.md)对象的详细信息。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:----------------|:--------------------------------------------|
| 委派（工作或学校帐户） | OnlineMeetings.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{id}/registration
```

## <a name="request-headers"></a>请求标头

| 名称            | 说明               |
| :-------------- | :------------------------ |
| Authorization   | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，仅提供需要以 [meetingRegistration](../resources/meetingregistration.md) 对象的 JSON 表示形式更新的属性。

> [!TIP]
>
>- 所有不是只读的属性都可以更新 **，allowedRegistrant** 属性除外。
>- **无法更新 customQuestions** 导航属性;使用 [Update meetingRegistrationQuestion](meetingregistrationquestion-update.md)方法来更新它。
>- 更新扬声器 **时**，始终提供扬声器的完整列表。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [meetingRegistration](../resources/meetingregistration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update-registration"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration
Content-Type: application/json

{
  "subject":"Microsoft Ignite: Day 1",
  "startDateTime":"2021-11-02T08:00:00-08:00",
  "endDateTime":"2021-11-02T15:45:00-08:00",
  "speakers": [
    {
      "displayName": "Henry Ross",
      "bio": "Chairman and Chief Executive Officer"
    },
    {
      "displayName": "Fred Ryan",
      "bio": "CVP"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-registration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-registration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-registration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-registration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-registration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-registration-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "name": "update-registration",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingRegistration"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/registration(customQuestions())/$entity",
  "id": "gWWckDBR6UOI8_yzWCzeNw,6pABiSU1bkGqzLnbHG_muA,bzLh6uR-5EGYsCvtvIvs6Q,luiTigKrcUGE6Cm33MyQgA,29OIGSH4skyQNu6mNxJr3w,m2bnpmqE_EqwV1Q8dr280E",
  "registrationPageWebUrl": "https://teams.microsoft.com/registration/gWWckDBR6UOI8_yzWCzeNw,6pABiSU1bkGqzLnbHG_muA,bzLh6uR-5EGYsCvtvIvs6Q,luiTigKrcUGE6Cm33MyQgA,29OIGSH4skyQNu6mNxJr3w,m2bnpmqE_EqwV1Q8dr280E?mode=read&tenantId=eefc0b3a-a334-4fb7-ac60-2f1cf13ec00d",
  "allowedRegistrant": "everyone",
  "subject": "Microsoft Ignite: Day 1",
  "description": "Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.",
  "startDateTime": "2021-11-02T16:00:00Z",
  "endDateTime": "2021-11-02T23:45:00Z",
  "registrationPageViewCount": null,
  "speakers": [
    {
      "displayName": "John Doe",
      "bio": "Chairman and Chief Executive Officer"
    },
    {
      "displayName": "Foo Bar",
      "bio": "CVP, Microsoft Security, Compliance & Identity"
    }
  ]
}
```
