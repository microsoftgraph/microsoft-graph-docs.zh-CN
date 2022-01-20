---
title: 删除 meetingRegistrationQuestion
description: 从联机会议中删除自定义会议注册问题。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7f00f76ef30ed31c84201feabb4916b052ec5c16
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102804"
---
# <a name="delete-meetingregistrationquestion"></a>删除 meetingRegistrationQuestion

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 [组织者从](../resources/meetingregistrationquestion.md) [meetingRegistration](../resources/meetingregistration.md) 对象中删除自定义注册问题。

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
DELETE /me/onlineMeetings/{meetingId}/registration/customQuestions/{id}
```

> [!NOTE]
> `meetingId`是 [onlineMeeting 对象的](../resources/onlineMeeting.md) **ID。**

## <a name="request-headers"></a>请求标头

| 名称            | 说明               |
| :-------------- | :------------------------ |
| Authorization   | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法仅返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-custom-question"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/customQuestions/MSMxY2E2ZmE3OS1hOTY3LTQ4ZX3lvdV94MDAyMF9hX3gwMDIwX2RldmU=
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-custom-question-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-custom-question-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-custom-question-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-custom-question-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-custom-question-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-custom-question-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "name": "delete-custom-question"
}-->

```http
HTTP/1.1 204 No Content
```
