---
title: 消除 riskyUser
description: 消除 riskyUser 对象的风险。
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: eaf5ce5c0ed05777fa4ccb05a05adf1ed215ac2a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960853"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="37e39-103">riskyUser： dismiss</span><span class="sxs-lookup"><span data-stu-id="37e39-103">riskyUser: dismiss</span></span>

<span data-ttu-id="37e39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="37e39-105">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="37e39-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="37e39-106">消除一个或多个 [riskyUser 对象](../resources/riskyuser.md) 的风险。</span><span class="sxs-lookup"><span data-stu-id="37e39-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="37e39-107">此操作将目标用户的风险级别设定为无。</span><span class="sxs-lookup"><span data-stu-id="37e39-107">This action sets the targeted user's risk level to none.</span></span> <span data-ttu-id="37e39-108">一次呼叫中要消除的最大用户数为 60。</span><span class="sxs-lookup"><span data-stu-id="37e39-108">The maximum count of users to dismiss in one call is 60.</span></span>

## <a name="permissions"></a><span data-ttu-id="37e39-109">权限</span><span class="sxs-lookup"><span data-stu-id="37e39-109">Permissions</span></span>
<span data-ttu-id="37e39-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37e39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37e39-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="37e39-112">Permission type</span></span>      | <span data-ttu-id="37e39-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37e39-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37e39-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37e39-114">Delegated (work or school account)</span></span> | <span data-ttu-id="37e39-115">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e39-115">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="37e39-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37e39-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37e39-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="37e39-117">Not supported.</span></span>    |
|<span data-ttu-id="37e39-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="37e39-118">Application</span></span> | <span data-ttu-id="37e39-119">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e39-119">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37e39-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37e39-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
GET /identityProtection/riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="37e39-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="37e39-121">Request headers</span></span>
| <span data-ttu-id="37e39-122">名称</span><span class="sxs-lookup"><span data-stu-id="37e39-122">Name</span></span>      |<span data-ttu-id="37e39-123">说明</span><span class="sxs-lookup"><span data-stu-id="37e39-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37e39-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="37e39-124">Authorization</span></span>  | <span data-ttu-id="37e39-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37e39-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37e39-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="37e39-127">Request body</span></span>
<span data-ttu-id="37e39-128">在请求正文中指定要消除的 userId。</span><span class="sxs-lookup"><span data-stu-id="37e39-128">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="37e39-129">响应</span><span class="sxs-lookup"><span data-stu-id="37e39-129">Response</span></span>

<span data-ttu-id="37e39-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="37e39-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="37e39-132">示例</span><span class="sxs-lookup"><span data-stu-id="37e39-132">Examples</span></span>
### <a name="example-1-dismiss-risky-users"></a><span data-ttu-id="37e39-133">示例 1：消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="37e39-133">Example 1: Dismiss risky users</span></span>
#### <a name="request"></a><span data-ttu-id="37e39-134">请求</span><span class="sxs-lookup"><span data-stu-id="37e39-134">Request</span></span>
<span data-ttu-id="37e39-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37e39-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37e39-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="37e39-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser_1"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="37e39-137">C#</span><span class="sxs-lookup"><span data-stu-id="37e39-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37e39-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37e39-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37e39-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37e39-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37e39-140">Java</span><span class="sxs-lookup"><span data-stu-id="37e39-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="37e39-141">响应</span><span class="sxs-lookup"><span data-stu-id="37e39-141">Response</span></span>
<span data-ttu-id="37e39-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="37e39-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-dismiss-a-risky-user"></a><span data-ttu-id="37e39-143">示例 2：消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="37e39-143">Example 2: Dismiss a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="37e39-144">请求</span><span class="sxs-lookup"><span data-stu-id="37e39-144">Request</span></span>
<span data-ttu-id="37e39-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37e39-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37e39-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="37e39-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser_2"
}-->
```http
POST https://graph.microsoft.com/beta/identityProtection/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="37e39-147">C#</span><span class="sxs-lookup"><span data-stu-id="37e39-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37e39-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37e39-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37e39-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37e39-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37e39-150">Java</span><span class="sxs-lookup"><span data-stu-id="37e39-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="37e39-151">响应</span><span class="sxs-lookup"><span data-stu-id="37e39-151">Response</span></span>
<span data-ttu-id="37e39-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="37e39-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


