---
title: 删除 onlineMeeting
description: 删除联机会议。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9998e67ff9e8ffe93d349115cfe50beb8d317073
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456521"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="b4ee2-103">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b4ee2-103">Delete onlineMeeting</span></span>

<span data-ttu-id="b4ee2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b4ee2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4ee2-105">删除[onlineMeeting](../resources/onlinemeeting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b4ee2-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ee2-106">权限</span><span class="sxs-lookup"><span data-stu-id="b4ee2-106">Permissions</span></span>

| <span data-ttu-id="b4ee2-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4ee2-107">Permission type</span></span> | <span data-ttu-id="b4ee2-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4ee2-108">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="b4ee2-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ee2-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4ee2-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4ee2-110">OnlineMeetings.ReadWrite</span></span>              |
| <span data-ttu-id="b4ee2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ee2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ee2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4ee2-112">Not Supported.</span></span>                         |
| <span data-ttu-id="b4ee2-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4ee2-113">Application</span></span>                            | <span data-ttu-id="b4ee2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4ee2-114">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="b4ee2-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4ee2-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4ee2-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4ee2-116">Request headers</span></span>
| <span data-ttu-id="b4ee2-117">名称</span><span class="sxs-lookup"><span data-stu-id="b4ee2-117">Name</span></span>          | <span data-ttu-id="b4ee2-118">说明</span><span class="sxs-lookup"><span data-stu-id="b4ee2-118">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b4ee2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4ee2-119">Authorization</span></span> | <span data-ttu-id="b4ee2-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4ee2-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4ee2-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4ee2-122">Request body</span></span>
<span data-ttu-id="b4ee2-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4ee2-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4ee2-124">响应</span><span class="sxs-lookup"><span data-stu-id="b4ee2-124">Response</span></span>
<span data-ttu-id="b4ee2-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4ee2-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4ee2-127">示例</span><span class="sxs-lookup"><span data-stu-id="b4ee2-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4ee2-128">请求</span><span class="sxs-lookup"><span data-stu-id="b4ee2-128">Request</span></span>
<span data-ttu-id="b4ee2-129">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4ee2-129">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4ee2-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4ee2-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="b4ee2-131">C#</span><span class="sxs-lookup"><span data-stu-id="b4ee2-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4ee2-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4ee2-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4ee2-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4ee2-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b4ee2-134">响应</span><span class="sxs-lookup"><span data-stu-id="b4ee2-134">Response</span></span>

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
