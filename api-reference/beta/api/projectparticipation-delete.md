---
title: 删除 projectParticipation
description: 从用户的配置文件中删除 projectParticipation 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 723385798068e12ae03e6cf48943034ee7c887de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454934"
---
# <a name="delete-projectparticipation"></a><span data-ttu-id="0ebb5-103">删除 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="0ebb5-103">Delete projectParticipation</span></span>

<span data-ttu-id="0ebb5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0ebb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ebb5-105">从用户的[配置文件](../resources/profile.md)中删除[projectParticipation](../resources/projectparticipation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ebb5-105">Delete a [projectParticipation](../resources/projectparticipation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ebb5-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ebb5-106">Permissions</span></span>

<span data-ttu-id="0ebb5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ebb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ebb5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ebb5-109">Permission type</span></span>                        | <span data-ttu-id="0ebb5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ebb5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ebb5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ebb5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ebb5-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="0ebb5-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0ebb5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ebb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ebb5-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="0ebb5-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0ebb5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ebb5-115">Application</span></span>                            | <span data-ttu-id="0ebb5-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ebb5-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0ebb5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ebb5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0ebb5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ebb5-118">Request headers</span></span>

| <span data-ttu-id="0ebb5-119">名称</span><span class="sxs-lookup"><span data-stu-id="0ebb5-119">Name</span></span>           |<span data-ttu-id="0ebb5-120">说明</span><span class="sxs-lookup"><span data-stu-id="0ebb5-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0ebb5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ebb5-121">Authorization</span></span>  | <span data-ttu-id="0ebb5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ebb5-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0ebb5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ebb5-124">Content-Type</span></span>   | <span data-ttu-id="0ebb5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ebb5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ebb5-127">Request body</span></span>

<span data-ttu-id="0ebb5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ebb5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ebb5-129">响应</span><span class="sxs-lookup"><span data-stu-id="0ebb5-129">Response</span></span>

<span data-ttu-id="0ebb5-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0ebb5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ebb5-132">示例</span><span class="sxs-lookup"><span data-stu-id="0ebb5-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ebb5-133">请求</span><span class="sxs-lookup"><span data-stu-id="0ebb5-133">Request</span></span>

<span data-ttu-id="0ebb5-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ebb5-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ebb5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ebb5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_projectparticipation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/projects/{id}
```
# <a name="c"></a>[<span data-ttu-id="0ebb5-136">C#</span><span class="sxs-lookup"><span data-stu-id="0ebb5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ebb5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ebb5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ebb5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ebb5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0ebb5-139">响应</span><span class="sxs-lookup"><span data-stu-id="0ebb5-139">Response</span></span>

<span data-ttu-id="0ebb5-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ebb5-140">The following is an example of the response.</span></span>

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
  "description": "Delete projectParticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
