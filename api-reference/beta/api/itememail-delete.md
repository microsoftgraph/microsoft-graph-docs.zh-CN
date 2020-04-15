---
title: 删除 itemEmail
description: 从用户配置文件中删除 itemEmail 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 60f14889f40faedf0e6c8e75a4ff20382db7554c
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510887"
---
# <a name="delete-itememail"></a><span data-ttu-id="39d01-103">删除 itemEmail</span><span class="sxs-lookup"><span data-stu-id="39d01-103">Delete itemEmail</span></span>

<span data-ttu-id="39d01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39d01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39d01-105">从用户的[配置文件](../resources/profile.md)中删除[itemEmail](../resources/itememail.md)对象。</span><span class="sxs-lookup"><span data-stu-id="39d01-105">Delete an [itemEmail](../resources/itememail.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="39d01-106">权限</span><span class="sxs-lookup"><span data-stu-id="39d01-106">Permissions</span></span>

<span data-ttu-id="39d01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39d01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39d01-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="39d01-109">Permission type</span></span>                        | <span data-ttu-id="39d01-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39d01-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39d01-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39d01-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39d01-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="39d01-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="39d01-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39d01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39d01-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="39d01-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="39d01-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="39d01-115">Application</span></span>                            | <span data-ttu-id="39d01-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d01-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="39d01-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39d01-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/emails/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="39d01-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="39d01-118">Request headers</span></span>

| <span data-ttu-id="39d01-119">名称</span><span class="sxs-lookup"><span data-stu-id="39d01-119">Name</span></span>           |<span data-ttu-id="39d01-120">说明</span><span class="sxs-lookup"><span data-stu-id="39d01-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="39d01-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="39d01-121">Authorization</span></span>  | <span data-ttu-id="39d01-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39d01-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="39d01-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="39d01-124">Request body</span></span>

<span data-ttu-id="39d01-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39d01-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39d01-126">响应</span><span class="sxs-lookup"><span data-stu-id="39d01-126">Response</span></span>

<span data-ttu-id="39d01-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="39d01-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39d01-129">示例</span><span class="sxs-lookup"><span data-stu-id="39d01-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39d01-130">请求</span><span class="sxs-lookup"><span data-stu-id="39d01-130">Request</span></span>

<span data-ttu-id="39d01-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="39d01-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39d01-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="39d01-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itememail"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/emails/{id}
```

# <a name="c"></a>[<span data-ttu-id="39d01-133">C#</span><span class="sxs-lookup"><span data-stu-id="39d01-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itememail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39d01-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39d01-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itememail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39d01-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39d01-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itememail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="39d01-136">响应</span><span class="sxs-lookup"><span data-stu-id="39d01-136">Response</span></span>

<span data-ttu-id="39d01-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="39d01-137">The following is an example of the response.</span></span>

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
  "description": "Delete itemEmail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
