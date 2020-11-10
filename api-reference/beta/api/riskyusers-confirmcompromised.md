---
title: 确认 riskyUser 已泄露
description: 确认 riskyUser 对象是否已泄露。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: d9f3b141144654e21c47c523c46a3329865c7031
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970939"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="652a7-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="652a7-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="652a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="652a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="652a7-105">**注意：** RiskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="652a7-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="652a7-106">确认一个或多个 [riskyUser](../resources/riskyuser.md) 对象已泄露。</span><span class="sxs-lookup"><span data-stu-id="652a7-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="652a7-107">此操作将目标用户的风险级别设置为 "高"。</span><span class="sxs-lookup"><span data-stu-id="652a7-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="652a7-108">权限</span><span class="sxs-lookup"><span data-stu-id="652a7-108">Permissions</span></span>
<span data-ttu-id="652a7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="652a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="652a7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="652a7-111">Permission type</span></span>      | <span data-ttu-id="652a7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="652a7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="652a7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="652a7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="652a7-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="652a7-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="652a7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="652a7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="652a7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="652a7-116">Not supported.</span></span>    |
|<span data-ttu-id="652a7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="652a7-117">Application</span></span> | <span data-ttu-id="652a7-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="652a7-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="652a7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="652a7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
POST /identityProtection/riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="652a7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="652a7-120">Request headers</span></span>
| <span data-ttu-id="652a7-121">名称</span><span class="sxs-lookup"><span data-stu-id="652a7-121">Name</span></span>      |<span data-ttu-id="652a7-122">说明</span><span class="sxs-lookup"><span data-stu-id="652a7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="652a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="652a7-123">Authorization</span></span>  | <span data-ttu-id="652a7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="652a7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="652a7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="652a7-126">Request body</span></span>
<span data-ttu-id="652a7-127">指定要在请求正文中消除的有风险的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="652a7-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="652a7-128">响应</span><span class="sxs-lookup"><span data-stu-id="652a7-128">Response</span></span>

<span data-ttu-id="652a7-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="652a7-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="652a7-131">示例</span><span class="sxs-lookup"><span data-stu-id="652a7-131">Examples</span></span>
### <a name="example-1-confirm-users-as-compromised"></a><span data-ttu-id="652a7-132">示例1：确认用户受到威胁</span><span class="sxs-lookup"><span data-stu-id="652a7-132">Example 1: Confirm users as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="652a7-133">请求</span><span class="sxs-lookup"><span data-stu-id="652a7-133">Request</span></span>
<span data-ttu-id="652a7-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="652a7-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="652a7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="652a7-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="652a7-136">C#</span><span class="sxs-lookup"><span data-stu-id="652a7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="652a7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="652a7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="652a7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="652a7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="652a7-139">Java</span><span class="sxs-lookup"><span data-stu-id="652a7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="652a7-140">响应</span><span class="sxs-lookup"><span data-stu-id="652a7-140">Response</span></span>
<span data-ttu-id="652a7-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="652a7-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
### <a name="example-2-confirm-a-user-as-compromised"></a><span data-ttu-id="652a7-142">示例2：确认用户已受到攻击</span><span class="sxs-lookup"><span data-stu-id="652a7-142">Example 2: Confirm a user as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="652a7-143">请求</span><span class="sxs-lookup"><span data-stu-id="652a7-143">Request</span></span>
<span data-ttu-id="652a7-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="652a7-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="652a7-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="652a7-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="652a7-146">C#</span><span class="sxs-lookup"><span data-stu-id="652a7-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="652a7-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="652a7-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="652a7-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="652a7-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="652a7-149">Java</span><span class="sxs-lookup"><span data-stu-id="652a7-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="652a7-150">响应</span><span class="sxs-lookup"><span data-stu-id="652a7-150">Response</span></span>
<span data-ttu-id="652a7-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="652a7-151">Here is an example of the response.</span></span>
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


