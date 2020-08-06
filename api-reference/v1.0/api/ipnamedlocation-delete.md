---
title: 删除 ipNamedLocation
description: 删除 ipNamedLocation 对象。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c06b6d594e9b6772ef466c21f324ab8ae68a2fb4
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565020"
---
# <a name="delete-ipnamedlocation"></a><span data-ttu-id="cfef1-103">删除 ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="cfef1-103">Delete ipNamedLocation</span></span>

<span data-ttu-id="cfef1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfef1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cfef1-105">删除[ipNamedLocation](../resources/ipNamedLocation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cfef1-105">Delete an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfef1-106">权限</span><span class="sxs-lookup"><span data-stu-id="cfef1-106">Permissions</span></span>

<span data-ttu-id="cfef1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfef1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfef1-109">Permission type</span></span>                        | <span data-ttu-id="cfef1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfef1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cfef1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfef1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfef1-112">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="cfef1-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="cfef1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfef1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfef1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfef1-114">Not supported.</span></span> |
| <span data-ttu-id="cfef1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfef1-115">Application</span></span>                            | <span data-ttu-id="cfef1-116">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="cfef1-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfef1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfef1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cfef1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfef1-118">Request headers</span></span>

| <span data-ttu-id="cfef1-119">名称</span><span class="sxs-lookup"><span data-stu-id="cfef1-119">Name</span></span>          | <span data-ttu-id="cfef1-120">说明</span><span class="sxs-lookup"><span data-stu-id="cfef1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cfef1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfef1-121">Authorization</span></span> | <span data-ttu-id="cfef1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfef1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfef1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfef1-124">Request body</span></span>

<span data-ttu-id="cfef1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfef1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfef1-126">响应</span><span class="sxs-lookup"><span data-stu-id="cfef1-126">Response</span></span>

<span data-ttu-id="cfef1-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cfef1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfef1-129">示例</span><span class="sxs-lookup"><span data-stu-id="cfef1-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfef1-130">请求</span><span class="sxs-lookup"><span data-stu-id="cfef1-130">Request</span></span>

<span data-ttu-id="cfef1-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cfef1-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cfef1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfef1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_ipnamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="cfef1-133">C#</span><span class="sxs-lookup"><span data-stu-id="cfef1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cfef1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfef1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cfef1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfef1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cfef1-136">Java</span><span class="sxs-lookup"><span data-stu-id="cfef1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-ipnamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cfef1-137">响应</span><span class="sxs-lookup"><span data-stu-id="cfef1-137">Response</span></span>

<span data-ttu-id="cfef1-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cfef1-138">The following is an example of the response.</span></span>

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
  "description": "Delete ipNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
