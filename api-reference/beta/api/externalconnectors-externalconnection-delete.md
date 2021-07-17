---
title: 删除 externalConnection
description: 删除 externalConnection。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a33561b82527ab4494303b3b7cb092f0b7a57a7a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467586"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="26109-103">删除 externalConnection</span><span class="sxs-lookup"><span data-stu-id="26109-103">Delete externalConnection</span></span>

<span data-ttu-id="26109-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="26109-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26109-105">删除 [externalConnection](../resources/externalconnectors-externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="26109-105">Delete an [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26109-106">权限</span><span class="sxs-lookup"><span data-stu-id="26109-106">Permissions</span></span>

<span data-ttu-id="26109-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26109-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="26109-109">Permission type</span></span>                        | <span data-ttu-id="26109-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26109-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26109-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26109-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26109-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="26109-112">Not supported.</span></span> |
| <span data-ttu-id="26109-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26109-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26109-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="26109-114">Not supported.</span></span> |
| <span data-ttu-id="26109-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="26109-115">Application</span></span>                            | <span data-ttu-id="26109-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="26109-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="26109-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26109-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26109-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="26109-118">Request headers</span></span>

| <span data-ttu-id="26109-119">名称</span><span class="sxs-lookup"><span data-stu-id="26109-119">Name</span></span>          | <span data-ttu-id="26109-120">说明</span><span class="sxs-lookup"><span data-stu-id="26109-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="26109-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="26109-121">Authorization</span></span> | <span data-ttu-id="26109-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26109-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26109-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="26109-124">Request body</span></span>

<span data-ttu-id="26109-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26109-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26109-126">响应</span><span class="sxs-lookup"><span data-stu-id="26109-126">Response</span></span>

<span data-ttu-id="26109-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="26109-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26109-129">示例</span><span class="sxs-lookup"><span data-stu-id="26109-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26109-130">请求</span><span class="sxs-lookup"><span data-stu-id="26109-130">Request</span></span>

<span data-ttu-id="26109-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26109-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26109-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="26109-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="26109-133">C#</span><span class="sxs-lookup"><span data-stu-id="26109-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26109-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26109-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26109-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26109-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26109-136">Java</span><span class="sxs-lookup"><span data-stu-id="26109-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="26109-137">响应</span><span class="sxs-lookup"><span data-stu-id="26109-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="26109-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26109-138">The following is an example of the response.</span></span>

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


