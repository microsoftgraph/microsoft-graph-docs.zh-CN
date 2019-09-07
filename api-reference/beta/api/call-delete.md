---
title: 删除呼叫
description: 删除或挂断活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aa1d0111085fa48f6c6186e764d19210a9f10ae2
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792413"
---
# <a name="delete-call"></a><span data-ttu-id="8f4ca-103">删除呼叫</span><span class="sxs-lookup"><span data-stu-id="8f4ca-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f4ca-104">删除或挂断活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-104">Delete or hang up an active call.</span></span> <span data-ttu-id="8f4ca-105">对于多方呼叫，这只会删除您的呼叫线路;基础多方调用仍将继续。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-105">For multiparty calls, this will only delete your call leg; the underlying multiparty call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f4ca-106">权限</span><span class="sxs-lookup"><span data-stu-id="8f4ca-106">Permissions</span></span>

<span data-ttu-id="8f4ca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f4ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f4ca-109">Permission type</span></span> | <span data-ttu-id="8f4ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f4ca-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="8f4ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f4ca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f4ca-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-112">Not Supported.</span></span>                         |
| <span data-ttu-id="8f4ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f4ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f4ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-114">Not Supported.</span></span>                         |
| <span data-ttu-id="8f4ca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f4ca-115">Application</span></span>                            | <span data-ttu-id="8f4ca-116">无。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="8f4ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f4ca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8f4ca-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f4ca-118">Request headers</span></span>
| <span data-ttu-id="8f4ca-119">名称</span><span class="sxs-lookup"><span data-stu-id="8f4ca-119">Name</span></span>          | <span data-ttu-id="8f4ca-120">说明</span><span class="sxs-lookup"><span data-stu-id="8f4ca-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8f4ca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f4ca-121">Authorization</span></span> | <span data-ttu-id="8f4ca-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f4ca-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f4ca-124">Request body</span></span>
<span data-ttu-id="8f4ca-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f4ca-126">响应</span><span class="sxs-lookup"><span data-stu-id="8f4ca-126">Response</span></span>
<span data-ttu-id="8f4ca-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f4ca-129">示例</span><span class="sxs-lookup"><span data-stu-id="8f4ca-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8f4ca-130">请求</span><span class="sxs-lookup"><span data-stu-id="8f4ca-130">Request</span></span>
<span data-ttu-id="8f4ca-131">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8f4ca-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8f4ca-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f4ca-133">C#</span><span class="sxs-lookup"><span data-stu-id="8f4ca-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f4ca-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f4ca-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f4ca-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="8f4ca-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8f4ca-136">响应</span><span class="sxs-lookup"><span data-stu-id="8f4ca-136">Response</span></span>

> <span data-ttu-id="8f4ca-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8f4ca-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="8f4ca-139">通知终止</span><span class="sxs-lookup"><span data-stu-id="8f4ca-139">Notification - terminating</span></span>

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
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminating"
      }
    }
  ]
}
  
```

##### <a name="notification---terminated"></a><span data-ttu-id="8f4ca-140">通知终止</span><span class="sxs-lookup"><span data-stu-id="8f4ca-140">Notification - terminated</span></span>

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
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": "0"
        }
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
