---
title: 删除呼叫
description: 删除或挂断活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 23c3f2d1b79e8eabb2f7abcc45567bb2852f879d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317716"
---
# <a name="delete-call"></a><span data-ttu-id="93488-103">删除呼叫</span><span class="sxs-lookup"><span data-stu-id="93488-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93488-104">删除或挂断活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="93488-104">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="93488-105">权限</span><span class="sxs-lookup"><span data-stu-id="93488-105">Permissions</span></span>

<span data-ttu-id="93488-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93488-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="93488-108">Permission type</span></span> | <span data-ttu-id="93488-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93488-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="93488-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93488-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="93488-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="93488-111">Not Supported.</span></span>                         |
| <span data-ttu-id="93488-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93488-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93488-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="93488-113">Not Supported.</span></span>                         |
| <span data-ttu-id="93488-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="93488-114">Application</span></span>                            | <span data-ttu-id="93488-115">无。</span><span class="sxs-lookup"><span data-stu-id="93488-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="93488-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93488-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="93488-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="93488-117">Request headers</span></span>
| <span data-ttu-id="93488-118">名称</span><span class="sxs-lookup"><span data-stu-id="93488-118">Name</span></span>          | <span data-ttu-id="93488-119">说明</span><span class="sxs-lookup"><span data-stu-id="93488-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="93488-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="93488-120">Authorization</span></span> | <span data-ttu-id="93488-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93488-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93488-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="93488-123">Request body</span></span>
<span data-ttu-id="93488-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="93488-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93488-125">响应</span><span class="sxs-lookup"><span data-stu-id="93488-125">Response</span></span>
<span data-ttu-id="93488-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="93488-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93488-128">示例</span><span class="sxs-lookup"><span data-stu-id="93488-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="93488-129">请求</span><span class="sxs-lookup"><span data-stu-id="93488-129">Request</span></span>
<span data-ttu-id="93488-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="93488-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="93488-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="93488-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93488-132">C#</span><span class="sxs-lookup"><span data-stu-id="93488-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93488-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93488-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93488-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="93488-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="93488-135">Java</span><span class="sxs-lookup"><span data-stu-id="93488-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="93488-136">响应</span><span class="sxs-lookup"><span data-stu-id="93488-136">Response</span></span>

> <span data-ttu-id="93488-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="93488-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="93488-139">通知终止</span><span class="sxs-lookup"><span data-stu-id="93488-139">Notification - terminating</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminating"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="93488-140">通知终止</span><span class="sxs-lookup"><span data-stu-id="93488-140">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppInitiated"
      }
    }
  ]
}
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
