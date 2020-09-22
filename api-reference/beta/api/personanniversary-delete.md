---
title: 删除 personAnniversary
description: 从用户的配置文件中删除 personAnniversary 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8d1cc615539c986fc9641f1fff4d0f9f9f38e3c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040299"
---
# <a name="delete-personanniversary"></a><span data-ttu-id="e3036-103">删除 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="e3036-103">Delete personAnniversary</span></span>

<span data-ttu-id="e3036-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3036-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3036-105">从用户的[配置文件](../resources/profile.md)中删除[personAnniversary](../resources/personanniversary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e3036-105">Delete a [personAnniversary](../resources/personanniversary.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3036-106">权限</span><span class="sxs-lookup"><span data-stu-id="e3036-106">Permissions</span></span>

<span data-ttu-id="e3036-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3036-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3036-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3036-109">Permission type</span></span>                        | <span data-ttu-id="e3036-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3036-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3036-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3036-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3036-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="e3036-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e3036-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3036-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3036-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="e3036-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e3036-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3036-115">Application</span></span>                            | <span data-ttu-id="e3036-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3036-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e3036-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3036-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/anniversaries/{id}
DELETE /users/{id | userPrincipalName}/profile/anniversaries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e3036-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3036-118">Request headers</span></span>

| <span data-ttu-id="e3036-119">名称</span><span class="sxs-lookup"><span data-stu-id="e3036-119">Name</span></span>           |<span data-ttu-id="e3036-120">说明</span><span class="sxs-lookup"><span data-stu-id="e3036-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e3036-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3036-121">Authorization</span></span>  | <span data-ttu-id="e3036-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3036-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="e3036-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3036-124">Request body</span></span>

<span data-ttu-id="e3036-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3036-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3036-126">响应</span><span class="sxs-lookup"><span data-stu-id="e3036-126">Response</span></span>

<span data-ttu-id="e3036-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e3036-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3036-129">示例</span><span class="sxs-lookup"><span data-stu-id="e3036-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3036-130">请求</span><span class="sxs-lookup"><span data-stu-id="e3036-130">Request</span></span>

<span data-ttu-id="e3036-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e3036-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3036-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3036-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personanniversary"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
```
# <a name="c"></a>[<span data-ttu-id="e3036-133">C#</span><span class="sxs-lookup"><span data-stu-id="e3036-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3036-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3036-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3036-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3036-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e3036-136">响应</span><span class="sxs-lookup"><span data-stu-id="e3036-136">Response</span></span>

<span data-ttu-id="e3036-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e3036-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


