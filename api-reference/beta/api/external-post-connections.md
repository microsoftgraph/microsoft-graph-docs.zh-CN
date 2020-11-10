---
title: Create Connection
description: 使用此 API 创建新的 externalConnection。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 9f5b8381e999429fb29e718b199596d3f987a415
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965705"
---
# <a name="create-connection"></a><span data-ttu-id="93ccd-103">Create Connection</span><span class="sxs-lookup"><span data-stu-id="93ccd-103">Create connection</span></span>

<span data-ttu-id="93ccd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93ccd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93ccd-105">创建新的 [externalConnection](../resources/externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="93ccd-105">Create a new [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="93ccd-106">权限</span><span class="sxs-lookup"><span data-stu-id="93ccd-106">Permissions</span></span>

<span data-ttu-id="93ccd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93ccd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="93ccd-109">Permission type</span></span>                        | <span data-ttu-id="93ccd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93ccd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="93ccd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93ccd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="93ccd-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="93ccd-112">Not supported.</span></span> |
| <span data-ttu-id="93ccd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93ccd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93ccd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="93ccd-114">Not supported.</span></span> |
| <span data-ttu-id="93ccd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="93ccd-115">Application</span></span>                            | <span data-ttu-id="93ccd-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ccd-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93ccd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93ccd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="93ccd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="93ccd-118">Request headers</span></span>

| <span data-ttu-id="93ccd-119">名称</span><span class="sxs-lookup"><span data-stu-id="93ccd-119">Name</span></span>          | <span data-ttu-id="93ccd-120">说明</span><span class="sxs-lookup"><span data-stu-id="93ccd-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="93ccd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="93ccd-121">Authorization</span></span> | <span data-ttu-id="93ccd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93ccd-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="93ccd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93ccd-124">Content-Type</span></span>  | <span data-ttu-id="93ccd-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="93ccd-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93ccd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="93ccd-127">Request body</span></span>

<span data-ttu-id="93ccd-128">在请求正文中，提供 [externalConnection](../resources/externalconnection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93ccd-128">In the request body, supply a JSON representation of an [externalConnection](../resources/externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="93ccd-129">响应</span><span class="sxs-lookup"><span data-stu-id="93ccd-129">Response</span></span>

<span data-ttu-id="93ccd-130">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [externalConnection](../resources/externalconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93ccd-130">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93ccd-131">示例</span><span class="sxs-lookup"><span data-stu-id="93ccd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="93ccd-132">请求</span><span class="sxs-lookup"><span data-stu-id="93ccd-132">Request</span></span>

<span data-ttu-id="93ccd-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="93ccd-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93ccd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="93ccd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connection_from_external"
}-->

```http
POST https://graph.microsoft.com/beta/external/connections
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system"
}
```
# <a name="c"></a>[<span data-ttu-id="93ccd-135">C#</span><span class="sxs-lookup"><span data-stu-id="93ccd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connection-from-external-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93ccd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93ccd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connection-from-external-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93ccd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93ccd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connection-from-external-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93ccd-138">Java</span><span class="sxs-lookup"><span data-stu-id="93ccd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connection-from-external-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="93ccd-139">响应</span><span class="sxs-lookup"><span data-stu-id="93ccd-139">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="93ccd-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="93ccd-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "configuration": {
    "authorizedApps": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


