---
title: 获取状态
description: 获取用户的状态信息。
author: VinodRavichandran
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: fa059a7399762444d73a13305b5bec722830a1c0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867690"
---
# <a name="get-presence"></a><span data-ttu-id="55e99-103">获取状态</span><span class="sxs-lookup"><span data-stu-id="55e99-103">Get presence</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55e99-104">获取用户的[状态](../resources/presence.md)信息。</span><span class="sxs-lookup"><span data-stu-id="55e99-104">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="55e99-105">权限</span><span class="sxs-lookup"><span data-stu-id="55e99-105">Permissions</span></span>
<span data-ttu-id="55e99-106">若要调用这些 Api，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="55e99-106">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="55e99-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55e99-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55e99-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="55e99-108">Permission type</span></span> | <span data-ttu-id="55e99-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55e99-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="55e99-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55e99-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="55e99-111">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="55e99-111">Presence.Read, Presence.Read.All</span></span>                         |
| <span data-ttu-id="55e99-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55e99-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55e99-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="55e99-113">Not Supported.</span></span>                         |
| <span data-ttu-id="55e99-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="55e99-114">Application</span></span>                            | <span data-ttu-id="55e99-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="55e99-115">Not Supported.</span></span>                                  |

## <a name="http-requests"></a><span data-ttu-id="55e99-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55e99-116">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
```

## <a name="request-headers"></a><span data-ttu-id="55e99-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="55e99-117">Request Headers</span></span>
| <span data-ttu-id="55e99-118">名称</span><span class="sxs-lookup"><span data-stu-id="55e99-118">Name</span></span>          | <span data-ttu-id="55e99-119">说明</span><span class="sxs-lookup"><span data-stu-id="55e99-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="55e99-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="55e99-120">Authorization</span></span> | <span data-ttu-id="55e99-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55e99-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="55e99-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="55e99-123">Request body</span></span>

<span data-ttu-id="55e99-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55e99-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55e99-125">响应</span><span class="sxs-lookup"><span data-stu-id="55e99-125">Response</span></span>
<span data-ttu-id="55e99-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[状态](../resources/presence.md)对象。</span><span class="sxs-lookup"><span data-stu-id="55e99-126">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55e99-127">示例</span><span class="sxs-lookup"><span data-stu-id="55e99-127">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="55e99-128">示例1：获取自己的状态信息</span><span class="sxs-lookup"><span data-stu-id="55e99-128">Example 1: Get your own presence information</span></span>

<span data-ttu-id="55e99-129">下面的示例展示了如何获取自己的状态信息。</span><span class="sxs-lookup"><span data-stu-id="55e99-129">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="55e99-130">此操作需要状态为 "读取" 权限。</span><span class="sxs-lookup"><span data-stu-id="55e99-130">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="55e99-131">请求</span><span class="sxs-lookup"><span data-stu-id="55e99-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="55e99-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="55e99-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="55e99-133">C#</span><span class="sxs-lookup"><span data-stu-id="55e99-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e99-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55e99-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55e99-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55e99-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55e99-136">响应</span><span class="sxs-lookup"><span data-stu-id="55e99-136">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="55e99-137">示例2：获取其他用户的状态信息</span><span class="sxs-lookup"><span data-stu-id="55e99-137">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="55e99-138">下面的示例展示了如何获取其他用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="55e99-138">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="55e99-139">此操作需要已读。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="55e99-139">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="55e99-140">请求</span><span class="sxs-lookup"><span data-stu-id="55e99-140">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="55e99-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="55e99-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="55e99-142">C#</span><span class="sxs-lookup"><span data-stu-id="55e99-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55e99-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55e99-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55e99-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55e99-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55e99-145">响应</span><span class="sxs-lookup"><span data-stu-id="55e99-145">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
