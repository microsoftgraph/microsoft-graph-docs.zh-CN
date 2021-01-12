---
title: 获取状态
description: 获取用户状态信息。
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 80a5bd421d3c8ab5497f0b52a52fb77135e11648
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796708"
---
# <a name="get-presence"></a><span data-ttu-id="d72dd-103">获取状态</span><span class="sxs-lookup"><span data-stu-id="d72dd-103">Get presence</span></span>

<span data-ttu-id="d72dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d72dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d72dd-105">获取用户 [状态](../resources/presence.md) 信息。</span><span class="sxs-lookup"><span data-stu-id="d72dd-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="d72dd-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d72dd-106">Permissions</span></span>
<span data-ttu-id="d72dd-107">调用这些 API 需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="d72dd-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="d72dd-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d72dd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d72dd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d72dd-109">Permission type</span></span> | <span data-ttu-id="d72dd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d72dd-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="d72dd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d72dd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d72dd-112">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="d72dd-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="d72dd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d72dd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d72dd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d72dd-114">Not Supported.</span></span>                        |
| <span data-ttu-id="d72dd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d72dd-115">Application</span></span>                            | <span data-ttu-id="d72dd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d72dd-116">Not Supported.</span></span>                        |

## <a name="http-requests"></a><span data-ttu-id="d72dd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d72dd-117">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="d72dd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d72dd-118">Request Headers</span></span>
| <span data-ttu-id="d72dd-119">名称</span><span class="sxs-lookup"><span data-stu-id="d72dd-119">Name</span></span>          | <span data-ttu-id="d72dd-120">说明</span><span class="sxs-lookup"><span data-stu-id="d72dd-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d72dd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d72dd-121">Authorization</span></span> | <span data-ttu-id="d72dd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d72dd-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d72dd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d72dd-124">Request body</span></span>

<span data-ttu-id="d72dd-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d72dd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d72dd-126">响应</span><span class="sxs-lookup"><span data-stu-id="d72dd-126">Response</span></span>
<span data-ttu-id="d72dd-127">如果成功，此方法在响应 `200 OK` 正文中返回响应代码[](../resources/presence.md)和状态对象。</span><span class="sxs-lookup"><span data-stu-id="d72dd-127">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d72dd-128">示例</span><span class="sxs-lookup"><span data-stu-id="d72dd-128">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="d72dd-129">示例 1：获取你自己的状态信息</span><span class="sxs-lookup"><span data-stu-id="d72dd-129">Example 1: Get your own presence information</span></span>

<span data-ttu-id="d72dd-130">以下示例显示如何获取你自己的状态信息。</span><span class="sxs-lookup"><span data-stu-id="d72dd-130">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="d72dd-131">此操作需要 Presence.Read 权限。</span><span class="sxs-lookup"><span data-stu-id="d72dd-131">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="d72dd-132">请求</span><span class="sxs-lookup"><span data-stu-id="d72dd-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d72dd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d72dd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```
# <a name="c"></a>[<span data-ttu-id="d72dd-134">C#</span><span class="sxs-lookup"><span data-stu-id="d72dd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d72dd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d72dd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d72dd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d72dd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d72dd-137">Java</span><span class="sxs-lookup"><span data-stu-id="d72dd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-your-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d72dd-138">响应</span><span class="sxs-lookup"><span data-stu-id="d72dd-138">Response</span></span>

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
  "activity": "Available",
  "outOfOfficeSettings": {
    "message": null,
    "isOutOfOffice": false
  }
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="d72dd-139">示例 2：获取其他用户状态信息</span><span class="sxs-lookup"><span data-stu-id="d72dd-139">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="d72dd-140">以下示例显示如何获取其他用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="d72dd-140">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="d72dd-141">此操作需要 Presence.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="d72dd-141">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="d72dd-142">请求</span><span class="sxs-lookup"><span data-stu-id="d72dd-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d72dd-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d72dd-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="d72dd-144">C#</span><span class="sxs-lookup"><span data-stu-id="d72dd-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d72dd-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d72dd-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d72dd-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d72dd-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d72dd-147">Java</span><span class="sxs-lookup"><span data-stu-id="d72dd-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d72dd-148">响应</span><span class="sxs-lookup"><span data-stu-id="d72dd-148">Response</span></span>

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
  "activity": "Presenting",
  "outOfOfficeSettings": {
    "message": null,
    "isOutOfOffice": false
  }
}
```

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="d72dd-149">示例 3：获取其他用户状态信息</span><span class="sxs-lookup"><span data-stu-id="d72dd-149">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="d72dd-150">以下示例显示如何获取其他用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="d72dd-150">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="d72dd-151">此操作需要 Presence.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="d72dd-151">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="d72dd-152">请求</span><span class="sxs-lookup"><span data-stu-id="d72dd-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d72dd-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="d72dd-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```
# <a name="c"></a>[<span data-ttu-id="d72dd-154">C#</span><span class="sxs-lookup"><span data-stu-id="d72dd-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d72dd-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d72dd-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d72dd-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d72dd-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d72dd-157">Java</span><span class="sxs-lookup"><span data-stu-id="d72dd-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d72dd-158">响应</span><span class="sxs-lookup"><span data-stu-id="d72dd-158">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
  "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
  "availability": "Away",
  "activity": "BeRightBack",
  "outOfOfficeSettings": {
    "message": null,
    "isOutOfOffice": false
  }
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


