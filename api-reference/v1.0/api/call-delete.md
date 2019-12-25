---
title: 删除呼叫
description: 删除或挂断活动呼叫。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: def11fd1f30cbba8a1bef7f85821d7901dc7f379
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871123"
---
# <a name="delete-call"></a><span data-ttu-id="401cd-103">删除呼叫</span><span class="sxs-lookup"><span data-stu-id="401cd-103">Delete call</span></span>

<span data-ttu-id="401cd-104">删除或挂断活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="401cd-104">Delete or hang up an active call.</span></span> <span data-ttu-id="401cd-105">对于组呼叫，这只会删除您的呼叫线路，基础组呼叫仍将继续进行。</span><span class="sxs-lookup"><span data-stu-id="401cd-105">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="401cd-106">权限</span><span class="sxs-lookup"><span data-stu-id="401cd-106">Permissions</span></span>

| <span data-ttu-id="401cd-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="401cd-107">Permission type</span></span> | <span data-ttu-id="401cd-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="401cd-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="401cd-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="401cd-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="401cd-110">不支持。</span><span class="sxs-lookup"><span data-stu-id="401cd-110">Not Supported.</span></span>                         |
| <span data-ttu-id="401cd-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="401cd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="401cd-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="401cd-112">Not Supported.</span></span>                         |
| <span data-ttu-id="401cd-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="401cd-113">Application</span></span>                            | <span data-ttu-id="401cd-114">无。</span><span class="sxs-lookup"><span data-stu-id="401cd-114">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="401cd-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="401cd-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="401cd-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="401cd-116">Request headers</span></span>
| <span data-ttu-id="401cd-117">名称</span><span class="sxs-lookup"><span data-stu-id="401cd-117">Name</span></span>          | <span data-ttu-id="401cd-118">说明</span><span class="sxs-lookup"><span data-stu-id="401cd-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="401cd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="401cd-119">Authorization</span></span> | <span data-ttu-id="401cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="401cd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="401cd-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="401cd-122">Request body</span></span>
<span data-ttu-id="401cd-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="401cd-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="401cd-124">响应</span><span class="sxs-lookup"><span data-stu-id="401cd-124">Response</span></span>
<span data-ttu-id="401cd-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="401cd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="401cd-127">示例</span><span class="sxs-lookup"><span data-stu-id="401cd-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="401cd-128">请求</span><span class="sxs-lookup"><span data-stu-id="401cd-128">Request</span></span>
<span data-ttu-id="401cd-129">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="401cd-129">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="401cd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="401cd-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="401cd-131">C#</span><span class="sxs-lookup"><span data-stu-id="401cd-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="401cd-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="401cd-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="401cd-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="401cd-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="401cd-134">Java</span><span class="sxs-lookup"><span data-stu-id="401cd-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="401cd-135">响应</span><span class="sxs-lookup"><span data-stu-id="401cd-135">Response</span></span>

> <span data-ttu-id="401cd-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="401cd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="401cd-138">通知终止</span><span class="sxs-lookup"><span data-stu-id="401cd-138">Notification - terminating</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminating"
      }
    }
  ]
}
  
```

##### <a name="notification---terminated"></a><span data-ttu-id="401cd-139">通知终止</span><span class="sxs-lookup"><span data-stu-id="401cd-139">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
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
