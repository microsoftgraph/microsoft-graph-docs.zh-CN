---
title: 确认 riskyUser 遭到入侵
description: 确认 riskyUser 对象已泄露。
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: ab156960911b1267ea20e7a46f2cc89fbaf9d37f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950503"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="d829c-103">riskyUser：confirmComprom一</span><span class="sxs-lookup"><span data-stu-id="d829c-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="d829c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d829c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="d829c-105">**注意：** riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="d829c-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="d829c-106">确认一个或多个 [riskyUser](../resources/riskyuser.md) 对象受到威胁。</span><span class="sxs-lookup"><span data-stu-id="d829c-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="d829c-107">此操作将目标用户的风险级别设置得较高。</span><span class="sxs-lookup"><span data-stu-id="d829c-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="d829c-108">权限</span><span class="sxs-lookup"><span data-stu-id="d829c-108">Permissions</span></span>
<span data-ttu-id="d829c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d829c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d829c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d829c-111">Permission type</span></span>      | <span data-ttu-id="d829c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d829c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d829c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d829c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d829c-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d829c-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="d829c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d829c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d829c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d829c-116">Not supported.</span></span>    |
|<span data-ttu-id="d829c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d829c-117">Application</span></span> | <span data-ttu-id="d829c-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d829c-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d829c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d829c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
POST /identityProtection/riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="d829c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d829c-120">Request headers</span></span>
| <span data-ttu-id="d829c-121">名称</span><span class="sxs-lookup"><span data-stu-id="d829c-121">Name</span></span>      |<span data-ttu-id="d829c-122">说明</span><span class="sxs-lookup"><span data-stu-id="d829c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d829c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d829c-123">Authorization</span></span>  | <span data-ttu-id="d829c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d829c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d829c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d829c-126">Request body</span></span>
<span data-ttu-id="d829c-127">在请求正文中指定要消除的风险用户 ID。</span><span class="sxs-lookup"><span data-stu-id="d829c-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="d829c-128">响应</span><span class="sxs-lookup"><span data-stu-id="d829c-128">Response</span></span>

<span data-ttu-id="d829c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d829c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="d829c-131">示例</span><span class="sxs-lookup"><span data-stu-id="d829c-131">Examples</span></span>
### <a name="example-1-confirm-users-as-compromised"></a><span data-ttu-id="d829c-132">示例 1：确认用户受到威胁</span><span class="sxs-lookup"><span data-stu-id="d829c-132">Example 1: Confirm users as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="d829c-133">请求</span><span class="sxs-lookup"><span data-stu-id="d829c-133">Request</span></span>
<span data-ttu-id="d829c-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d829c-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d829c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d829c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser_1"
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
# <a name="c"></a>[<span data-ttu-id="d829c-136">C#</span><span class="sxs-lookup"><span data-stu-id="d829c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d829c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d829c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d829c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d829c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d829c-139">Java</span><span class="sxs-lookup"><span data-stu-id="d829c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d829c-140">响应</span><span class="sxs-lookup"><span data-stu-id="d829c-140">Response</span></span>
<span data-ttu-id="d829c-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d829c-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
### <a name="example-2-confirm-a-user-as-compromised"></a><span data-ttu-id="d829c-142">示例 2：确认用户遭到入侵</span><span class="sxs-lookup"><span data-stu-id="d829c-142">Example 2: Confirm a user as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="d829c-143">请求</span><span class="sxs-lookup"><span data-stu-id="d829c-143">Request</span></span>
<span data-ttu-id="d829c-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d829c-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d829c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d829c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser_2"
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
# <a name="c"></a>[<span data-ttu-id="d829c-146">C#</span><span class="sxs-lookup"><span data-stu-id="d829c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d829c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d829c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d829c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d829c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d829c-149">Java</span><span class="sxs-lookup"><span data-stu-id="d829c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d829c-150">响应</span><span class="sxs-lookup"><span data-stu-id="d829c-150">Response</span></span>
<span data-ttu-id="d829c-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d829c-151">Here is an example of the response.</span></span>
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


