---
title: 确认 riskyUser 已泄露
description: 确认 riskyUser 对象是否已泄露。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 51634a1a87dd2ba2c77544dcd461b6051babca66
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863318"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="19784-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="19784-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="19784-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19784-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="19784-105">**注意：** RiskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="19784-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="19784-106">确认一个或多个[riskyUser](../resources/riskyuser.md)对象已泄露。</span><span class="sxs-lookup"><span data-stu-id="19784-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="19784-107">此操作将目标用户的风险级别设置为 "高"。</span><span class="sxs-lookup"><span data-stu-id="19784-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="19784-108">权限</span><span class="sxs-lookup"><span data-stu-id="19784-108">Permissions</span></span>
<span data-ttu-id="19784-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="19784-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="19784-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19784-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19784-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="19784-111">Permission type</span></span>      | <span data-ttu-id="19784-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19784-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19784-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19784-113">Delegated (work or school account)</span></span> | <span data-ttu-id="19784-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19784-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="19784-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19784-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19784-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19784-116">Not supported.</span></span>    |
|<span data-ttu-id="19784-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="19784-117">Application</span></span> | <span data-ttu-id="19784-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19784-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19784-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19784-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
POST /identityProtection/riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="19784-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="19784-120">Request headers</span></span>
| <span data-ttu-id="19784-121">名称</span><span class="sxs-lookup"><span data-stu-id="19784-121">Name</span></span>      |<span data-ttu-id="19784-122">说明</span><span class="sxs-lookup"><span data-stu-id="19784-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19784-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19784-123">Authorization</span></span>  | <span data-ttu-id="19784-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="19784-124">Bearer {token}.</span></span> <span data-ttu-id="19784-125">Required.</span><span class="sxs-lookup"><span data-stu-id="19784-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19784-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="19784-126">Request body</span></span>
<span data-ttu-id="19784-127">指定要在请求正文中消除的有风险的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="19784-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="19784-128">响应</span><span class="sxs-lookup"><span data-stu-id="19784-128">Response</span></span>

<span data-ttu-id="19784-129">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="19784-129">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="19784-130">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="19784-130">It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="19784-131">示例</span><span class="sxs-lookup"><span data-stu-id="19784-131">Examples</span></span>
### <a name="example-1-confirm-users-as-compromised"></a><span data-ttu-id="19784-132">示例1：确认用户受到威胁</span><span class="sxs-lookup"><span data-stu-id="19784-132">Example 1: Confirm users as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="19784-133">请求</span><span class="sxs-lookup"><span data-stu-id="19784-133">Request</span></span>
<span data-ttu-id="19784-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19784-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19784-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="19784-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="19784-136">C#</span><span class="sxs-lookup"><span data-stu-id="19784-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19784-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19784-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19784-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19784-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="19784-139">响应</span><span class="sxs-lookup"><span data-stu-id="19784-139">Response</span></span>
<span data-ttu-id="19784-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="19784-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
### <a name="example-2-confirm-a-user-as-compromised"></a><span data-ttu-id="19784-141">示例2：确认用户已受到攻击</span><span class="sxs-lookup"><span data-stu-id="19784-141">Example 2: Confirm a user as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="19784-142">请求</span><span class="sxs-lookup"><span data-stu-id="19784-142">Request</span></span>
<span data-ttu-id="19784-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19784-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19784-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="19784-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/identityProtection/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="19784-145">C#</span><span class="sxs-lookup"><span data-stu-id="19784-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19784-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19784-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19784-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19784-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="19784-148">响应</span><span class="sxs-lookup"><span data-stu-id="19784-148">Response</span></span>
<span data-ttu-id="19784-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="19784-149">Here is an example of the response.</span></span>
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
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
