---
title: 删除 personWebsite
description: 从用户的配置文件中删除 personWebsite 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 84e53137c64e7b8c54009faae6c5ac9feae9dcd6
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997084"
---
# <a name="delete-personwebsite"></a><span data-ttu-id="fe2b4-103">删除 personWebsite</span><span class="sxs-lookup"><span data-stu-id="fe2b4-103">Delete personWebsite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe2b4-104">从用户的[配置文件](../resources/profile.md)中删除[personWebsite](../resources/personwebsite.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fe2b4-104">Deletes a [personWebsite](../resources/personwebsite.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe2b4-105">权限</span><span class="sxs-lookup"><span data-stu-id="fe2b4-105">Permissions</span></span>

<span data-ttu-id="fe2b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe2b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe2b4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe2b4-108">Permission type</span></span>                        | <span data-ttu-id="fe2b4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe2b4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fe2b4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe2b4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe2b4-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="fe2b4-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fe2b4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe2b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe2b4-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="fe2b4-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="fe2b4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe2b4-114">Application</span></span>                            | <span data-ttu-id="fe2b4-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe2b4-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="fe2b4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe2b4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/websites/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fe2b4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe2b4-117">Request headers</span></span>

| <span data-ttu-id="fe2b4-118">名称</span><span class="sxs-lookup"><span data-stu-id="fe2b4-118">Name</span></span>           |<span data-ttu-id="fe2b4-119">说明</span><span class="sxs-lookup"><span data-stu-id="fe2b4-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="fe2b4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe2b4-120">Authorization</span></span>  | <span data-ttu-id="fe2b4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe2b4-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="fe2b4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe2b4-123">Content-Type</span></span>   | <span data-ttu-id="fe2b4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fe2b4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe2b4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe2b4-126">Request body</span></span>

<span data-ttu-id="fe2b4-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe2b4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe2b4-128">响应</span><span class="sxs-lookup"><span data-stu-id="fe2b4-128">Response</span></span>

<span data-ttu-id="fe2b4-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fe2b4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe2b4-131">示例</span><span class="sxs-lookup"><span data-stu-id="fe2b4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fe2b4-132">请求</span><span class="sxs-lookup"><span data-stu-id="fe2b4-132">Request</span></span>

<span data-ttu-id="fe2b4-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fe2b4-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fe2b4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe2b4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personwebsite"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/websites/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe2b4-135">C#</span><span class="sxs-lookup"><span data-stu-id="fe2b4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personwebsite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe2b4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe2b4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personwebsite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe2b4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe2b4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personwebsite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe2b4-138">响应</span><span class="sxs-lookup"><span data-stu-id="fe2b4-138">Response</span></span>

<span data-ttu-id="fe2b4-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fe2b4-139">The following is an example of the response.</span></span>

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
  "description": "Delete personWebsite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
