---
title: 获取状态
description: 获取用户状态信息。
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 591c388418ddb60fad1d78a04de79cb65a884630
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663948"
---
# <a name="get-presence"></a><span data-ttu-id="6fcb1-103">获取状态</span><span class="sxs-lookup"><span data-stu-id="6fcb1-103">Get presence</span></span>

<span data-ttu-id="6fcb1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fcb1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fcb1-105">获取用户 [状态](../resources/presence.md) 信息。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fcb1-106">权限</span><span class="sxs-lookup"><span data-stu-id="6fcb1-106">Permissions</span></span>
<span data-ttu-id="6fcb1-107">调用这些 API 需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="6fcb1-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6fcb1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fcb1-109">Permission type</span></span> | <span data-ttu-id="6fcb1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fcb1-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="6fcb1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fcb1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fcb1-112">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="6fcb1-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="6fcb1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fcb1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fcb1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-114">Not Supported.</span></span>                        |
| <span data-ttu-id="6fcb1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fcb1-115">Application</span></span>                            | <span data-ttu-id="6fcb1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-116">Not Supported.</span></span>                        |

> <span data-ttu-id="6fcb1-117">**注意：** 此 API 的最大请求速率是每个租户每个应用程序的 30 秒内 1500 个 API 请求。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-117">**Note:** The maximum request rate for this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-requests"></a><span data-ttu-id="6fcb1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fcb1-118">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="6fcb1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fcb1-119">Request Headers</span></span>
| <span data-ttu-id="6fcb1-120">名称</span><span class="sxs-lookup"><span data-stu-id="6fcb1-120">Name</span></span>          | <span data-ttu-id="6fcb1-121">说明</span><span class="sxs-lookup"><span data-stu-id="6fcb1-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6fcb1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fcb1-122">Authorization</span></span> | <span data-ttu-id="6fcb1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6fcb1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fcb1-125">Request body</span></span>

<span data-ttu-id="6fcb1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fcb1-127">响应</span><span class="sxs-lookup"><span data-stu-id="6fcb1-127">Response</span></span>
<span data-ttu-id="6fcb1-128">如果成功，此方法在响应 `200 OK` 正文中返回响应代码[](../resources/presence.md)和状态对象。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-128">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fcb1-129">示例</span><span class="sxs-lookup"><span data-stu-id="6fcb1-129">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="6fcb1-130">示例 1：获取你自己的状态信息</span><span class="sxs-lookup"><span data-stu-id="6fcb1-130">Example 1: Get your own presence information</span></span>

<span data-ttu-id="6fcb1-131">以下示例显示如何获取你自己的状态信息。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-131">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="6fcb1-132">此操作需要 Presence.Read 权限。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-132">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="6fcb1-133">请求</span><span class="sxs-lookup"><span data-stu-id="6fcb1-133">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="6fcb1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fcb1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/presence
```
# <a name="c"></a>[<span data-ttu-id="6fcb1-135">C#</span><span class="sxs-lookup"><span data-stu-id="6fcb1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-your-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fcb1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fcb1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-your-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fcb1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fcb1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-your-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fcb1-138">Java</span><span class="sxs-lookup"><span data-stu-id="6fcb1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-your-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="6fcb1-139">响应</span><span class="sxs-lookup"><span data-stu-id="6fcb1-139">Response</span></span>

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

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="6fcb1-140">示例 2：获取其他用户状态信息</span><span class="sxs-lookup"><span data-stu-id="6fcb1-140">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="6fcb1-141">以下示例显示如何获取其他用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-141">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="6fcb1-142">此操作需要 Presence.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-142">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="6fcb1-143">请求</span><span class="sxs-lookup"><span data-stu-id="6fcb1-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6fcb1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fcb1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```
# <a name="c"></a>[<span data-ttu-id="6fcb1-145">C#</span><span class="sxs-lookup"><span data-stu-id="6fcb1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fcb1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fcb1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fcb1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fcb1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fcb1-148">Java</span><span class="sxs-lookup"><span data-stu-id="6fcb1-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="6fcb1-149">响应</span><span class="sxs-lookup"><span data-stu-id="6fcb1-149">Response</span></span>

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

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="6fcb1-150">示例 3：获取其他用户状态信息</span><span class="sxs-lookup"><span data-stu-id="6fcb1-150">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="6fcb1-151">以下示例显示如何获取其他用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-151">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="6fcb1-152">此操作需要 Presence.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="6fcb1-152">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="6fcb1-153">请求</span><span class="sxs-lookup"><span data-stu-id="6fcb1-153">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```

---


#### <a name="response"></a><span data-ttu-id="6fcb1-154">响应</span><span class="sxs-lookup"><span data-stu-id="6fcb1-154">Response</span></span>

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


