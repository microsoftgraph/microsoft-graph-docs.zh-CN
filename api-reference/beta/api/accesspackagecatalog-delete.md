---
title: 删除 accessPackageCatalog
description: 删除 accessPackageCatalog。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ad2dd60c9e2f104987edeef0bac46dcf940a14cd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439602"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="7969c-103">删除 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7969c-103">Delete accessPackageCatalog</span></span>

<span data-ttu-id="7969c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7969c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7969c-105">删除 [accessPackageCatalog](../resources/accesspackagecatalog.md)。</span><span class="sxs-lookup"><span data-stu-id="7969c-105">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7969c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7969c-106">Permissions</span></span>

<span data-ttu-id="7969c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7969c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7969c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7969c-109">Permission type</span></span>                        | <span data-ttu-id="7969c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7969c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7969c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7969c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7969c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7969c-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7969c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7969c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7969c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7969c-114">Not supported.</span></span> |
| <span data-ttu-id="7969c-115">Application</span><span class="sxs-lookup"><span data-stu-id="7969c-115">Application</span></span>                            | <span data-ttu-id="7969c-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7969c-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7969c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7969c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7969c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7969c-118">Request headers</span></span>

| <span data-ttu-id="7969c-119">名称</span><span class="sxs-lookup"><span data-stu-id="7969c-119">Name</span></span>          | <span data-ttu-id="7969c-120">说明</span><span class="sxs-lookup"><span data-stu-id="7969c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7969c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7969c-121">Authorization</span></span> | <span data-ttu-id="7969c-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="7969c-122">Bearer \{token\}.</span></span> <span data-ttu-id="7969c-123">必需。</span><span class="sxs-lookup"><span data-stu-id="7969c-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7969c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7969c-124">Request body</span></span>

<span data-ttu-id="7969c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7969c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7969c-126">响应</span><span class="sxs-lookup"><span data-stu-id="7969c-126">Response</span></span>

<span data-ttu-id="7969c-127">如果成功，此方法将返回 200 系列响应代码。</span><span class="sxs-lookup"><span data-stu-id="7969c-127">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="7969c-128">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7969c-128">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7969c-129">示例</span><span class="sxs-lookup"><span data-stu-id="7969c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7969c-130">请求</span><span class="sxs-lookup"><span data-stu-id="7969c-130">Request</span></span>

<span data-ttu-id="7969c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7969c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7969c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7969c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="7969c-133">C#</span><span class="sxs-lookup"><span data-stu-id="7969c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7969c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7969c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7969c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7969c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7969c-136">Java</span><span class="sxs-lookup"><span data-stu-id="7969c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7969c-137">响应</span><span class="sxs-lookup"><span data-stu-id="7969c-137">Response</span></span>

<span data-ttu-id="7969c-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7969c-138">The following is an example of the response.</span></span>

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


