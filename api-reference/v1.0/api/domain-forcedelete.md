---
title: 强制域删除
description: 使用异步长时间运行的操作删除域。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b50957082fe4f2e1e0a87d24cf36a7a7fc6eed16
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181341"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="afd36-103">强制域删除</span><span class="sxs-lookup"><span data-stu-id="afd36-103">Force domain deletion</span></span>

<span data-ttu-id="afd36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afd36-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="afd36-105">使用异步长时间运行的操作删除域。</span><span class="sxs-lookup"><span data-stu-id="afd36-105">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="afd36-106">在此操作过程中，将执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="afd36-106">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="afd36-107">通过将`userPrincipalName`对`mail`已删除`proxyAddresses`域的引用的、和属性更新为使用初始 onmicrosoft.com 域。 `users`</span><span class="sxs-lookup"><span data-stu-id="afd36-107">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="afd36-108">将`groups`包含`mail`对已删除域的引用的属性更新为使用初始 onmicrosoft.com 域。</span><span class="sxs-lookup"><span data-stu-id="afd36-108">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="afd36-109">将`applications`包含`identifierUris`对已删除域的引用的属性更新为使用初始 onmicrosoft.com 域。</span><span class="sxs-lookup"><span data-stu-id="afd36-109">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="afd36-110">如果要重命名的对象的数量大于1000，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="afd36-110">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="afd36-111">如果要重命名`applications`的其中一个是多租户应用，则会返回错误。</span><span class="sxs-lookup"><span data-stu-id="afd36-111">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="afd36-112">域删除完成后，已删除域的 API 操作将返回 HTTP 404 状态代码。</span><span class="sxs-lookup"><span data-stu-id="afd36-112">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="afd36-113">若要验证域的删除，您可以执行 "[获取域](domain-get.md)" 操作。</span><span class="sxs-lookup"><span data-stu-id="afd36-113">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="afd36-114">权限</span><span class="sxs-lookup"><span data-stu-id="afd36-114">Permissions</span></span>

<span data-ttu-id="afd36-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afd36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afd36-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="afd36-117">Permission type</span></span>      | <span data-ttu-id="afd36-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="afd36-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afd36-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afd36-119">Delegated (work or school account)</span></span> | <span data-ttu-id="afd36-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="afd36-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="afd36-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afd36-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afd36-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="afd36-122">Not supported.</span></span>    |
|<span data-ttu-id="afd36-123">Application</span><span class="sxs-lookup"><span data-stu-id="afd36-123">Application</span></span> | <span data-ttu-id="afd36-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afd36-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afd36-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afd36-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="afd36-126">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="afd36-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afd36-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="afd36-127">Request headers</span></span>

| <span data-ttu-id="afd36-128">名称</span><span class="sxs-lookup"><span data-stu-id="afd36-128">Name</span></span> | <span data-ttu-id="afd36-129">说明</span><span class="sxs-lookup"><span data-stu-id="afd36-129">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="afd36-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="afd36-130">Authorization</span></span>  | <span data-ttu-id="afd36-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="afd36-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="afd36-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afd36-133">Content-Type</span></span>  | <span data-ttu-id="afd36-134">application/json</span><span class="sxs-lookup"><span data-stu-id="afd36-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="afd36-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="afd36-135">Request body</span></span>

<span data-ttu-id="afd36-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="afd36-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="afd36-137">参数</span><span class="sxs-lookup"><span data-stu-id="afd36-137">Parameter</span></span> | <span data-ttu-id="afd36-138">类型</span><span class="sxs-lookup"><span data-stu-id="afd36-138">Type</span></span> | <span data-ttu-id="afd36-139">说明</span><span class="sxs-lookup"><span data-stu-id="afd36-139">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="afd36-140">禁用重命名的用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="afd36-140">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="afd36-141">如果用户帐户已禁用，则不允许用户登录。</span><span class="sxs-lookup"><span data-stu-id="afd36-141">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="afd36-142">如果设置为**true** ， `users`则将禁用作为此操作的一部分进行更新的。</span><span class="sxs-lookup"><span data-stu-id="afd36-142">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="afd36-143">默认值为 **True**。</span><span class="sxs-lookup"><span data-stu-id="afd36-143">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="afd36-144">响应正文</span><span class="sxs-lookup"><span data-stu-id="afd36-144">Response body</span></span>

<span data-ttu-id="afd36-145">如果成功，此方法将`HTTP/1.1 204 OK`返回状态代码。</span><span class="sxs-lookup"><span data-stu-id="afd36-145">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="afd36-146">示例</span><span class="sxs-lookup"><span data-stu-id="afd36-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="afd36-147">请求</span><span class="sxs-lookup"><span data-stu-id="afd36-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="afd36-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="afd36-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="afd36-149">C#</span><span class="sxs-lookup"><span data-stu-id="afd36-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afd36-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afd36-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afd36-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afd36-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="afd36-152">响应</span><span class="sxs-lookup"><span data-stu-id="afd36-152">Response</span></span>

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
