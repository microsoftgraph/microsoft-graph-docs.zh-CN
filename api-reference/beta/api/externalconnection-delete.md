---
title: 删除 externalConnection
description: 删除 externalConnection。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 37b46e3cd6de8a12d6a77106abbe81a8a5da090f
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943610"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="def0a-103">删除 externalConnection</span><span class="sxs-lookup"><span data-stu-id="def0a-103">Delete externalConnection</span></span>

<span data-ttu-id="def0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="def0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="def0a-105">删除 [externalConnection](../resources/externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="def0a-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="def0a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="def0a-106">Permissions</span></span>

<span data-ttu-id="def0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="def0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="def0a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="def0a-109">Permission type</span></span>                        | <span data-ttu-id="def0a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="def0a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="def0a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="def0a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="def0a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="def0a-112">Not supported.</span></span> |
| <span data-ttu-id="def0a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="def0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="def0a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="def0a-114">Not supported.</span></span> |
| <span data-ttu-id="def0a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="def0a-115">Application</span></span>                            | <span data-ttu-id="def0a-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def0a-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="def0a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="def0a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="def0a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="def0a-118">Request headers</span></span>

| <span data-ttu-id="def0a-119">名称</span><span class="sxs-lookup"><span data-stu-id="def0a-119">Name</span></span>          | <span data-ttu-id="def0a-120">说明</span><span class="sxs-lookup"><span data-stu-id="def0a-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="def0a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="def0a-121">Authorization</span></span> | <span data-ttu-id="def0a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="def0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="def0a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="def0a-124">Request body</span></span>

<span data-ttu-id="def0a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="def0a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="def0a-126">响应</span><span class="sxs-lookup"><span data-stu-id="def0a-126">Response</span></span>

<span data-ttu-id="def0a-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="def0a-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="def0a-129">示例</span><span class="sxs-lookup"><span data-stu-id="def0a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="def0a-130">请求</span><span class="sxs-lookup"><span data-stu-id="def0a-130">Request</span></span>

<span data-ttu-id="def0a-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="def0a-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="def0a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="def0a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="def0a-133">C#</span><span class="sxs-lookup"><span data-stu-id="def0a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="def0a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="def0a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="def0a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="def0a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="def0a-136">Java</span><span class="sxs-lookup"><span data-stu-id="def0a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="def0a-137">响应</span><span class="sxs-lookup"><span data-stu-id="def0a-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="def0a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="def0a-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete externalConnection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


