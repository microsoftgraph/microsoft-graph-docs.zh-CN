---
title: 获取 connectionOperation
description: 检索 connectionOperation 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f709d05f1b93b3443dffc5171da6deb39dadc187
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366574"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="e2c25-103">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="e2c25-103">Get connectionOperation</span></span>

<span data-ttu-id="e2c25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2c25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2c25-105">检索 [connectionOperation 的属性](../resources/connectionoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="e2c25-105">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e2c25-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e2c25-106">Permissions</span></span>

<span data-ttu-id="e2c25-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2c25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2c25-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2c25-109">Permission type</span></span>                        | <span data-ttu-id="e2c25-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2c25-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2c25-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2c25-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2c25-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2c25-112">Not supported.</span></span> |
| <span data-ttu-id="e2c25-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2c25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2c25-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2c25-114">Not supported.</span></span> |
| <span data-ttu-id="e2c25-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2c25-115">Application</span></span>                            | <span data-ttu-id="e2c25-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2c25-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2c25-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2c25-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="e2c25-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2c25-118">Request headers</span></span>

| <span data-ttu-id="e2c25-119">名称</span><span class="sxs-lookup"><span data-stu-id="e2c25-119">Name</span></span>          | <span data-ttu-id="e2c25-120">说明</span><span class="sxs-lookup"><span data-stu-id="e2c25-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e2c25-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2c25-121">Authorization</span></span> | <span data-ttu-id="e2c25-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2c25-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2c25-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2c25-124">Request body</span></span>

<span data-ttu-id="e2c25-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2c25-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2c25-126">响应</span><span class="sxs-lookup"><span data-stu-id="e2c25-126">Response</span></span>

<span data-ttu-id="e2c25-127">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [connectionOperation](../resources/connectionoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2c25-127">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2c25-128">示例</span><span class="sxs-lookup"><span data-stu-id="e2c25-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2c25-129">请求</span><span class="sxs-lookup"><span data-stu-id="e2c25-129">Request</span></span>

<span data-ttu-id="e2c25-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e2c25-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2c25-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2c25-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="c"></a>[<span data-ttu-id="e2c25-132">C#</span><span class="sxs-lookup"><span data-stu-id="e2c25-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2c25-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2c25-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2c25-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2c25-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2c25-135">Java</span><span class="sxs-lookup"><span data-stu-id="e2c25-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectionoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="e2c25-136">响应</span><span class="sxs-lookup"><span data-stu-id="e2c25-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="e2c25-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e2c25-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "expectError": true,
  "@odata.type": "microsoft.graph.connectionOperation"
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


