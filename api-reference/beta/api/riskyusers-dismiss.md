---
title: 消除 riskyUser
description: 消除 riskyUser 对象的风险。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 8ae21d3adb754798ea2332c1b9acc7880b4a6d99
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975889"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="899d6-103">riskyUser：消除</span><span class="sxs-lookup"><span data-stu-id="899d6-103">riskyUser: dismiss</span></span>

<span data-ttu-id="899d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="899d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="899d6-105">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="899d6-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="899d6-106">消除一个或多个 [riskyUser](../resources/riskyuser.md) 对象的风险。</span><span class="sxs-lookup"><span data-stu-id="899d6-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="899d6-107">此操作将目标用户的风险级别设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="899d6-107">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="899d6-108">权限</span><span class="sxs-lookup"><span data-stu-id="899d6-108">Permissions</span></span>
<span data-ttu-id="899d6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="899d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="899d6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="899d6-111">Permission type</span></span>      | <span data-ttu-id="899d6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="899d6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="899d6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="899d6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="899d6-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="899d6-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="899d6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="899d6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="899d6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="899d6-116">Not supported.</span></span>    |
|<span data-ttu-id="899d6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="899d6-117">Application</span></span> | <span data-ttu-id="899d6-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="899d6-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="899d6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="899d6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
GET /identityProtection/riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="899d6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="899d6-120">Request headers</span></span>
| <span data-ttu-id="899d6-121">名称</span><span class="sxs-lookup"><span data-stu-id="899d6-121">Name</span></span>      |<span data-ttu-id="899d6-122">说明</span><span class="sxs-lookup"><span data-stu-id="899d6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="899d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="899d6-123">Authorization</span></span>  | <span data-ttu-id="899d6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="899d6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="899d6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="899d6-126">Request body</span></span>
<span data-ttu-id="899d6-127">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="899d6-127">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="899d6-128">响应</span><span class="sxs-lookup"><span data-stu-id="899d6-128">Response</span></span>

<span data-ttu-id="899d6-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="899d6-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="899d6-131">示例</span><span class="sxs-lookup"><span data-stu-id="899d6-131">Examples</span></span>
### <a name="example-1-dismiss-risky-users"></a><span data-ttu-id="899d6-132">示例1：消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="899d6-132">Example 1: Dismiss risky users</span></span>
#### <a name="request"></a><span data-ttu-id="899d6-133">请求</span><span class="sxs-lookup"><span data-stu-id="899d6-133">Request</span></span>
<span data-ttu-id="899d6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="899d6-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="899d6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="899d6-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="899d6-136">C#</span><span class="sxs-lookup"><span data-stu-id="899d6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="899d6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="899d6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="899d6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="899d6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="899d6-139">Java</span><span class="sxs-lookup"><span data-stu-id="899d6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="899d6-140">响应</span><span class="sxs-lookup"><span data-stu-id="899d6-140">Response</span></span>
<span data-ttu-id="899d6-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="899d6-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-dismiss-a-risky-user"></a><span data-ttu-id="899d6-142">示例2：消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="899d6-142">Example 2: Dismiss a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="899d6-143">请求</span><span class="sxs-lookup"><span data-stu-id="899d6-143">Request</span></span>
<span data-ttu-id="899d6-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="899d6-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="899d6-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="899d6-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="899d6-146">C#</span><span class="sxs-lookup"><span data-stu-id="899d6-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="899d6-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="899d6-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="899d6-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="899d6-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="899d6-149">Java</span><span class="sxs-lookup"><span data-stu-id="899d6-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/dismiss-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="899d6-150">响应</span><span class="sxs-lookup"><span data-stu-id="899d6-150">Response</span></span>
<span data-ttu-id="899d6-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="899d6-151">Here is an example of the response.</span></span>
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


