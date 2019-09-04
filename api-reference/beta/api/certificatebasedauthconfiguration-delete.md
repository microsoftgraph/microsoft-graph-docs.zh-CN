---
title: 删除 certificateBasedAuthConfiguration
description: 删除 certificateBasedAuthConfiguration。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce54ddecbaa166a64ba5379c09729af44baad7d8
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718729"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="0df23-103">删除 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="0df23-103">Delete certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df23-104">删除[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0df23-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0df23-105">权限</span><span class="sxs-lookup"><span data-stu-id="0df23-105">Permissions</span></span>

<span data-ttu-id="0df23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0df23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0df23-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0df23-108">Permission type</span></span>                        | <span data-ttu-id="0df23-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0df23-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0df23-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0df23-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0df23-111">组织关系。 All</span><span class="sxs-lookup"><span data-stu-id="0df23-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="0df23-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0df23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0df23-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0df23-113">Not supported.</span></span> |
| <span data-ttu-id="0df23-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0df23-114">Application</span></span>    | <span data-ttu-id="0df23-115">组织关系。 All</span><span class="sxs-lookup"><span data-stu-id="0df23-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0df23-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0df23-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0df23-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0df23-117">Request headers</span></span>

| <span data-ttu-id="0df23-118">名称</span><span class="sxs-lookup"><span data-stu-id="0df23-118">Name</span></span>          | <span data-ttu-id="0df23-119">说明</span><span class="sxs-lookup"><span data-stu-id="0df23-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0df23-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0df23-120">Authorization</span></span> | <span data-ttu-id="0df23-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0df23-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0df23-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="0df23-122">Request body</span></span>

<span data-ttu-id="0df23-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0df23-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0df23-124">响应</span><span class="sxs-lookup"><span data-stu-id="0df23-124">Response</span></span>

<span data-ttu-id="0df23-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0df23-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0df23-127">示例</span><span class="sxs-lookup"><span data-stu-id="0df23-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0df23-128">请求</span><span class="sxs-lookup"><span data-stu-id="0df23-128">Request</span></span>

<span data-ttu-id="0df23-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0df23-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0df23-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0df23-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0df23-131">C#</span><span class="sxs-lookup"><span data-stu-id="0df23-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0df23-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0df23-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0df23-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="0df23-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0df23-134">响应</span><span class="sxs-lookup"><span data-stu-id="0df23-134">Response</span></span>

<span data-ttu-id="0df23-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0df23-135">The following is an example of the response.</span></span>

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
  "description": "Delete certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
