---
title: 域：forceDelete
description: 使用异步操作删除域。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fc074f3160ef8260f04fe2795a58a0ddfd1c54d7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131262"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="01d00-103">域：forceDelete</span><span class="sxs-lookup"><span data-stu-id="01d00-103">domain: forceDelete</span></span>

<span data-ttu-id="01d00-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01d00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01d00-105">使用异步操作删除域。</span><span class="sxs-lookup"><span data-stu-id="01d00-105">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="01d00-106">在调用 [forceDelete](domain-forcedelete.md)之前，必须更新或删除对 **Exchange** 作为设置服务的任何引用。</span><span class="sxs-lookup"><span data-stu-id="01d00-106">Prior to calling [forceDelete](domain-forcedelete.md), you must update or remove any references to **Exchange** as the provisioning service.</span></span>

<span data-ttu-id="01d00-107">以下操作作为此操作的一部分执行：</span><span class="sxs-lookup"><span data-stu-id="01d00-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="01d00-108">使用对已删除域的引用重命名用户的 UPN、EmailAddress 和 ProxyAddress。</span><span class="sxs-lookup"><span data-stu-id="01d00-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="01d00-109">使用对已删除域的引用重命名组的 EmailAddress。</span><span class="sxs-lookup"><span data-stu-id="01d00-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="01d00-110">使用对已删除域的引用重命名应用程序的 identifierUri。</span><span class="sxs-lookup"><span data-stu-id="01d00-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="01d00-111">如果要重命名的对象数大于 1，000，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="01d00-111">If the number of objects to be renamed is greater than 1,000, an error is returned.</span></span>

* <span data-ttu-id="01d00-112">如果要重命名的应用程序之一是多租户应用，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="01d00-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="01d00-113">域删除完成后，已删除域的 API 操作将返回 404 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="01d00-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="01d00-114">若要验证是否删除域，可以执行 [获取域](domain-get.md)。</span><span class="sxs-lookup"><span data-stu-id="01d00-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="01d00-115">如果域已成功删除，响应中将返回 404 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="01d00-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="01d00-116">权限</span><span class="sxs-lookup"><span data-stu-id="01d00-116">Permissions</span></span>

<span data-ttu-id="01d00-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01d00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="01d00-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="01d00-119">Permission type</span></span>      | <span data-ttu-id="01d00-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01d00-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01d00-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01d00-121">Delegated (work or school account)</span></span> | <span data-ttu-id="01d00-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01d00-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01d00-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01d00-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01d00-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="01d00-124">Not supported.</span></span>    |
|<span data-ttu-id="01d00-125">Application</span><span class="sxs-lookup"><span data-stu-id="01d00-125">Application</span></span> | <span data-ttu-id="01d00-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d00-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01d00-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01d00-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="01d00-128">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="01d00-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01d00-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="01d00-129">Request headers</span></span>

| <span data-ttu-id="01d00-130">名称</span><span class="sxs-lookup"><span data-stu-id="01d00-130">Name</span></span>       | <span data-ttu-id="01d00-131">说明</span><span class="sxs-lookup"><span data-stu-id="01d00-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01d00-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="01d00-132">Authorization</span></span>  | <span data-ttu-id="01d00-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01d00-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="01d00-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01d00-135">Content-Type</span></span>  | <span data-ttu-id="01d00-136">application/json</span><span class="sxs-lookup"><span data-stu-id="01d00-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="01d00-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="01d00-137">Request body</span></span>

<span data-ttu-id="01d00-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="01d00-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01d00-139">参数</span><span class="sxs-lookup"><span data-stu-id="01d00-139">Parameter</span></span>    | <span data-ttu-id="01d00-140">类型</span><span class="sxs-lookup"><span data-stu-id="01d00-140">Type</span></span>   |<span data-ttu-id="01d00-141">说明</span><span class="sxs-lookup"><span data-stu-id="01d00-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01d00-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="01d00-142">disableUserAccounts</span></span>|<span data-ttu-id="01d00-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="01d00-143">Boolean</span></span>| <span data-ttu-id="01d00-144">用于禁用重命名的用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="01d00-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="01d00-145">如果用户帐户被禁用，则不允许用户登录。</span><span class="sxs-lookup"><span data-stu-id="01d00-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="01d00-146">*True* (默认值) - 重命名为此操作一部分的用户帐户将被禁用。</span><span class="sxs-lookup"><span data-stu-id="01d00-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="01d00-147">*False* - 不会禁用作为此操作的一部分重命名的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="01d00-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="01d00-148">响应</span><span class="sxs-lookup"><span data-stu-id="01d00-148">Response</span></span>

<span data-ttu-id="01d00-149">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="01d00-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="01d00-150">示例</span><span class="sxs-lookup"><span data-stu-id="01d00-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="01d00-151">请求</span><span class="sxs-lookup"><span data-stu-id="01d00-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="01d00-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="01d00-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="c"></a>[<span data-ttu-id="01d00-153">C#</span><span class="sxs-lookup"><span data-stu-id="01d00-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01d00-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01d00-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01d00-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01d00-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01d00-156">Java</span><span class="sxs-lookup"><span data-stu-id="01d00-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01d00-157">响应</span><span class="sxs-lookup"><span data-stu-id="01d00-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


