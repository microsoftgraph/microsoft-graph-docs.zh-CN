---
title: 消除 riskyUser
description: 消除 riskyUser 对象的风险。
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 47b749e1ac5d782d96210b493ed1451db19184c7
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761484"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="bfccf-103">riskyUser： dismiss</span><span class="sxs-lookup"><span data-stu-id="bfccf-103">riskyUser: dismiss</span></span>

<span data-ttu-id="bfccf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfccf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="bfccf-105">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="bfccf-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="bfccf-106">消除一个或多个 [riskyUser 对象](../resources/riskyuser.md) 的风险。</span><span class="sxs-lookup"><span data-stu-id="bfccf-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="bfccf-107">此操作将目标用户的风险级别设定为无。</span><span class="sxs-lookup"><span data-stu-id="bfccf-107">This action sets the targeted user's risk level to none.</span></span> <span data-ttu-id="bfccf-108">一次呼叫中要消除的最大用户数为 60。</span><span class="sxs-lookup"><span data-stu-id="bfccf-108">The maximum count of users to dismiss in one call is 60.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfccf-109">权限</span><span class="sxs-lookup"><span data-stu-id="bfccf-109">Permissions</span></span>
<span data-ttu-id="bfccf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfccf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfccf-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfccf-112">Permission type</span></span>      | <span data-ttu-id="bfccf-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfccf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfccf-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfccf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bfccf-115">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfccf-115">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="bfccf-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfccf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfccf-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfccf-117">Not supported.</span></span>    |
|<span data-ttu-id="bfccf-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfccf-118">Application</span></span> | <span data-ttu-id="bfccf-119">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfccf-119">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfccf-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfccf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
GET /identityProtection/riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="bfccf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfccf-121">Request headers</span></span>
| <span data-ttu-id="bfccf-122">名称</span><span class="sxs-lookup"><span data-stu-id="bfccf-122">Name</span></span>      |<span data-ttu-id="bfccf-123">说明</span><span class="sxs-lookup"><span data-stu-id="bfccf-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bfccf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfccf-124">Authorization</span></span>  | <span data-ttu-id="bfccf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfccf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfccf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfccf-127">Request body</span></span>
<span data-ttu-id="bfccf-128">在请求正文中指定要消除的 userId。</span><span class="sxs-lookup"><span data-stu-id="bfccf-128">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="bfccf-129">响应</span><span class="sxs-lookup"><span data-stu-id="bfccf-129">Response</span></span>

<span data-ttu-id="bfccf-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bfccf-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="bfccf-132">示例</span><span class="sxs-lookup"><span data-stu-id="bfccf-132">Examples</span></span>
### <a name="example-1-dismiss-risky-users"></a><span data-ttu-id="bfccf-133">示例 1：消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="bfccf-133">Example 1: Dismiss risky users</span></span>
#### <a name="request"></a><span data-ttu-id="bfccf-134">请求</span><span class="sxs-lookup"><span data-stu-id="bfccf-134">Request</span></span>
<span data-ttu-id="bfccf-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bfccf-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfccf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfccf-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
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
# <a name="c"></a>[<span data-ttu-id="bfccf-137">C#</span><span class="sxs-lookup"><span data-stu-id="bfccf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfccf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfccf-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfccf-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfccf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfccf-140">Java</span><span class="sxs-lookup"><span data-stu-id="bfccf-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bfccf-141">响应</span><span class="sxs-lookup"><span data-stu-id="bfccf-141">Response</span></span>
<span data-ttu-id="bfccf-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bfccf-142">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-dismiss-a-risky-user"></a><span data-ttu-id="bfccf-143">示例 2：消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="bfccf-143">Example 2: Dismiss a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="bfccf-144">请求</span><span class="sxs-lookup"><span data-stu-id="bfccf-144">Request</span></span>
<span data-ttu-id="bfccf-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bfccf-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfccf-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfccf-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
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
# <a name="c"></a>[<span data-ttu-id="bfccf-147">C#</span><span class="sxs-lookup"><span data-stu-id="bfccf-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfccf-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfccf-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfccf-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfccf-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfccf-150">Java</span><span class="sxs-lookup"><span data-stu-id="bfccf-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="bfccf-151">响应</span><span class="sxs-lookup"><span data-stu-id="bfccf-151">Response</span></span>
<span data-ttu-id="bfccf-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bfccf-152">Here is an example of the response.</span></span>
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


