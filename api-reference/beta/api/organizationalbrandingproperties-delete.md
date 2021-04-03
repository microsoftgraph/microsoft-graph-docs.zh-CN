---
title: 删除 organizationalBrandingProperties
description: 删除 organizationalBrandingProperties。
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: eba5a039143c55b4ac77610ac07a5a721ae3a3f4
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582730"
---
# <a name="delete-organizationalbrandingproperties"></a><span data-ttu-id="ac057-103">删除 organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="ac057-103">Delete organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac057-104">删除 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac057-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac057-105">权限</span><span class="sxs-lookup"><span data-stu-id="ac057-105">Permissions</span></span>

<span data-ttu-id="ac057-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac057-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac057-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac057-108">Permission type</span></span>                        | <span data-ttu-id="ac057-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac057-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ac057-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac057-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac057-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac057-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="ac057-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac057-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac057-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac057-113">Not supported.</span></span> |
| <span data-ttu-id="ac057-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac057-114">Application</span></span>                            | <span data-ttu-id="ac057-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac057-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac057-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac057-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="ac057-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac057-117">Request headers</span></span>

| <span data-ttu-id="ac057-118">名称</span><span class="sxs-lookup"><span data-stu-id="ac057-118">Name</span></span>          | <span data-ttu-id="ac057-119">说明</span><span class="sxs-lookup"><span data-stu-id="ac057-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ac057-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac057-120">Authorization</span></span> | <span data-ttu-id="ac057-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac057-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac057-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac057-123">Request body</span></span>

<span data-ttu-id="ac057-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ac057-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac057-125">响应</span><span class="sxs-lookup"><span data-stu-id="ac057-125">Response</span></span>

<span data-ttu-id="ac057-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ac057-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac057-128">示例</span><span class="sxs-lookup"><span data-stu-id="ac057-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac057-129">请求</span><span class="sxs-lookup"><span data-stu-id="ac057-129">Request</span></span>

<span data-ttu-id="ac057-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac057-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac057-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac057-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties_1"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="ac057-132">C#</span><span class="sxs-lookup"><span data-stu-id="ac057-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac057-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac057-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac057-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac057-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac057-135">Java</span><span class="sxs-lookup"><span data-stu-id="ac057-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac057-136">响应</span><span class="sxs-lookup"><span data-stu-id="ac057-136">Response</span></span>

<span data-ttu-id="ac057-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac057-137">The following is an example of the response.</span></span>

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
  "description": "Delete organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
