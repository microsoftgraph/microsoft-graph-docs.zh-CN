---
title: 获取状态
description: 获取用户的状态信息。
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 6af22c5e4ab1756aecaa384a78e010e12f071c16
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556287"
---
# <a name="get-presence"></a><span data-ttu-id="f670f-103">获取状态</span><span class="sxs-lookup"><span data-stu-id="f670f-103">Get presence</span></span>

<span data-ttu-id="f670f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f670f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f670f-105">获取用户的[状态](../resources/presence.md)信息。</span><span class="sxs-lookup"><span data-stu-id="f670f-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="f670f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f670f-106">Permissions</span></span>
<span data-ttu-id="f670f-107">若要调用这些 Api，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="f670f-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="f670f-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f670f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f670f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f670f-109">Permission type</span></span> | <span data-ttu-id="f670f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f670f-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f670f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f670f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f670f-112">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="f670f-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="f670f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f670f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f670f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f670f-114">Not Supported.</span></span>                        |
| <span data-ttu-id="f670f-115">Application</span><span class="sxs-lookup"><span data-stu-id="f670f-115">Application</span></span>                            | <span data-ttu-id="f670f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f670f-116">Not Supported.</span></span>                        |

## <a name="http-requests"></a><span data-ttu-id="f670f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f670f-117">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="f670f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f670f-118">Request Headers</span></span>
| <span data-ttu-id="f670f-119">名称</span><span class="sxs-lookup"><span data-stu-id="f670f-119">Name</span></span>          | <span data-ttu-id="f670f-120">说明</span><span class="sxs-lookup"><span data-stu-id="f670f-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f670f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f670f-121">Authorization</span></span> | <span data-ttu-id="f670f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f670f-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f670f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f670f-124">Request body</span></span>

<span data-ttu-id="f670f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f670f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f670f-126">响应</span><span class="sxs-lookup"><span data-stu-id="f670f-126">Response</span></span>
<span data-ttu-id="f670f-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[状态](../resources/presence.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f670f-127">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f670f-128">示例</span><span class="sxs-lookup"><span data-stu-id="f670f-128">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="f670f-129">示例1：获取自己的状态信息</span><span class="sxs-lookup"><span data-stu-id="f670f-129">Example 1: Get your own presence information</span></span>

<span data-ttu-id="f670f-130">下面的示例展示了如何获取自己的状态信息。</span><span class="sxs-lookup"><span data-stu-id="f670f-130">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="f670f-131">此操作需要状态为 "读取" 权限。</span><span class="sxs-lookup"><span data-stu-id="f670f-131">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="f670f-132">请求</span><span class="sxs-lookup"><span data-stu-id="f670f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f670f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f670f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="c"></a>[<span data-ttu-id="f670f-134">C#</span><span class="sxs-lookup"><span data-stu-id="f670f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f670f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f670f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f670f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f670f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f670f-137">响应</span><span class="sxs-lookup"><span data-stu-id="f670f-137">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="f670f-138">示例2：获取其他用户的状态信息</span><span class="sxs-lookup"><span data-stu-id="f670f-138">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="f670f-139">下面的示例展示了如何获取其他用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="f670f-139">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="f670f-140">此操作需要已读。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="f670f-140">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="f670f-141">请求</span><span class="sxs-lookup"><span data-stu-id="f670f-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f670f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f670f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="f670f-143">C#</span><span class="sxs-lookup"><span data-stu-id="f670f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f670f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f670f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f670f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f670f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f670f-146">响应</span><span class="sxs-lookup"><span data-stu-id="f670f-146">Response</span></span>

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

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="f670f-147">示例3：获取其他用户的状态信息</span><span class="sxs-lookup"><span data-stu-id="f670f-147">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="f670f-148">下面的示例展示了如何获取其他用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="f670f-148">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="f670f-149">此操作需要已读。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="f670f-149">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="f670f-150">请求</span><span class="sxs-lookup"><span data-stu-id="f670f-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```

#### <a name="response"></a><span data-ttu-id="f670f-151">响应</span><span class="sxs-lookup"><span data-stu-id="f670f-151">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
            "availability": "Away",
            "activity": "BeRightBack"
        }
    ]
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
