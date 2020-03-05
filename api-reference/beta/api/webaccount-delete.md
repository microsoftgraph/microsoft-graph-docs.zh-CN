---
title: 删除 webAccount
description: 从用户的配置文件中删除 webAccount 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4c7674e656fa01fb858a0184c667720e99048dd6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451532"
---
# <a name="delete-webaccount"></a><span data-ttu-id="3dcae-103">删除 webAccount</span><span class="sxs-lookup"><span data-stu-id="3dcae-103">Delete webAccount</span></span>

<span data-ttu-id="3dcae-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3dcae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dcae-105">从用户的配置文件中删除[webAccount](../resources/webaccount.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3dcae-105">Delete a [webAccount](../resources/webaccount.md) object from the user's profile.</span></span>

## <a name="permissions"></a><span data-ttu-id="3dcae-106">权限</span><span class="sxs-lookup"><span data-stu-id="3dcae-106">Permissions</span></span>

<span data-ttu-id="3dcae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dcae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3dcae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dcae-109">Permission type</span></span>                        | <span data-ttu-id="3dcae-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3dcae-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3dcae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dcae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3dcae-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="3dcae-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3dcae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dcae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dcae-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="3dcae-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3dcae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dcae-115">Application</span></span>                            | <span data-ttu-id="3dcae-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dcae-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3dcae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dcae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3dcae-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dcae-118">Request headers</span></span>

| <span data-ttu-id="3dcae-119">名称</span><span class="sxs-lookup"><span data-stu-id="3dcae-119">Name</span></span>           |<span data-ttu-id="3dcae-120">说明</span><span class="sxs-lookup"><span data-stu-id="3dcae-120">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="3dcae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dcae-121">Authorization</span></span>  | <span data-ttu-id="3dcae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3dcae-p102">Bearer {token}. Required.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="3dcae-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dcae-124">Request body</span></span>

<span data-ttu-id="3dcae-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3dcae-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dcae-126">响应</span><span class="sxs-lookup"><span data-stu-id="3dcae-126">Response</span></span>

<span data-ttu-id="3dcae-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3dcae-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3dcae-129">示例</span><span class="sxs-lookup"><span data-stu-id="3dcae-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3dcae-130">请求</span><span class="sxs-lookup"><span data-stu-id="3dcae-130">Request</span></span>

<span data-ttu-id="3dcae-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3dcae-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3dcae-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dcae-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_webaccount"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
```
# <a name="c"></a>[<span data-ttu-id="3dcae-133">C#</span><span class="sxs-lookup"><span data-stu-id="3dcae-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dcae-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dcae-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dcae-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dcae-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3dcae-136">响应</span><span class="sxs-lookup"><span data-stu-id="3dcae-136">Response</span></span>

<span data-ttu-id="3dcae-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3dcae-137">The following is an example of the response.</span></span>

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
  "description": "Delete webAccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
