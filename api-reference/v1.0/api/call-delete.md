---
title: 删除呼叫
description: 删除或挂断活动呼叫。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d9ad696741d9dfa02fc6dabea43673b268dfe97f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052493"
---
# <a name="delete-call"></a><span data-ttu-id="94578-103">删除呼叫</span><span class="sxs-lookup"><span data-stu-id="94578-103">Delete call</span></span>

<span data-ttu-id="94578-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94578-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94578-105">删除或挂断活动呼叫。</span><span class="sxs-lookup"><span data-stu-id="94578-105">Delete or hang up an active call.</span></span> <span data-ttu-id="94578-106">对于组呼叫，这只会删除你的通话记录，基础组呼叫将继续。</span><span class="sxs-lookup"><span data-stu-id="94578-106">For group calls, this will only delete your call leg and the underlying group call will still continue.</span></span>

## <a name="permissions"></a><span data-ttu-id="94578-107">权限</span><span class="sxs-lookup"><span data-stu-id="94578-107">Permissions</span></span>

| <span data-ttu-id="94578-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="94578-108">Permission type</span></span> | <span data-ttu-id="94578-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94578-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="94578-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94578-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="94578-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="94578-111">Not Supported.</span></span>                         |
| <span data-ttu-id="94578-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94578-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94578-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="94578-113">Not Supported.</span></span>                         |
| <span data-ttu-id="94578-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="94578-114">Application</span></span>                            | <span data-ttu-id="94578-115">无。</span><span class="sxs-lookup"><span data-stu-id="94578-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="94578-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94578-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="94578-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="94578-117">Request headers</span></span>
| <span data-ttu-id="94578-118">名称</span><span class="sxs-lookup"><span data-stu-id="94578-118">Name</span></span>          | <span data-ttu-id="94578-119">说明</span><span class="sxs-lookup"><span data-stu-id="94578-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="94578-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="94578-120">Authorization</span></span> | <span data-ttu-id="94578-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94578-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94578-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="94578-123">Request body</span></span>
<span data-ttu-id="94578-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94578-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94578-125">响应</span><span class="sxs-lookup"><span data-stu-id="94578-125">Response</span></span>
<span data-ttu-id="94578-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="94578-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94578-128">示例</span><span class="sxs-lookup"><span data-stu-id="94578-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="94578-129">请求</span><span class="sxs-lookup"><span data-stu-id="94578-129">Request</span></span>
<span data-ttu-id="94578-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="94578-130">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94578-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="94578-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call-1"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="c"></a>[<span data-ttu-id="94578-132">C#</span><span class="sxs-lookup"><span data-stu-id="94578-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94578-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94578-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94578-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94578-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94578-135">Java</span><span class="sxs-lookup"><span data-stu-id="94578-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94578-136">响应</span><span class="sxs-lookup"><span data-stu-id="94578-136">Response</span></span>

> <span data-ttu-id="94578-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="94578-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="94578-138">通知 - 终止</span><span class="sxs-lookup"><span data-stu-id="94578-138">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="94578-139">Notification - 已终止</span><span class="sxs-lookup"><span data-stu-id="94578-139">Notification - terminated</span></span>

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

