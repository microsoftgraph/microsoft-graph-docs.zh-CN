---
title: 域：forceDelete
description: 使用异步操作删除域。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 47f81a25fc29f6a7eb0bb79c0f4d84e37825183a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786823"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="4a81e-103">域：forceDelete</span><span class="sxs-lookup"><span data-stu-id="4a81e-103">domain: forceDelete</span></span>

<span data-ttu-id="4a81e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a81e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a81e-105">使用异步操作删除域。</span><span class="sxs-lookup"><span data-stu-id="4a81e-105">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="4a81e-106">在调用 [forceDelete](domain-forcedelete.md)之前，必须更新或删除对 **Exchange设置服务** 的任何引用。</span><span class="sxs-lookup"><span data-stu-id="4a81e-106">Prior to calling [forceDelete](domain-forcedelete.md), you must update or remove any references to **Exchange** as the provisioning service.</span></span>

<span data-ttu-id="4a81e-107">以下操作作为此操作的一部分执行：</span><span class="sxs-lookup"><span data-stu-id="4a81e-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="4a81e-108">使用对已删除域的引用重命名用户的 UPN、EmailAddress 和 ProxyAddress。</span><span class="sxs-lookup"><span data-stu-id="4a81e-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="4a81e-109">使用对已删除域的引用重命名组的 EmailAddress。</span><span class="sxs-lookup"><span data-stu-id="4a81e-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="4a81e-110">使用对已删除域的引用重命名应用程序的 identifierUri。</span><span class="sxs-lookup"><span data-stu-id="4a81e-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="4a81e-111">如果要重命名的对象数大于 1，000，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="4a81e-111">If the number of objects to be renamed is greater than 1,000, an error is returned.</span></span>

* <span data-ttu-id="4a81e-112">如果要重命名的应用程序之一是多租户应用，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="4a81e-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="4a81e-113">域删除完成后，已删除域的 API 操作将返回 404 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4a81e-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="4a81e-114">若要验证是否删除域，可以执行获取 [域](domain-get.md)。</span><span class="sxs-lookup"><span data-stu-id="4a81e-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="4a81e-115">如果成功删除域，响应中将返回 404 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4a81e-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a81e-116">权限</span><span class="sxs-lookup"><span data-stu-id="4a81e-116">Permissions</span></span>

<span data-ttu-id="4a81e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a81e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4a81e-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a81e-119">Permission type</span></span>      | <span data-ttu-id="4a81e-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a81e-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a81e-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a81e-121">Delegated (work or school account)</span></span> | <span data-ttu-id="4a81e-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a81e-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a81e-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a81e-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a81e-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a81e-124">Not supported.</span></span>    |
|<span data-ttu-id="4a81e-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a81e-125">Application</span></span> | <span data-ttu-id="4a81e-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a81e-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a81e-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a81e-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="4a81e-128">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="4a81e-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a81e-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a81e-129">Request headers</span></span>

| <span data-ttu-id="4a81e-130">名称</span><span class="sxs-lookup"><span data-stu-id="4a81e-130">Name</span></span>       | <span data-ttu-id="4a81e-131">说明</span><span class="sxs-lookup"><span data-stu-id="4a81e-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a81e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a81e-132">Authorization</span></span>  | <span data-ttu-id="4a81e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a81e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4a81e-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a81e-135">Content-Type</span></span>  | <span data-ttu-id="4a81e-136">application/json</span><span class="sxs-lookup"><span data-stu-id="4a81e-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a81e-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a81e-137">Request body</span></span>

<span data-ttu-id="4a81e-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4a81e-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a81e-139">参数</span><span class="sxs-lookup"><span data-stu-id="4a81e-139">Parameter</span></span>    | <span data-ttu-id="4a81e-140">类型</span><span class="sxs-lookup"><span data-stu-id="4a81e-140">Type</span></span>   |<span data-ttu-id="4a81e-141">说明</span><span class="sxs-lookup"><span data-stu-id="4a81e-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a81e-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="4a81e-142">disableUserAccounts</span></span>|<span data-ttu-id="4a81e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a81e-143">Boolean</span></span>| <span data-ttu-id="4a81e-144">用于禁用重命名的用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="4a81e-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="4a81e-145">如果禁用用户帐户，将不允许用户登录。</span><span class="sxs-lookup"><span data-stu-id="4a81e-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="4a81e-146">*为* (默认) - 已禁用作为此操作的一部分重命名的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="4a81e-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="4a81e-147">*False* - 不会禁用作为此操作的一部分重命名的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="4a81e-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="4a81e-148">响应</span><span class="sxs-lookup"><span data-stu-id="4a81e-148">Response</span></span>

<span data-ttu-id="4a81e-149">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4a81e-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="4a81e-150">示例</span><span class="sxs-lookup"><span data-stu-id="4a81e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a81e-151">请求</span><span class="sxs-lookup"><span data-stu-id="4a81e-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4a81e-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a81e-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4a81e-153">C#</span><span class="sxs-lookup"><span data-stu-id="4a81e-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a81e-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a81e-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a81e-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a81e-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a81e-156">Java</span><span class="sxs-lookup"><span data-stu-id="4a81e-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4a81e-157">响应</span><span class="sxs-lookup"><span data-stu-id="4a81e-157">Response</span></span>

<!-- {
  "blockType": "response"
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


