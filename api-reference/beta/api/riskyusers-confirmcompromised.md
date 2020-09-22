---
title: 确认 riskyUser 已泄露
description: 确认 riskyUser 对象是否已泄露。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 9954565c2be8b239671d74e55e875ea2b01c229b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085323"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="e12b9-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="e12b9-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="e12b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e12b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="e12b9-105">**注意：** RiskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="e12b9-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="e12b9-106">确认一个或多个 [riskyUser](../resources/riskyuser.md) 对象已泄露。</span><span class="sxs-lookup"><span data-stu-id="e12b9-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="e12b9-107">此操作将目标用户的风险级别设置为 "高"。</span><span class="sxs-lookup"><span data-stu-id="e12b9-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="e12b9-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="e12b9-108">Permissions</span></span>
<span data-ttu-id="e12b9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e12b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e12b9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e12b9-111">Permission type</span></span>      | <span data-ttu-id="e12b9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e12b9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e12b9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e12b9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e12b9-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e12b9-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="e12b9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e12b9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e12b9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e12b9-116">Not supported.</span></span>    |
|<span data-ttu-id="e12b9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e12b9-117">Application</span></span> | <span data-ttu-id="e12b9-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e12b9-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e12b9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e12b9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
POST /identityProtection/riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="e12b9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e12b9-120">Request headers</span></span>
| <span data-ttu-id="e12b9-121">名称</span><span class="sxs-lookup"><span data-stu-id="e12b9-121">Name</span></span>      |<span data-ttu-id="e12b9-122">说明</span><span class="sxs-lookup"><span data-stu-id="e12b9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e12b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e12b9-123">Authorization</span></span>  | <span data-ttu-id="e12b9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e12b9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e12b9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e12b9-126">Request body</span></span>
<span data-ttu-id="e12b9-127">指定要在请求正文中消除的有风险的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="e12b9-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="e12b9-128">响应</span><span class="sxs-lookup"><span data-stu-id="e12b9-128">Response</span></span>

<span data-ttu-id="e12b9-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e12b9-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="e12b9-131">示例</span><span class="sxs-lookup"><span data-stu-id="e12b9-131">Examples</span></span>
### <a name="example-1-confirm-users-as-compromised"></a><span data-ttu-id="e12b9-132">示例1：确认用户受到威胁</span><span class="sxs-lookup"><span data-stu-id="e12b9-132">Example 1: Confirm users as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="e12b9-133">请求</span><span class="sxs-lookup"><span data-stu-id="e12b9-133">Request</span></span>
<span data-ttu-id="e12b9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e12b9-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e12b9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e12b9-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e12b9-136">C#</span><span class="sxs-lookup"><span data-stu-id="e12b9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e12b9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e12b9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e12b9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e12b9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e12b9-139">响应</span><span class="sxs-lookup"><span data-stu-id="e12b9-139">Response</span></span>
<span data-ttu-id="e12b9-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e12b9-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
### <a name="example-2-confirm-a-user-as-compromised"></a><span data-ttu-id="e12b9-141">示例2：确认用户已受到攻击</span><span class="sxs-lookup"><span data-stu-id="e12b9-141">Example 2: Confirm a user as compromised</span></span>
#### <a name="request"></a><span data-ttu-id="e12b9-142">请求</span><span class="sxs-lookup"><span data-stu-id="e12b9-142">Request</span></span>
<span data-ttu-id="e12b9-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e12b9-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e12b9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e12b9-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e12b9-145">C#</span><span class="sxs-lookup"><span data-stu-id="e12b9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e12b9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e12b9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e12b9-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e12b9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e12b9-148">响应</span><span class="sxs-lookup"><span data-stu-id="e12b9-148">Response</span></span>
<span data-ttu-id="e12b9-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e12b9-149">Here is an example of the response.</span></span>
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


