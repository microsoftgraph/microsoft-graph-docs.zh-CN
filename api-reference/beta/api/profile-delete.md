---
title: 删除配置文件
description: 删除配置文件。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5acbffb4f272b5c5c8b760dd7a032608189d78ad
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998044"
---
# <a name="delete-profile"></a><span data-ttu-id="855e9-103">删除配置文件</span><span class="sxs-lookup"><span data-stu-id="855e9-103">Delete profile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="855e9-104">从用户帐户中删除[配置文件](../resources/profile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="855e9-104">Delete [profile](../resources/profile.md) object from a user's account.</span></span>

## <a name="permissions"></a><span data-ttu-id="855e9-105">权限</span><span class="sxs-lookup"><span data-stu-id="855e9-105">Permissions</span></span>

<span data-ttu-id="855e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="855e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="855e9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="855e9-108">Permission type</span></span>                        | <span data-ttu-id="855e9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="855e9-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="855e9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="855e9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="855e9-111">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="855e9-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="855e9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="855e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="855e9-113">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="855e9-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="855e9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="855e9-114">Application</span></span>                            | <span data-ttu-id="855e9-115">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="855e9-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="855e9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="855e9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile
```

## <a name="request-headers"></a><span data-ttu-id="855e9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="855e9-117">Request headers</span></span>

| <span data-ttu-id="855e9-118">名称</span><span class="sxs-lookup"><span data-stu-id="855e9-118">Name</span></span>           |<span data-ttu-id="855e9-119">说明</span><span class="sxs-lookup"><span data-stu-id="855e9-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="855e9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="855e9-120">Authorization</span></span>  | <span data-ttu-id="855e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="855e9-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="855e9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="855e9-123">Content-Type</span></span>   | <span data-ttu-id="855e9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="855e9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="855e9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="855e9-126">Request body</span></span>

<span data-ttu-id="855e9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="855e9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="855e9-128">响应</span><span class="sxs-lookup"><span data-stu-id="855e9-128">Response</span></span>

<span data-ttu-id="855e9-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="855e9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="855e9-131">示例</span><span class="sxs-lookup"><span data-stu-id="855e9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="855e9-132">请求</span><span class="sxs-lookup"><span data-stu-id="855e9-132">Request</span></span>

<span data-ttu-id="855e9-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="855e9-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="855e9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="855e9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_profile"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="855e9-135">C#</span><span class="sxs-lookup"><span data-stu-id="855e9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="855e9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="855e9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="855e9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="855e9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="855e9-138">响应</span><span class="sxs-lookup"><span data-stu-id="855e9-138">Response</span></span>

<span data-ttu-id="855e9-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="855e9-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete profile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
