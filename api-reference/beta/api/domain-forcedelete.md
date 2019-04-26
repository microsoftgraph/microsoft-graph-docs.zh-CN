---
title: '域: forceDelete'
description: 使用异步操作删除域。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c58b7d345ba7c5cdc7c029ecf929676fc7529f12
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325875"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="6e358-103">域: forceDelete</span><span class="sxs-lookup"><span data-stu-id="6e358-103">domain: forceDelete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e358-104">使用异步操作删除域。</span><span class="sxs-lookup"><span data-stu-id="6e358-104">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="6e358-105">在此操作过程中, 将执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="6e358-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="6e358-106">使用对已删除域的引用重命名用户的 UPN、EmailAddress 和 ProxyAddress。</span><span class="sxs-lookup"><span data-stu-id="6e358-106">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="6e358-107">使用对已删除域的引用重命名组的 EmailAddress。</span><span class="sxs-lookup"><span data-stu-id="6e358-107">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="6e358-108">将应用程序的 identifierUris 重命名为对已删除的域的引用。</span><span class="sxs-lookup"><span data-stu-id="6e358-108">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="6e358-109">如果要重命名的对象的数量大于 1000, 则返回错误。</span><span class="sxs-lookup"><span data-stu-id="6e358-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="6e358-110">如果要重命名的某个应用程序是多租户应用程序, 则会返回错误。</span><span class="sxs-lookup"><span data-stu-id="6e358-110">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="6e358-111">域删除完成后, 已删除域的 API 操作将返回 404 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6e358-111">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="6e358-112">若要验证域的删除, 可以执行[获取域](domain-get.md)。</span><span class="sxs-lookup"><span data-stu-id="6e358-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="6e358-113">如果已成功删除域, 响应中将返回 404 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6e358-113">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e358-114">权限</span><span class="sxs-lookup"><span data-stu-id="6e358-114">Permissions</span></span>

<span data-ttu-id="6e358-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e358-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6e358-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e358-117">Permission type</span></span>      | <span data-ttu-id="6e358-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e358-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e358-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e358-119">Delegated (work or school account)</span></span> | <span data-ttu-id="6e358-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e358-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6e358-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e358-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e358-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e358-122">Not supported.</span></span>    |
|<span data-ttu-id="6e358-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e358-123">Application</span></span> | <span data-ttu-id="6e358-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e358-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e358-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e358-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="6e358-126">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="6e358-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e358-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e358-127">Request headers</span></span>

| <span data-ttu-id="6e358-128">名称</span><span class="sxs-lookup"><span data-stu-id="6e358-128">Name</span></span>       | <span data-ttu-id="6e358-129">说明</span><span class="sxs-lookup"><span data-stu-id="6e358-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6e358-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e358-130">Authorization</span></span>  | <span data-ttu-id="6e358-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e358-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="6e358-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e358-133">Content-Type</span></span>  | <span data-ttu-id="6e358-134">application/json</span><span class="sxs-lookup"><span data-stu-id="6e358-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e358-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e358-135">Request body</span></span>

<span data-ttu-id="6e358-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6e358-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6e358-137">参数</span><span class="sxs-lookup"><span data-stu-id="6e358-137">Parameter</span></span>    | <span data-ttu-id="6e358-138">类型</span><span class="sxs-lookup"><span data-stu-id="6e358-138">Type</span></span>   |<span data-ttu-id="6e358-139">说明</span><span class="sxs-lookup"><span data-stu-id="6e358-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e358-140">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="6e358-140">disableUserAccounts</span></span>|<span data-ttu-id="6e358-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e358-141">Boolean</span></span>| <span data-ttu-id="6e358-142">用于禁用重命名的用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="6e358-142">Option to disable renamed user accounts.</span></span> <span data-ttu-id="6e358-143">如果用户帐户已禁用, 则不允许用户登录。</span><span class="sxs-lookup"><span data-stu-id="6e358-143">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="6e358-144">*True*(默认值)-已禁用作为此操作的一部分重命名的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="6e358-144">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="6e358-145">*False* -不禁用作为此操作的一部分重命名的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="6e358-145">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="6e358-146">响应</span><span class="sxs-lookup"><span data-stu-id="6e358-146">Response</span></span>

<span data-ttu-id="6e358-147">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6e358-147">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="6e358-148">示例</span><span class="sxs-lookup"><span data-stu-id="6e358-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e358-149">请求</span><span class="sxs-lookup"><span data-stu-id="6e358-149">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="6e358-150">响应</span><span class="sxs-lookup"><span data-stu-id="6e358-150">Response</span></span>

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
  "suppressions": []
}
-->
