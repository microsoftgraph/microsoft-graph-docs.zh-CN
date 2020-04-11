---
title: 删除 languageProficiency
description: 从用户的配置文件中删除 languageProficiency 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8c33c10a3dd4674c59816b18b84b1bce9d84bf26
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228936"
---
# <a name="delete-languageproficiency"></a><span data-ttu-id="39a93-103">删除 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="39a93-103">Delete languageProficiency</span></span>

<span data-ttu-id="39a93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39a93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39a93-105">从用户的[配置文件](../resources/profile.md)中删除[languageProficiency](../resources/languageproficiency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="39a93-105">Delete a [languageProficiency](../resources/languageproficiency.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="39a93-106">权限</span><span class="sxs-lookup"><span data-stu-id="39a93-106">Permissions</span></span>

<span data-ttu-id="39a93-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39a93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39a93-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="39a93-109">Permission type</span></span>                        | <span data-ttu-id="39a93-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39a93-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39a93-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39a93-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39a93-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="39a93-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="39a93-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39a93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39a93-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="39a93-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="39a93-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="39a93-115">Application</span></span>                            | <span data-ttu-id="39a93-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39a93-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="39a93-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39a93-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="39a93-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="39a93-118">Request headers</span></span>

| <span data-ttu-id="39a93-119">名称</span><span class="sxs-lookup"><span data-stu-id="39a93-119">Name</span></span>           |<span data-ttu-id="39a93-120">说明</span><span class="sxs-lookup"><span data-stu-id="39a93-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="39a93-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="39a93-121">Authorization</span></span>  | <span data-ttu-id="39a93-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39a93-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="39a93-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39a93-124">Content-Type</span></span>   | <span data-ttu-id="39a93-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="39a93-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39a93-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="39a93-127">Request body</span></span>

<span data-ttu-id="39a93-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39a93-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39a93-129">响应</span><span class="sxs-lookup"><span data-stu-id="39a93-129">Response</span></span>

<span data-ttu-id="39a93-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="39a93-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39a93-132">示例</span><span class="sxs-lookup"><span data-stu-id="39a93-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39a93-133">请求</span><span class="sxs-lookup"><span data-stu-id="39a93-133">Request</span></span>

<span data-ttu-id="39a93-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="39a93-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39a93-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="39a93-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_languageproficiency"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/languages/{id}
```
# <a name="c"></a>[<span data-ttu-id="39a93-136">C#</span><span class="sxs-lookup"><span data-stu-id="39a93-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39a93-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39a93-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39a93-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39a93-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="39a93-139">响应</span><span class="sxs-lookup"><span data-stu-id="39a93-139">Response</span></span>

<span data-ttu-id="39a93-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="39a93-140">The following is an example of the response.</span></span>

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
  "description": "Delete languageProficiency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
