---
title: 删除 itemPhone
description: 从用户的配置文件中删除 itemPhone 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: da4866a6b5c5dbe2a8b0d65a04ae4dd7bccbb4a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457244"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="cffcc-103">删除 itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="cffcc-103">Delete itemPhoneNumber</span></span>

<span data-ttu-id="cffcc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cffcc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cffcc-105">从用户的[配置文件](../resources/profile.md)中删除[itemPhone](../resources/itemphone.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cffcc-105">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cffcc-106">权限</span><span class="sxs-lookup"><span data-stu-id="cffcc-106">Permissions</span></span>

<span data-ttu-id="cffcc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cffcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cffcc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cffcc-109">Permission type</span></span>                        | <span data-ttu-id="cffcc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cffcc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cffcc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cffcc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cffcc-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="cffcc-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="cffcc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cffcc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cffcc-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="cffcc-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="cffcc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cffcc-115">Application</span></span>                            | <span data-ttu-id="cffcc-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cffcc-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="cffcc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cffcc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/phones/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cffcc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cffcc-118">Request headers</span></span>

| <span data-ttu-id="cffcc-119">名称</span><span class="sxs-lookup"><span data-stu-id="cffcc-119">Name</span></span>           |<span data-ttu-id="cffcc-120">说明</span><span class="sxs-lookup"><span data-stu-id="cffcc-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="cffcc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cffcc-121">Authorization</span></span>  | <span data-ttu-id="cffcc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cffcc-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="cffcc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cffcc-124">Content-Type</span></span>   | <span data-ttu-id="cffcc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cffcc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cffcc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cffcc-127">Request body</span></span>

<span data-ttu-id="cffcc-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cffcc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cffcc-129">响应</span><span class="sxs-lookup"><span data-stu-id="cffcc-129">Response</span></span>

<span data-ttu-id="cffcc-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cffcc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cffcc-132">示例</span><span class="sxs-lookup"><span data-stu-id="cffcc-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cffcc-133">请求</span><span class="sxs-lookup"><span data-stu-id="cffcc-133">Request</span></span>

<span data-ttu-id="cffcc-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cffcc-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cffcc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cffcc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/phones/{id}
```
# <a name="c"></a>[<span data-ttu-id="cffcc-136">C#</span><span class="sxs-lookup"><span data-stu-id="cffcc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cffcc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cffcc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cffcc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cffcc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cffcc-139">响应</span><span class="sxs-lookup"><span data-stu-id="cffcc-139">Response</span></span>

<span data-ttu-id="cffcc-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cffcc-140">The following is an example of the response.</span></span>

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
  "description": "Delete itemPhone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
