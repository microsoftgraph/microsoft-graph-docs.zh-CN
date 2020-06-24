---
title: 消除 riskyUser
description: 消除 riskyUser 对象的风险。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 3a549ca4b50d1a0e873a905a6312e30d6bf1e838
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863514"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="84a1f-103">riskyUser：消除</span><span class="sxs-lookup"><span data-stu-id="84a1f-103">riskyUser: dismiss</span></span>

<span data-ttu-id="84a1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84a1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="84a1f-105">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="84a1f-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="84a1f-106">消除一个或多个[riskyUser](../resources/riskyuser.md)对象的风险。</span><span class="sxs-lookup"><span data-stu-id="84a1f-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="84a1f-107">此操作将目标用户的风险级别设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="84a1f-107">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="84a1f-108">权限</span><span class="sxs-lookup"><span data-stu-id="84a1f-108">Permissions</span></span>
<span data-ttu-id="84a1f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="84a1f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="84a1f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84a1f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84a1f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="84a1f-111">Permission type</span></span>      | <span data-ttu-id="84a1f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84a1f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84a1f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84a1f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="84a1f-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a1f-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="84a1f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84a1f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84a1f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="84a1f-116">Not supported.</span></span>    |
|<span data-ttu-id="84a1f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="84a1f-117">Application</span></span> | <span data-ttu-id="84a1f-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a1f-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84a1f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84a1f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
GET /identityProtection/riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="84a1f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="84a1f-120">Request headers</span></span>
| <span data-ttu-id="84a1f-121">名称</span><span class="sxs-lookup"><span data-stu-id="84a1f-121">Name</span></span>      |<span data-ttu-id="84a1f-122">说明</span><span class="sxs-lookup"><span data-stu-id="84a1f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84a1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84a1f-123">Authorization</span></span>  | <span data-ttu-id="84a1f-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="84a1f-124">Bearer {token}.</span></span> <span data-ttu-id="84a1f-125">Required.</span><span class="sxs-lookup"><span data-stu-id="84a1f-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84a1f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="84a1f-126">Request body</span></span>
<span data-ttu-id="84a1f-127">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="84a1f-127">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="84a1f-128">响应</span><span class="sxs-lookup"><span data-stu-id="84a1f-128">Response</span></span>

<span data-ttu-id="84a1f-129">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="84a1f-129">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="84a1f-130">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="84a1f-130">It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="84a1f-131">示例</span><span class="sxs-lookup"><span data-stu-id="84a1f-131">Examples</span></span>
### <a name="example-1-dismiss-risky-users"></a><span data-ttu-id="84a1f-132">示例1：消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="84a1f-132">Example 1: Dismiss risky users</span></span>
#### <a name="request"></a><span data-ttu-id="84a1f-133">请求</span><span class="sxs-lookup"><span data-stu-id="84a1f-133">Request</span></span>
<span data-ttu-id="84a1f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84a1f-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84a1f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="84a1f-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="84a1f-136">C#</span><span class="sxs-lookup"><span data-stu-id="84a1f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84a1f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84a1f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84a1f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84a1f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="84a1f-139">响应</span><span class="sxs-lookup"><span data-stu-id="84a1f-139">Response</span></span>
<span data-ttu-id="84a1f-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="84a1f-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-dismiss-a-risky-user"></a><span data-ttu-id="84a1f-141">示例2：消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="84a1f-141">Example 2: Dismiss a risky user</span></span>
#### <a name="request"></a><span data-ttu-id="84a1f-142">请求</span><span class="sxs-lookup"><span data-stu-id="84a1f-142">Request</span></span>
<span data-ttu-id="84a1f-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84a1f-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84a1f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="84a1f-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="84a1f-145">C#</span><span class="sxs-lookup"><span data-stu-id="84a1f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84a1f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84a1f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84a1f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84a1f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="84a1f-148">响应</span><span class="sxs-lookup"><span data-stu-id="84a1f-148">Response</span></span>
<span data-ttu-id="84a1f-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="84a1f-149">Here is an example of the response.</span></span>
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
