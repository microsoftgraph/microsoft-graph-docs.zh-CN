---
title: 删除 personInterest
description: 从用户的配置文件中删除 personInterest 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4143d9ab789052dc92502a12a45aa37977756339
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036182"
---
# <a name="delete-personinterest"></a><span data-ttu-id="10234-103">删除 personInterest</span><span class="sxs-lookup"><span data-stu-id="10234-103">Delete personInterest</span></span>

<span data-ttu-id="10234-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10234-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10234-105">从用户的[配置文件](../resources/profile.md)中删除[personInterest](../resources/personinterest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10234-105">Deletes a [personInterest](../resources/personinterest.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10234-106">权限</span><span class="sxs-lookup"><span data-stu-id="10234-106">Permissions</span></span>

<span data-ttu-id="10234-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10234-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="10234-109">Permission type</span></span>                        | <span data-ttu-id="10234-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10234-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10234-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10234-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10234-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="10234-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="10234-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10234-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10234-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="10234-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="10234-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="10234-115">Application</span></span>                            | <span data-ttu-id="10234-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10234-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="10234-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10234-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/interests/{id}
DELETE /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="10234-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="10234-118">Request headers</span></span>

| <span data-ttu-id="10234-119">名称</span><span class="sxs-lookup"><span data-stu-id="10234-119">Name</span></span>           |<span data-ttu-id="10234-120">说明</span><span class="sxs-lookup"><span data-stu-id="10234-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="10234-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="10234-121">Authorization</span></span>  | <span data-ttu-id="10234-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10234-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="10234-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="10234-124">Request body</span></span>

<span data-ttu-id="10234-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10234-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10234-126">响应</span><span class="sxs-lookup"><span data-stu-id="10234-126">Response</span></span>

<span data-ttu-id="10234-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="10234-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10234-129">示例</span><span class="sxs-lookup"><span data-stu-id="10234-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10234-130">请求</span><span class="sxs-lookup"><span data-stu-id="10234-130">Request</span></span>

<span data-ttu-id="10234-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="10234-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10234-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="10234-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personinterest"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/interests/{id}
```
# <a name="c"></a>[<span data-ttu-id="10234-133">C#</span><span class="sxs-lookup"><span data-stu-id="10234-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10234-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10234-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10234-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10234-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10234-136">响应</span><span class="sxs-lookup"><span data-stu-id="10234-136">Response</span></span>

<span data-ttu-id="10234-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="10234-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


