---
title: 删除 oAuth2PermissionGrant
description: 删除代表委派权限授予的 oAuth2PermissionGrant。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: c73349396b1e2d65130653e56d49550be3bf969b
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44384020"
---
# <a name="delete-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="9e71a-103">删除委派权限授予（oAuth2PermissionGrant）</span><span class="sxs-lookup"><span data-stu-id="9e71a-103">Delete a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="9e71a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e71a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e71a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e71a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e71a-106">删除[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)。</span><span class="sxs-lookup"><span data-stu-id="9e71a-106">Delete an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="9e71a-107">删除委派权限授予时，其授予的访问权限将被吊销。</span><span class="sxs-lookup"><span data-stu-id="9e71a-107">When a delegated permission grant is deleted, the access it granted is revoked.</span></span> <span data-ttu-id="9e71a-108">现有的访问令牌将在其生命周期内继续有效，但不会为删除的**oAuth2PermissionGrant**中标识的委派权限授予新的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="9e71a-108">Existing access tokens will continue to be valid for their lifetime, but new access tokens will not be granted for the delegated permissions identified in the deleted **oAuth2PermissionGrant**.</span></span>

> [!NOTE]
> <span data-ttu-id="9e71a-109">在调用 API 时，可能有两个委派权限授权应用程序代表用户执行操作。</span><span class="sxs-lookup"><span data-stu-id="9e71a-109">There may be two delegated permission grants authorizing an application to act on behalf of a user when calling an API.</span></span> <span data-ttu-id="9e71a-110">当用户代表自己对应用程序同意时（创建具有**consentType** *主体*的**oAuth2PermissionGrant** ，标识用户），然后管理员授予代表所有用户的租户范围*内的管理员*同意（使用 consentType 的**AllPrincipals**创建第二个**oAuth2PermissionGrant** ）时，可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="9e71a-110">This can happen when a user consents for the application on their own behalf (creating an **oAuth2PermissionGrant** with **consentType** *Principal*, identifying the user) and then an administrator grants tenant-wide admin consent on behalf of all users (creating a second **oAuth2PermissionGrant** with **consentType** of *AllPrincipals*).</span></span>

## <a name="permissions"></a><span data-ttu-id="9e71a-111">权限</span><span class="sxs-lookup"><span data-stu-id="9e71a-111">Permissions</span></span>

<span data-ttu-id="9e71a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e71a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e71a-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e71a-114">Permission type</span></span>      | <span data-ttu-id="9e71a-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e71a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e71a-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e71a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9e71a-117">DelegatedPermissionGrant、Directory.accessasuser.all、all 和的所有子目录</span><span class="sxs-lookup"><span data-stu-id="9e71a-117">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e71a-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e71a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e71a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e71a-119">Not supported.</span></span>    |
|<span data-ttu-id="9e71a-120">Application</span><span class="sxs-lookup"><span data-stu-id="9e71a-120">Application</span></span> | <span data-ttu-id="9e71a-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e71a-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e71a-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e71a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9e71a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e71a-123">Request headers</span></span>

| <span data-ttu-id="9e71a-124">名称</span><span class="sxs-lookup"><span data-stu-id="9e71a-124">Name</span></span>       | <span data-ttu-id="9e71a-125">类型</span><span class="sxs-lookup"><span data-stu-id="9e71a-125">Type</span></span> | <span data-ttu-id="9e71a-126">说明</span><span class="sxs-lookup"><span data-stu-id="9e71a-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9e71a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e71a-127">Authorization</span></span>  | <span data-ttu-id="9e71a-128">string</span><span class="sxs-lookup"><span data-stu-id="9e71a-128">string</span></span>  | <span data-ttu-id="9e71a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9e71a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e71a-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e71a-131">Request body</span></span>

<span data-ttu-id="9e71a-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e71a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e71a-133">响应</span><span class="sxs-lookup"><span data-stu-id="9e71a-133">Response</span></span>

<span data-ttu-id="9e71a-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9e71a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e71a-136">示例</span><span class="sxs-lookup"><span data-stu-id="9e71a-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e71a-137">请求</span><span class="sxs-lookup"><span data-stu-id="9e71a-137">Request</span></span>

<span data-ttu-id="9e71a-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e71a-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e71a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e71a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2PermissionGrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="9e71a-140">C#</span><span class="sxs-lookup"><span data-stu-id="9e71a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e71a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e71a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e71a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e71a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9e71a-143">响应</span><span class="sxs-lookup"><span data-stu-id="9e71a-143">Response</span></span>

<span data-ttu-id="9e71a-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9e71a-144">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
