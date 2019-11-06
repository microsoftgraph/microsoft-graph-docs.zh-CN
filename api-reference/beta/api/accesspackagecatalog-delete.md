---
title: 删除 accessPackageCatalog
description: 删除 accessPackageCatalog。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 063b2baff5ad2bae4ff9ea68e32daf689ceca6dc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994324"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="cfc86-103">删除 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="cfc86-103">Delete accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfc86-104">删除[accessPackageCatalog](../resources/accesspackagecatalog.md)。</span><span class="sxs-lookup"><span data-stu-id="cfc86-104">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cfc86-105">权限</span><span class="sxs-lookup"><span data-stu-id="cfc86-105">Permissions</span></span>

<span data-ttu-id="cfc86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfc86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cfc86-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfc86-108">Permission type</span></span>                        | <span data-ttu-id="cfc86-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfc86-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cfc86-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfc86-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfc86-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfc86-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="cfc86-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfc86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfc86-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfc86-113">Not supported.</span></span> |
| <span data-ttu-id="cfc86-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfc86-114">Application</span></span>                            | <span data-ttu-id="cfc86-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfc86-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfc86-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfc86-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cfc86-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfc86-117">Request headers</span></span>

| <span data-ttu-id="cfc86-118">名称</span><span class="sxs-lookup"><span data-stu-id="cfc86-118">Name</span></span>          | <span data-ttu-id="cfc86-119">说明</span><span class="sxs-lookup"><span data-stu-id="cfc86-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cfc86-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfc86-120">Authorization</span></span> | <span data-ttu-id="cfc86-121">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="cfc86-121">Bearer \{token\}.</span></span> <span data-ttu-id="cfc86-122">必填。</span><span class="sxs-lookup"><span data-stu-id="cfc86-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfc86-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfc86-123">Request body</span></span>

<span data-ttu-id="cfc86-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfc86-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfc86-125">响应</span><span class="sxs-lookup"><span data-stu-id="cfc86-125">Response</span></span>

<span data-ttu-id="cfc86-126">如果成功，此方法将返回一个200系列响应代码。</span><span class="sxs-lookup"><span data-stu-id="cfc86-126">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="cfc86-127">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cfc86-127">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfc86-128">示例</span><span class="sxs-lookup"><span data-stu-id="cfc86-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfc86-129">请求</span><span class="sxs-lookup"><span data-stu-id="cfc86-129">Request</span></span>

<span data-ttu-id="cfc86-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cfc86-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cfc86-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfc86-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfc86-132">C#</span><span class="sxs-lookup"><span data-stu-id="cfc86-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfc86-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cfc86-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfc86-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cfc86-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cfc86-135">响应</span><span class="sxs-lookup"><span data-stu-id="cfc86-135">Response</span></span>

<span data-ttu-id="cfc86-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cfc86-136">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
