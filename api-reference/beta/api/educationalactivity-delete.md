---
title: 删除 educationalActivity
description: 从用户配置文件中删除 educationalActivity 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ad9cc4f842e9d4cf4402d70d515a109279b1f92d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966676"
---
# <a name="delete-educationalactivity"></a><span data-ttu-id="e6ae2-103">删除 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="e6ae2-103">Delete educationalActivity</span></span>

<span data-ttu-id="e6ae2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6ae2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6ae2-105">从用户的[配置文件](../resources/profile.md)中删除[educationalActivity](../resources/educationalactivity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e6ae2-105">Delete an [educationalActivity](../resources/educationalactivity.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6ae2-106">权限</span><span class="sxs-lookup"><span data-stu-id="e6ae2-106">Permissions</span></span>

<span data-ttu-id="e6ae2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6ae2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6ae2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6ae2-109">Permission type</span></span>                        | <span data-ttu-id="e6ae2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6ae2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e6ae2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6ae2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6ae2-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="e6ae2-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e6ae2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6ae2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6ae2-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="e6ae2-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e6ae2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6ae2-115">Application</span></span>                            | <span data-ttu-id="e6ae2-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ae2-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e6ae2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6ae2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/educationalActivities/{id} 
DELETE /users/{id | userPrincipalName}/profile/educationalActivities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e6ae2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6ae2-118">Request headers</span></span>

| <span data-ttu-id="e6ae2-119">名称</span><span class="sxs-lookup"><span data-stu-id="e6ae2-119">Name</span></span>           |<span data-ttu-id="e6ae2-120">说明</span><span class="sxs-lookup"><span data-stu-id="e6ae2-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e6ae2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6ae2-121">Authorization</span></span>  | <span data-ttu-id="e6ae2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6ae2-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="e6ae2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6ae2-124">Request body</span></span>

<span data-ttu-id="e6ae2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e6ae2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6ae2-126">响应</span><span class="sxs-lookup"><span data-stu-id="e6ae2-126">Response</span></span>

<span data-ttu-id="e6ae2-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e6ae2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6ae2-129">示例</span><span class="sxs-lookup"><span data-stu-id="e6ae2-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e6ae2-130">请求</span><span class="sxs-lookup"><span data-stu-id="e6ae2-130">Request</span></span>

<span data-ttu-id="e6ae2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e6ae2-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e6ae2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6ae2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationalactivity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
```
# <a name="c"></a>[<span data-ttu-id="e6ae2-133">C#</span><span class="sxs-lookup"><span data-stu-id="e6ae2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6ae2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6ae2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6ae2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6ae2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6ae2-136">Java</span><span class="sxs-lookup"><span data-stu-id="e6ae2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationalactivity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e6ae2-137">响应</span><span class="sxs-lookup"><span data-stu-id="e6ae2-137">Response</span></span>

<span data-ttu-id="e6ae2-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e6ae2-138">The following is an example of the response.</span></span>

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
  "description": "Delete educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


