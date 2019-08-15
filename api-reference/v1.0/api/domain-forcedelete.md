---
title: 强制域删除
description: 使用异步长时间运行的操作删除域。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fd00353777b908cc80a77e75878bbac0240ed490
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422287"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="9a8a3-103">强制域删除</span><span class="sxs-lookup"><span data-stu-id="9a8a3-103">Force domain deletion</span></span>

<span data-ttu-id="9a8a3-104">使用异步长时间运行的操作删除域。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="9a8a3-105">在此操作过程中, 将执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="9a8a3-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="9a8a3-106">通过将`userPrincipalName`对`mail`已删除`proxyAddresses`域的引用的、和属性更新为使用初始 onmicrosoft.com 域。 `users`</span><span class="sxs-lookup"><span data-stu-id="9a8a3-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="9a8a3-107">将`groups`包含`mail`对已删除域的引用的属性更新为使用初始 onmicrosoft.com 域。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="9a8a3-108">将`applications`包含`identifierUris`对已删除域的引用的属性更新为使用初始 onmicrosoft.com 域。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="9a8a3-109">如果要重命名的对象的数量大于 1000, 则返回错误。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="9a8a3-110">如果要重命名`applications`的其中一个是多租户应用, 则会返回错误。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="9a8a3-111">域删除完成后, 已删除域的 API 操作将返回 HTTP 404 状态代码。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="9a8a3-112">若要验证域的删除, 您可以执行 "[获取域](domain-get.md)" 操作。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a8a3-113">权限</span><span class="sxs-lookup"><span data-stu-id="9a8a3-113">Permissions</span></span>

<span data-ttu-id="9a8a3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a8a3-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a8a3-116">Permission type</span></span>      | <span data-ttu-id="9a8a3-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a8a3-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a8a3-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a8a3-118">Delegated (work or school account)</span></span> | <span data-ttu-id="9a8a3-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a8a3-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a8a3-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a8a3-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a8a3-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-121">Not supported.</span></span>    |
|<span data-ttu-id="9a8a3-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a8a3-122">Application</span></span> | <span data-ttu-id="9a8a3-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8a3-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a8a3-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a8a3-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="9a8a3-125">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a8a3-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a8a3-126">Request headers</span></span>

| <span data-ttu-id="9a8a3-127">名称</span><span class="sxs-lookup"><span data-stu-id="9a8a3-127">Name</span></span> | <span data-ttu-id="9a8a3-128">说明</span><span class="sxs-lookup"><span data-stu-id="9a8a3-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9a8a3-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a8a3-129">Authorization</span></span>  | <span data-ttu-id="9a8a3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9a8a3-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a8a3-132">Content-Type</span></span>  | <span data-ttu-id="9a8a3-133">application/json</span><span class="sxs-lookup"><span data-stu-id="9a8a3-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a8a3-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a8a3-134">Request body</span></span>

<span data-ttu-id="9a8a3-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9a8a3-136">参数</span><span class="sxs-lookup"><span data-stu-id="9a8a3-136">Parameter</span></span> | <span data-ttu-id="9a8a3-137">类型</span><span class="sxs-lookup"><span data-stu-id="9a8a3-137">Type</span></span> | <span data-ttu-id="9a8a3-138">说明</span><span class="sxs-lookup"><span data-stu-id="9a8a3-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="9a8a3-139">禁用重命名的用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="9a8a3-140">如果用户帐户已禁用, 则不允许用户登录。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="9a8a3-141">如果设置为**true** , `users`则将禁用作为此操作的一部分进行更新的。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="9a8a3-142">默认值为 **True**。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="9a8a3-143">响应正文</span><span class="sxs-lookup"><span data-stu-id="9a8a3-143">Response body</span></span>

<span data-ttu-id="9a8a3-144">如果成功, 此方法将`HTTP/1.1 204 OK`返回状态代码。</span><span class="sxs-lookup"><span data-stu-id="9a8a3-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="9a8a3-145">示例</span><span class="sxs-lookup"><span data-stu-id="9a8a3-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a8a3-146">请求</span><span class="sxs-lookup"><span data-stu-id="9a8a3-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9a8a3-147">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9a8a3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a8a3-148">C#</span><span class="sxs-lookup"><span data-stu-id="9a8a3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a8a3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a8a3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a8a3-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="9a8a3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a8a3-151">响应</span><span class="sxs-lookup"><span data-stu-id="9a8a3-151">Response</span></span>

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
