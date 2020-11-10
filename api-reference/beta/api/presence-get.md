---
title: 获取状态
description: 获取用户的状态信息。
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: a4851b527807c8c8787ad0fca62661a7f2c73175
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967128"
---
# <a name="get-presence"></a><span data-ttu-id="0e3ab-103">获取状态</span><span class="sxs-lookup"><span data-stu-id="0e3ab-103">Get presence</span></span>

<span data-ttu-id="0e3ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e3ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e3ab-105">获取用户的 [状态](../resources/presence.md) 信息。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e3ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="0e3ab-106">Permissions</span></span>
<span data-ttu-id="0e3ab-107">若要调用这些 Api，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="0e3ab-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e3ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e3ab-109">Permission type</span></span> | <span data-ttu-id="0e3ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e3ab-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="0e3ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e3ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e3ab-112">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="0e3ab-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="0e3ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e3ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e3ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-114">Not Supported.</span></span>                        |
| <span data-ttu-id="0e3ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e3ab-115">Application</span></span>                            | <span data-ttu-id="0e3ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-116">Not Supported.</span></span>                        |

## <a name="http-requests"></a><span data-ttu-id="0e3ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e3ab-117">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="0e3ab-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e3ab-118">Request Headers</span></span>
| <span data-ttu-id="0e3ab-119">名称</span><span class="sxs-lookup"><span data-stu-id="0e3ab-119">Name</span></span>          | <span data-ttu-id="0e3ab-120">说明</span><span class="sxs-lookup"><span data-stu-id="0e3ab-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0e3ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e3ab-121">Authorization</span></span> | <span data-ttu-id="0e3ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0e3ab-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e3ab-124">Request body</span></span>

<span data-ttu-id="0e3ab-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e3ab-126">响应</span><span class="sxs-lookup"><span data-stu-id="0e3ab-126">Response</span></span>
<span data-ttu-id="0e3ab-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [状态](../resources/presence.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-127">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e3ab-128">示例</span><span class="sxs-lookup"><span data-stu-id="0e3ab-128">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="0e3ab-129">示例1：获取自己的状态信息</span><span class="sxs-lookup"><span data-stu-id="0e3ab-129">Example 1: Get your own presence information</span></span>

<span data-ttu-id="0e3ab-130">下面的示例展示了如何获取自己的状态信息。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-130">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="0e3ab-131">此操作需要状态为 "读取" 权限。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-131">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="0e3ab-132">请求</span><span class="sxs-lookup"><span data-stu-id="0e3ab-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0e3ab-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e3ab-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="c"></a>[<span data-ttu-id="0e3ab-134">C#</span><span class="sxs-lookup"><span data-stu-id="0e3ab-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e3ab-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e3ab-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e3ab-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e3ab-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e3ab-137">Java</span><span class="sxs-lookup"><span data-stu-id="0e3ab-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-your-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0e3ab-138">响应</span><span class="sxs-lookup"><span data-stu-id="0e3ab-138">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="0e3ab-139">示例2：获取其他用户的状态信息</span><span class="sxs-lookup"><span data-stu-id="0e3ab-139">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="0e3ab-140">下面的示例展示了如何获取其他用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-140">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="0e3ab-141">此操作需要已读。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-141">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="0e3ab-142">请求</span><span class="sxs-lookup"><span data-stu-id="0e3ab-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0e3ab-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e3ab-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="0e3ab-144">C#</span><span class="sxs-lookup"><span data-stu-id="0e3ab-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e3ab-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e3ab-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e3ab-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e3ab-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e3ab-147">Java</span><span class="sxs-lookup"><span data-stu-id="0e3ab-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0e3ab-148">响应</span><span class="sxs-lookup"><span data-stu-id="0e3ab-148">Response</span></span>

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

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="0e3ab-149">示例3：获取其他用户的状态信息</span><span class="sxs-lookup"><span data-stu-id="0e3ab-149">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="0e3ab-150">下面的示例展示了如何获取其他用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-150">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="0e3ab-151">此操作需要已读。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="0e3ab-151">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="0e3ab-152">请求</span><span class="sxs-lookup"><span data-stu-id="0e3ab-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0e3ab-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e3ab-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```
# <a name="c"></a>[<span data-ttu-id="0e3ab-154">C#</span><span class="sxs-lookup"><span data-stu-id="0e3ab-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e3ab-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e3ab-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e3ab-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e3ab-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e3ab-157">Java</span><span class="sxs-lookup"><span data-stu-id="0e3ab-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0e3ab-158">响应</span><span class="sxs-lookup"><span data-stu-id="0e3ab-158">Response</span></span>

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


