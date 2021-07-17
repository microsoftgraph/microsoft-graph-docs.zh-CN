---
title: 获取 connectionOperation
description: 检索 connectionOperation 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 1592c1fc4a47195d51f1a744884680a4467b171b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467588"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="b47d9-103">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="b47d9-103">Get connectionOperation</span></span>

<span data-ttu-id="b47d9-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="b47d9-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b47d9-105">检索 [connectionOperation 的属性](../resources/externalconnectors-connectionoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="b47d9-105">Retrieve the properties of a [connectionOperation](../resources/externalconnectors-connectionoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b47d9-106">权限</span><span class="sxs-lookup"><span data-stu-id="b47d9-106">Permissions</span></span>

<span data-ttu-id="b47d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b47d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b47d9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b47d9-109">Permission type</span></span>                        | <span data-ttu-id="b47d9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b47d9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b47d9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b47d9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b47d9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b47d9-112">Not supported.</span></span> |
| <span data-ttu-id="b47d9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b47d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b47d9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b47d9-114">Not supported.</span></span> |
| <span data-ttu-id="b47d9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b47d9-115">Application</span></span>                            | <span data-ttu-id="b47d9-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="b47d9-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="b47d9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b47d9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="b47d9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b47d9-118">Request headers</span></span>

| <span data-ttu-id="b47d9-119">名称</span><span class="sxs-lookup"><span data-stu-id="b47d9-119">Name</span></span>          | <span data-ttu-id="b47d9-120">说明</span><span class="sxs-lookup"><span data-stu-id="b47d9-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b47d9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b47d9-121">Authorization</span></span> | <span data-ttu-id="b47d9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b47d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b47d9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b47d9-124">Request body</span></span>

<span data-ttu-id="b47d9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b47d9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b47d9-126">响应</span><span class="sxs-lookup"><span data-stu-id="b47d9-126">Response</span></span>

<span data-ttu-id="b47d9-127">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [connectionOperation](../resources/externalconnectors-connectionoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b47d9-127">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/externalconnectors-connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b47d9-128">示例</span><span class="sxs-lookup"><span data-stu-id="b47d9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b47d9-129">请求</span><span class="sxs-lookup"><span data-stu-id="b47d9-129">Request</span></span>

<span data-ttu-id="b47d9-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b47d9-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b47d9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b47d9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="c"></a>[<span data-ttu-id="b47d9-132">C#</span><span class="sxs-lookup"><span data-stu-id="b47d9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b47d9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b47d9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b47d9-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b47d9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b47d9-135">Java</span><span class="sxs-lookup"><span data-stu-id="b47d9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectionoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b47d9-136">响应</span><span class="sxs-lookup"><span data-stu-id="b47d9-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b47d9-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b47d9-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "expectError": true,
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "3ed1595a-4bae-43c2-acda-ef973e581323",
  "status": "failed",
  "error": {
    "message": "Server error, something went wrong"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectionOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
