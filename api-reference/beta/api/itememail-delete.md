---
title: 删除 itemEmail
description: 从用户配置文件中删除 itemEmail 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 51978f3f57be0244f5320688466ac21dcd94dd0b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997379"
---
# <a name="delete-itememail"></a><span data-ttu-id="de480-103">删除 itemEmail</span><span class="sxs-lookup"><span data-stu-id="de480-103">Delete itemEmail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de480-104">从用户的[配置文件](../resources/profile.md)中删除[itemEmail](../resources/itememail.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de480-104">Delete an [itemEmail](../resources/itememail.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="de480-105">权限</span><span class="sxs-lookup"><span data-stu-id="de480-105">Permissions</span></span>

<span data-ttu-id="de480-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de480-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de480-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="de480-108">Permission type</span></span>                        | <span data-ttu-id="de480-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de480-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de480-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de480-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="de480-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="de480-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="de480-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de480-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de480-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="de480-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="de480-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="de480-114">Application</span></span>                            | <span data-ttu-id="de480-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de480-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="de480-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de480-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/emails/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="de480-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="de480-117">Request headers</span></span>

| <span data-ttu-id="de480-118">名称</span><span class="sxs-lookup"><span data-stu-id="de480-118">Name</span></span>           |<span data-ttu-id="de480-119">说明</span><span class="sxs-lookup"><span data-stu-id="de480-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="de480-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de480-120">Authorization</span></span>  | <span data-ttu-id="de480-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de480-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="de480-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="de480-123">Request body</span></span>

<span data-ttu-id="de480-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="de480-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de480-125">响应</span><span class="sxs-lookup"><span data-stu-id="de480-125">Response</span></span>

<span data-ttu-id="de480-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="de480-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de480-128">示例</span><span class="sxs-lookup"><span data-stu-id="de480-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de480-129">请求</span><span class="sxs-lookup"><span data-stu-id="de480-129">Request</span></span>

<span data-ttu-id="de480-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="de480-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="de480-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="de480-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itememail"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/emails/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de480-132">C#</span><span class="sxs-lookup"><span data-stu-id="de480-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itememail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de480-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de480-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itememail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de480-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de480-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itememail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de480-135">响应</span><span class="sxs-lookup"><span data-stu-id="de480-135">Response</span></span>

<span data-ttu-id="de480-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="de480-136">The following is an example of the response.</span></span>

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
