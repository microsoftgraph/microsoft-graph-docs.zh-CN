---
title: 删除 userAccountInformation
description: 删除 userAccountInformation 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9f922b7ed4f55b6f7a4ad4b80b6b0c9bb2125052
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433501"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="6375d-103">删除 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="6375d-103">Delete userAccountInformation</span></span>

<span data-ttu-id="6375d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6375d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6375d-105">从 [用户配置文件中删除 userAccountInformation](../resources/useraccountinformation.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="6375d-105">Delete an [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6375d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6375d-106">Permissions</span></span>

<span data-ttu-id="6375d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6375d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6375d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6375d-109">Permission type</span></span>                        | <span data-ttu-id="6375d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6375d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6375d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6375d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6375d-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6375d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6375d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6375d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6375d-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6375d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6375d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6375d-115">Application</span></span>                            | <span data-ttu-id="6375d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6375d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="6375d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6375d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/account/{id}
DELETE /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6375d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6375d-118">Request headers</span></span>

| <span data-ttu-id="6375d-119">名称</span><span class="sxs-lookup"><span data-stu-id="6375d-119">Name</span></span>           | <span data-ttu-id="6375d-120">说明</span><span class="sxs-lookup"><span data-stu-id="6375d-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6375d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6375d-121">Authorization</span></span>  | <span data-ttu-id="6375d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6375d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6375d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6375d-124">Request body</span></span>

<span data-ttu-id="6375d-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6375d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6375d-126">响应</span><span class="sxs-lookup"><span data-stu-id="6375d-126">Response</span></span>

<span data-ttu-id="6375d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6375d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6375d-129">示例</span><span class="sxs-lookup"><span data-stu-id="6375d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6375d-130">请求</span><span class="sxs-lookup"><span data-stu-id="6375d-130">Request</span></span>

<span data-ttu-id="6375d-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6375d-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6375d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6375d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/account/{id}
```
# <a name="c"></a>[<span data-ttu-id="6375d-133">C#</span><span class="sxs-lookup"><span data-stu-id="6375d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6375d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6375d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6375d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6375d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6375d-136">Java</span><span class="sxs-lookup"><span data-stu-id="6375d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-useraccountinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6375d-137">响应</span><span class="sxs-lookup"><span data-stu-id="6375d-137">Response</span></span>

<span data-ttu-id="6375d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6375d-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

