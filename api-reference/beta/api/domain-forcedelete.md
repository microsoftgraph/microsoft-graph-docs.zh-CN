---
title: 域： forceDelete
description: 删除使用异步操作的域。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6c3d942352a0db20d6e46a4b00686ad948bd6798
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965122"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="eadd9-103">域： forceDelete</span><span class="sxs-lookup"><span data-stu-id="eadd9-103">domain: forceDelete</span></span>

> <span data-ttu-id="eadd9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eadd9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eadd9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eadd9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eadd9-106">删除使用异步操作的域。</span><span class="sxs-lookup"><span data-stu-id="eadd9-106">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="eadd9-107">此操作的一部分执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="eadd9-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="eadd9-108">重命名的 UPN、 EmailAddress 和 ProxyAddress 具有引用的已删除的域的用户。</span><span class="sxs-lookup"><span data-stu-id="eadd9-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="eadd9-109">重命名与引用的已删除的域的组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="eadd9-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="eadd9-110">重命名应用程序与已删除的域引用的 identifierUris。</span><span class="sxs-lookup"><span data-stu-id="eadd9-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="eadd9-111">如果要重命名的对象的数量大于 1000年，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="eadd9-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="eadd9-112">如果要重命名的应用程序之一是多租户应用程序，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="eadd9-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="eadd9-113">域删除完成后，已删除的域的 API 操作将返回 404 的 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eadd9-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="eadd9-114">若要验证删除的域，您可以执行[获取域](domain-get.md)。</span><span class="sxs-lookup"><span data-stu-id="eadd9-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="eadd9-115">如果已成功删除域，将在响应中返回 404 的 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eadd9-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="eadd9-116">权限</span><span class="sxs-lookup"><span data-stu-id="eadd9-116">Permissions</span></span>

<span data-ttu-id="eadd9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eadd9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eadd9-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="eadd9-119">Permission type</span></span>      | <span data-ttu-id="eadd9-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eadd9-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eadd9-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eadd9-121">Delegated (work or school account)</span></span> | <span data-ttu-id="eadd9-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eadd9-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eadd9-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eadd9-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eadd9-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="eadd9-124">Not supported.</span></span>    |
|<span data-ttu-id="eadd9-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="eadd9-125">Application</span></span> | <span data-ttu-id="eadd9-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eadd9-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eadd9-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eadd9-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="eadd9-128">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="eadd9-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eadd9-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="eadd9-129">Request headers</span></span>

| <span data-ttu-id="eadd9-130">名称</span><span class="sxs-lookup"><span data-stu-id="eadd9-130">Name</span></span>       | <span data-ttu-id="eadd9-131">说明</span><span class="sxs-lookup"><span data-stu-id="eadd9-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eadd9-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="eadd9-132">Authorization</span></span>  | <span data-ttu-id="eadd9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eadd9-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="eadd9-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eadd9-135">Content-Type</span></span>  | <span data-ttu-id="eadd9-136">application/json</span><span class="sxs-lookup"><span data-stu-id="eadd9-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="eadd9-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="eadd9-137">Request body</span></span>

<span data-ttu-id="eadd9-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="eadd9-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eadd9-139">参数</span><span class="sxs-lookup"><span data-stu-id="eadd9-139">Parameter</span></span>    | <span data-ttu-id="eadd9-140">类型</span><span class="sxs-lookup"><span data-stu-id="eadd9-140">Type</span></span>   |<span data-ttu-id="eadd9-141">说明</span><span class="sxs-lookup"><span data-stu-id="eadd9-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eadd9-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="eadd9-142">disableUserAccounts</span></span>|<span data-ttu-id="eadd9-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="eadd9-143">Boolean</span></span>| <span data-ttu-id="eadd9-144">若要禁用重命名的用户帐户的选项。</span><span class="sxs-lookup"><span data-stu-id="eadd9-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="eadd9-145">如果禁用的用户帐户，则用户将不允许登录。</span><span class="sxs-lookup"><span data-stu-id="eadd9-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="eadd9-146">*True*（默认值）-重命名此操作的一部分的帐户被禁用的用户。</span><span class="sxs-lookup"><span data-stu-id="eadd9-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="eadd9-147">未禁用*false* -重命名此操作的一部分的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="eadd9-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="eadd9-148">响应</span><span class="sxs-lookup"><span data-stu-id="eadd9-148">Response</span></span>

<span data-ttu-id="eadd9-149">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eadd9-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="eadd9-150">示例</span><span class="sxs-lookup"><span data-stu-id="eadd9-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eadd9-151">请求</span><span class="sxs-lookup"><span data-stu-id="eadd9-151">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="eadd9-152">响应</span><span class="sxs-lookup"><span data-stu-id="eadd9-152">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
