---
title: 域： forceDelete
description: 使用异步操作删除域。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4daff04db42782a5d9b611d454a5cfb2c12953b1
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180100"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="a4eb7-103">域： forceDelete</span><span class="sxs-lookup"><span data-stu-id="a4eb7-103">domain: forceDelete</span></span>

<span data-ttu-id="a4eb7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4eb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4eb7-105">使用异步操作删除域。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-105">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="a4eb7-106">在此操作过程中，将执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a4eb7-106">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="a4eb7-107">使用对已删除域的引用重命名用户的 UPN、EmailAddress 和 ProxyAddress。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-107">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="a4eb7-108">使用对已删除域的引用重命名组的 EmailAddress。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-108">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="a4eb7-109">将应用程序的 identifierUris 重命名为对已删除的域的引用。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-109">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="a4eb7-110">如果要重命名的对象的数量大于1000，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-110">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="a4eb7-111">如果要重命名的某个应用程序是多租户应用程序，则会返回错误。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-111">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="a4eb7-112">域删除完成后，已删除域的 API 操作将返回 404 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-112">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="a4eb7-113">若要验证域的删除，可以执行[获取域](domain-get.md)。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-113">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="a4eb7-114">如果已成功删除域，响应中将返回 404 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-114">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4eb7-115">权限</span><span class="sxs-lookup"><span data-stu-id="a4eb7-115">Permissions</span></span>

<span data-ttu-id="a4eb7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a4eb7-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4eb7-118">Permission type</span></span>      | <span data-ttu-id="a4eb7-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4eb7-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4eb7-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4eb7-120">Delegated (work or school account)</span></span> | <span data-ttu-id="a4eb7-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4eb7-121">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4eb7-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4eb7-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4eb7-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-123">Not supported.</span></span>    |
|<span data-ttu-id="a4eb7-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4eb7-124">Application</span></span> | <span data-ttu-id="a4eb7-125">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4eb7-125">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4eb7-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4eb7-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="a4eb7-127">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-127">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4eb7-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4eb7-128">Request headers</span></span>

| <span data-ttu-id="a4eb7-129">名称</span><span class="sxs-lookup"><span data-stu-id="a4eb7-129">Name</span></span>       | <span data-ttu-id="a4eb7-130">说明</span><span class="sxs-lookup"><span data-stu-id="a4eb7-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a4eb7-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4eb7-131">Authorization</span></span>  | <span data-ttu-id="a4eb7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a4eb7-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4eb7-134">Content-Type</span></span>  | <span data-ttu-id="a4eb7-135">application/json</span><span class="sxs-lookup"><span data-stu-id="a4eb7-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4eb7-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4eb7-136">Request body</span></span>

<span data-ttu-id="a4eb7-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4eb7-138">参数</span><span class="sxs-lookup"><span data-stu-id="a4eb7-138">Parameter</span></span>    | <span data-ttu-id="a4eb7-139">类型</span><span class="sxs-lookup"><span data-stu-id="a4eb7-139">Type</span></span>   |<span data-ttu-id="a4eb7-140">说明</span><span class="sxs-lookup"><span data-stu-id="a4eb7-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4eb7-141">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="a4eb7-141">disableUserAccounts</span></span>|<span data-ttu-id="a4eb7-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="a4eb7-142">Boolean</span></span>| <span data-ttu-id="a4eb7-143">用于禁用重命名的用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-143">Option to disable renamed user accounts.</span></span> <span data-ttu-id="a4eb7-144">如果用户帐户已禁用，则不允许用户登录。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-144">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="a4eb7-145">*True* （默认值）-在此操作中重命名的用户帐户将被禁用。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-145">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="a4eb7-146">*False* -不禁用作为此操作的一部分重命名的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-146">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="a4eb7-147">响应</span><span class="sxs-lookup"><span data-stu-id="a4eb7-147">Response</span></span>

<span data-ttu-id="a4eb7-148">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a4eb7-148">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="a4eb7-149">示例</span><span class="sxs-lookup"><span data-stu-id="a4eb7-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4eb7-150">请求</span><span class="sxs-lookup"><span data-stu-id="a4eb7-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a4eb7-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4eb7-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a4eb7-152">C#</span><span class="sxs-lookup"><span data-stu-id="a4eb7-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4eb7-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4eb7-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4eb7-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4eb7-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a4eb7-155">响应</span><span class="sxs-lookup"><span data-stu-id="a4eb7-155">Response</span></span>

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
