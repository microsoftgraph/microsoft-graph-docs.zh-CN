---
title: 删除本地化的组织BrandingProperties
description: 删除 organizationalBrandingProperties 以用于特定本地化。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 938a45dfe29d9473d57571f7b10e5693d8d8de05
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943850"
---
# <a name="delete-localized-organizationalbrandingproperties"></a><span data-ttu-id="f2cc9-103">删除本地化的组织BrandingProperties</span><span class="sxs-lookup"><span data-stu-id="f2cc9-103">Delete Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2cc9-104">删除 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2cc9-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2cc9-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2cc9-105">Permissions</span></span>

<span data-ttu-id="f2cc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2cc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2cc9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2cc9-108">Permission type</span></span>                        | <span data-ttu-id="f2cc9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2cc9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f2cc9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2cc9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2cc9-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2cc9-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="f2cc9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2cc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2cc9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2cc9-113">Not supported.</span></span> |
| <span data-ttu-id="f2cc9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2cc9-114">Application</span></span>                            | <span data-ttu-id="f2cc9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2cc9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2cc9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2cc9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="f2cc9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2cc9-117">Request headers</span></span>

| <span data-ttu-id="f2cc9-118">名称</span><span class="sxs-lookup"><span data-stu-id="f2cc9-118">Name</span></span>          | <span data-ttu-id="f2cc9-119">说明</span><span class="sxs-lookup"><span data-stu-id="f2cc9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f2cc9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2cc9-120">Authorization</span></span> | <span data-ttu-id="f2cc9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2cc9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2cc9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2cc9-123">Request body</span></span>

<span data-ttu-id="f2cc9-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2cc9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2cc9-125">响应</span><span class="sxs-lookup"><span data-stu-id="f2cc9-125">Response</span></span>

<span data-ttu-id="f2cc9-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f2cc9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2cc9-128">示例</span><span class="sxs-lookup"><span data-stu-id="f2cc9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2cc9-129">请求</span><span class="sxs-lookup"><span data-stu-id="f2cc9-129">Request</span></span>

<span data-ttu-id="f2cc9-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f2cc9-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2cc9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2cc9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties_2"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="f2cc9-132">C#</span><span class="sxs-lookup"><span data-stu-id="f2cc9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-organizationalbrandingproperties-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2cc9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2cc9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-organizationalbrandingproperties-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2cc9-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2cc9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-organizationalbrandingproperties-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2cc9-135">Java</span><span class="sxs-lookup"><span data-stu-id="f2cc9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-organizationalbrandingproperties-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2cc9-136">响应</span><span class="sxs-lookup"><span data-stu-id="f2cc9-136">Response</span></span>

<span data-ttu-id="f2cc9-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f2cc9-137">The following is an example of the response.</span></span>

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
