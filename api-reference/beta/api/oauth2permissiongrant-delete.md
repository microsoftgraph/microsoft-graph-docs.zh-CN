---
title: 删除 oAuth2PermissionGrant
description: 删除表示委派权限授予的 oAuth2PermissionGrant。
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: b026f2e254a0901526baddaf786ab8d1d6efab6d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447940"
---
# <a name="delete-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="b4cb4-103">删除 oAuth2PermissionGrant (委派) </span><span class="sxs-lookup"><span data-stu-id="b4cb4-103">Delete a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="b4cb4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4cb4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4cb4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4cb4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4cb4-106">删除 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-106">Delete an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="b4cb4-107">删除委派权限授予后，将撤消授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-107">When a delegated permission grant is deleted, the access it granted is revoked.</span></span> <span data-ttu-id="b4cb4-108">现有访问令牌在生存期内将继续有效，但不会为已删除 **的 oAuth2PermissionGrant** 中标识的委派权限授予新的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-108">Existing access tokens will continue to be valid for their lifetime, but new access tokens will not be granted for the delegated permissions identified in the deleted **oAuth2PermissionGrant**.</span></span>

> [!NOTE]
> <span data-ttu-id="b4cb4-109">可能有两个委派权限授予，授权应用程序在调用 API 时代表用户操作。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-109">There may be two delegated permission grants authorizing an application to act on behalf of a user when calling an API.</span></span> <span data-ttu-id="b4cb4-110">如果用户代表自己同意应用程序 (创建具有 **consentType** 主体的 **oAuth2PermissionGrant，** 标识用户) ，然后管理员代表所有用户授予租户范围的管理员同意， (创建具有 *AllPrincipals*) **consentType** 的第二个 **oAuth2PermissionGrant** 时，可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-110">This can happen when a user consents for the application on their own behalf (creating an **oAuth2PermissionGrant** with **consentType** *Principal*, identifying the user) and then an administrator grants tenant-wide admin consent on behalf of all users (creating a second **oAuth2PermissionGrant** with **consentType** of *AllPrincipals*).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4cb4-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="b4cb4-111">Permissions</span></span>

<span data-ttu-id="b4cb4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4cb4-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4cb4-114">Permission type</span></span>      | <span data-ttu-id="b4cb4-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4cb4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4cb4-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4cb4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b4cb4-117">DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4cb4-117">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4cb4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4cb4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4cb4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-119">Not supported.</span></span>    |
|<span data-ttu-id="b4cb4-120">Application</span><span class="sxs-lookup"><span data-stu-id="b4cb4-120">Application</span></span> | <span data-ttu-id="b4cb4-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4cb4-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4cb4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4cb4-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4cb4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4cb4-123">Request headers</span></span>

| <span data-ttu-id="b4cb4-124">名称</span><span class="sxs-lookup"><span data-stu-id="b4cb4-124">Name</span></span>       | <span data-ttu-id="b4cb4-125">类型</span><span class="sxs-lookup"><span data-stu-id="b4cb4-125">Type</span></span> | <span data-ttu-id="b4cb4-126">说明</span><span class="sxs-lookup"><span data-stu-id="b4cb4-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b4cb4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4cb4-127">Authorization</span></span>  | <span data-ttu-id="b4cb4-128">string</span><span class="sxs-lookup"><span data-stu-id="b4cb4-128">string</span></span>  | <span data-ttu-id="b4cb4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4cb4-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4cb4-131">Request body</span></span>

<span data-ttu-id="b4cb4-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4cb4-133">响应</span><span class="sxs-lookup"><span data-stu-id="b4cb4-133">Response</span></span>

<span data-ttu-id="b4cb4-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4cb4-136">示例</span><span class="sxs-lookup"><span data-stu-id="b4cb4-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4cb4-137">请求</span><span class="sxs-lookup"><span data-stu-id="b4cb4-137">Request</span></span>

<span data-ttu-id="b4cb4-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b4cb4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4cb4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2PermissionGrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
```

# <a name="c"></a>[<span data-ttu-id="b4cb4-140">C#</span><span class="sxs-lookup"><span data-stu-id="b4cb4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4cb4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4cb4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4cb4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4cb4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4cb4-143">Java</span><span class="sxs-lookup"><span data-stu-id="b4cb4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b4cb4-144">响应</span><span class="sxs-lookup"><span data-stu-id="b4cb4-144">Response</span></span>

<span data-ttu-id="b4cb4-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4cb4-145">Here is an example of the response.</span></span>

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


