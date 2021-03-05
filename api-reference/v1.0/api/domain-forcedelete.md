---
title: 强制删除域
description: 使用异步长时间运行的操作删除域。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a4376961ea843c5c512d5bdf59449a7e765399f0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441975"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="49584-103">强制删除域</span><span class="sxs-lookup"><span data-stu-id="49584-103">Force domain deletion</span></span>

<span data-ttu-id="49584-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49584-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49584-105">使用异步长时间运行的操作删除域。</span><span class="sxs-lookup"><span data-stu-id="49584-105">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="49584-106">在调用 [forceDelete](domain-forcedelete.md)之前，必须更新或删除对 **Exchange** 作为预配服务的任何引用。</span><span class="sxs-lookup"><span data-stu-id="49584-106">Prior to calling [forceDelete](domain-forcedelete.md), you must update or remove any references to **Exchange** as the provisioning service.</span></span>

<span data-ttu-id="49584-107">以下操作作为此操作的一部分执行：</span><span class="sxs-lookup"><span data-stu-id="49584-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="49584-108">使用 `userPrincipalName` 对已删除域的引用更新的 、和属性，以使用onmicrosoft.com `mail` `proxyAddresses` `users` 域。</span><span class="sxs-lookup"><span data-stu-id="49584-108">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="49584-109">使用 `mail` 对 `groups` 已删除域的引用更新其属性，以使用初始onmicrosoft.com域。</span><span class="sxs-lookup"><span data-stu-id="49584-109">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="49584-110">使用 `identifierUris` 对 `applications` 已删除域的引用更新其属性，以使用初始onmicrosoft.com域。</span><span class="sxs-lookup"><span data-stu-id="49584-110">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="49584-111">如果要重命名的对象数大于 1000，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="49584-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="49584-112">如果要重命名 `applications` 的其中一个应用是多租户应用，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="49584-112">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="49584-113">域删除完成后，已删除域的 API 操作将返回 HTTP 404 状态代码。</span><span class="sxs-lookup"><span data-stu-id="49584-113">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="49584-114">若要验证删除域，可以执行 [get 域](domain-get.md) 操作。</span><span class="sxs-lookup"><span data-stu-id="49584-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="49584-115">权限</span><span class="sxs-lookup"><span data-stu-id="49584-115">Permissions</span></span>

<span data-ttu-id="49584-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49584-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49584-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="49584-118">Permission type</span></span>      | <span data-ttu-id="49584-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49584-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49584-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49584-120">Delegated (work or school account)</span></span> | <span data-ttu-id="49584-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49584-121">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49584-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49584-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49584-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="49584-123">Not supported.</span></span>    |
|<span data-ttu-id="49584-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="49584-124">Application</span></span> | <span data-ttu-id="49584-125">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49584-125">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49584-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49584-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="49584-127">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="49584-127">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49584-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="49584-128">Request headers</span></span>

| <span data-ttu-id="49584-129">名称</span><span class="sxs-lookup"><span data-stu-id="49584-129">Name</span></span> | <span data-ttu-id="49584-130">说明</span><span class="sxs-lookup"><span data-stu-id="49584-130">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="49584-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="49584-131">Authorization</span></span>  | <span data-ttu-id="49584-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49584-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="49584-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49584-134">Content-Type</span></span>  | <span data-ttu-id="49584-135">application/json</span><span class="sxs-lookup"><span data-stu-id="49584-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="49584-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="49584-136">Request body</span></span>

<span data-ttu-id="49584-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="49584-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49584-138">参数</span><span class="sxs-lookup"><span data-stu-id="49584-138">Parameter</span></span> | <span data-ttu-id="49584-139">类型</span><span class="sxs-lookup"><span data-stu-id="49584-139">Type</span></span> | <span data-ttu-id="49584-140">说明</span><span class="sxs-lookup"><span data-stu-id="49584-140">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="49584-141">用于禁用重命名的用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="49584-141">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="49584-142">如果禁用用户帐户，则不允许用户登录。</span><span class="sxs-lookup"><span data-stu-id="49584-142">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="49584-143">如果设置为 **true，** `users` 将禁用作为此操作的一部分进行更新。</span><span class="sxs-lookup"><span data-stu-id="49584-143">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="49584-144">默认值为 **True**。</span><span class="sxs-lookup"><span data-stu-id="49584-144">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="49584-145">响应正文</span><span class="sxs-lookup"><span data-stu-id="49584-145">Response body</span></span>

<span data-ttu-id="49584-146">如果成功，此方法将返回 `HTTP/1.1 204 OK` 状态代码。</span><span class="sxs-lookup"><span data-stu-id="49584-146">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="49584-147">示例</span><span class="sxs-lookup"><span data-stu-id="49584-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="49584-148">请求</span><span class="sxs-lookup"><span data-stu-id="49584-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49584-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="49584-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/v1.0/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="c"></a>[<span data-ttu-id="49584-150">C#</span><span class="sxs-lookup"><span data-stu-id="49584-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49584-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49584-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49584-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49584-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49584-153">Java</span><span class="sxs-lookup"><span data-stu-id="49584-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49584-154">响应</span><span class="sxs-lookup"><span data-stu-id="49584-154">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

