---
title: 强制域删除
description: 删除使用长时间运行的异步操作的域。
ms.openlocfilehash: 20f00679998070b95af65292cadf83d76aa2add1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011552"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="4b0cc-103">强制域删除</span><span class="sxs-lookup"><span data-stu-id="4b0cc-103">Force domain deletion</span></span>

<span data-ttu-id="4b0cc-104">删除使用长时间运行的异步操作的域。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="4b0cc-105">此操作的一部分执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="4b0cc-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="4b0cc-106">更新`userPrincipalName`， `mail`，和`proxyAddresses`属性`users`与要使用初始 onmicrosoft.com 域的已删除域的引用。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="4b0cc-107">更新`mail`属性`groups`与要使用初始 onmicrosoft.com 域的已删除域的引用。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="4b0cc-108">更新`identifierUris`属性`applications`与要使用初始 onmicrosoft.com 域的已删除域的引用。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="4b0cc-109">如果要重命名的对象的数量大于 1000年，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="4b0cc-110">如果的`applications`要重命名为多租户应用程序，则返回一个错误。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="4b0cc-111">域删除完成后，已删除的域的 API 操作将返回 HTTP 404 状态代码。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="4b0cc-112">若要验证删除的域，可以执行[get 域](domain-get.md)操作。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b0cc-113">权限</span><span class="sxs-lookup"><span data-stu-id="4b0cc-113">Permissions</span></span>

<span data-ttu-id="4b0cc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b0cc-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b0cc-116">Permission type</span></span>      | <span data-ttu-id="4b0cc-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b0cc-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b0cc-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b0cc-118">Delegated (work or school account)</span></span> | <span data-ttu-id="4b0cc-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b0cc-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4b0cc-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b0cc-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b0cc-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-121">Not supported.</span></span>    |
|<span data-ttu-id="4b0cc-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b0cc-122">Application</span></span> | <span data-ttu-id="4b0cc-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b0cc-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b0cc-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b0cc-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="4b0cc-125">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b0cc-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b0cc-126">Request headers</span></span>

| <span data-ttu-id="4b0cc-127">名称</span><span class="sxs-lookup"><span data-stu-id="4b0cc-127">Name</span></span> | <span data-ttu-id="4b0cc-128">说明</span><span class="sxs-lookup"><span data-stu-id="4b0cc-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4b0cc-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b0cc-129">Authorization</span></span>  | <span data-ttu-id="4b0cc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4b0cc-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b0cc-132">Content-Type</span></span>  | <span data-ttu-id="4b0cc-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4b0cc-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b0cc-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b0cc-134">Request body</span></span>

<span data-ttu-id="4b0cc-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4b0cc-136">参数</span><span class="sxs-lookup"><span data-stu-id="4b0cc-136">Parameter</span></span> | <span data-ttu-id="4b0cc-137">类型</span><span class="sxs-lookup"><span data-stu-id="4b0cc-137">Type</span></span> | <span data-ttu-id="4b0cc-138">说明</span><span class="sxs-lookup"><span data-stu-id="4b0cc-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="4b0cc-139">若要禁用其重命名用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="4b0cc-140">如果禁用的用户帐户，则用户将不允许登录。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="4b0cc-141">如果设置为**true** `users`更新为属于此操作将被禁用。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="4b0cc-142">默认值为**true**。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="4b0cc-143">响应正文</span><span class="sxs-lookup"><span data-stu-id="4b0cc-143">Response body</span></span>

<span data-ttu-id="4b0cc-144">如果成功，此方法返回`HTTP/1.1 204 OK`状态代码。</span><span class="sxs-lookup"><span data-stu-id="4b0cc-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="4b0cc-145">示例</span><span class="sxs-lookup"><span data-stu-id="4b0cc-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b0cc-146">请求</span><span class="sxs-lookup"><span data-stu-id="4b0cc-146">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="4b0cc-147">响应</span><span class="sxs-lookup"><span data-stu-id="4b0cc-147">Response</span></span>

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
  "tocPath": ""
}-->