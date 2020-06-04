---
title: 删除 countryNamedLocation
description: 删除 countryNamedLocation 对象。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ad89d4c61f7e624bf4fc02f86a57e0b03bbd4fb
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555811"
---
# <a name="delete-countrynamedlocation"></a><span data-ttu-id="7b090-103">删除 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="7b090-103">Delete countryNamedLocation</span></span>

<span data-ttu-id="7b090-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b090-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b090-105">删除[countryNamedLocation](../resources/countryNamedLocation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7b090-105">Delete a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b090-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7b090-106">Permissions</span></span>

<span data-ttu-id="7b090-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b090-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b090-109">Permission type</span></span>                        | <span data-ttu-id="7b090-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b090-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7b090-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b090-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b090-112">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="7b090-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="7b090-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b090-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b090-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b090-114">Not supported.</span></span> |
| <span data-ttu-id="7b090-115">Application</span><span class="sxs-lookup"><span data-stu-id="7b090-115">Application</span></span>                            | <span data-ttu-id="7b090-116">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="7b090-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b090-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b090-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7b090-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b090-118">Request headers</span></span>

| <span data-ttu-id="7b090-119">名称</span><span class="sxs-lookup"><span data-stu-id="7b090-119">Name</span></span>          | <span data-ttu-id="7b090-120">说明</span><span class="sxs-lookup"><span data-stu-id="7b090-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7b090-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b090-121">Authorization</span></span> | <span data-ttu-id="7b090-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b090-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b090-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b090-124">Request body</span></span>

<span data-ttu-id="7b090-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b090-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b090-126">响应</span><span class="sxs-lookup"><span data-stu-id="7b090-126">Response</span></span>

<span data-ttu-id="7b090-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7b090-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b090-129">示例</span><span class="sxs-lookup"><span data-stu-id="7b090-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b090-130">请求</span><span class="sxs-lookup"><span data-stu-id="7b090-130">Request</span></span>

<span data-ttu-id="7b090-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7b090-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b090-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b090-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_countrynamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="7b090-133">C#</span><span class="sxs-lookup"><span data-stu-id="7b090-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b090-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b090-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b090-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b090-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b090-136">响应</span><span class="sxs-lookup"><span data-stu-id="7b090-136">Response</span></span>

<span data-ttu-id="7b090-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7b090-137">The following is an example of the response.</span></span>

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
  "description": "Delete countryNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
