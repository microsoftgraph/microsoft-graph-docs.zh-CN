---
title: 创建连接
description: 使用此 API 创建新的 externalConnection。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4a4f544b42ed6c102a43aaf6e5e5cacc1e5a2471
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994723"
---
# <a name="create-connection"></a><span data-ttu-id="7e1bd-103">创建连接</span><span class="sxs-lookup"><span data-stu-id="7e1bd-103">Create connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e1bd-104">创建新的[externalConnection](../resources/externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="7e1bd-104">Create a new [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e1bd-105">权限</span><span class="sxs-lookup"><span data-stu-id="7e1bd-105">Permissions</span></span>

<span data-ttu-id="7e1bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e1bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e1bd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e1bd-108">Permission type</span></span>                        | <span data-ttu-id="7e1bd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e1bd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7e1bd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e1bd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e1bd-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e1bd-111">Not supported.</span></span> |
| <span data-ttu-id="7e1bd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e1bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e1bd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e1bd-113">Not supported.</span></span> |
| <span data-ttu-id="7e1bd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e1bd-114">Application</span></span>                            | <span data-ttu-id="7e1bd-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e1bd-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e1bd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e1bd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="7e1bd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e1bd-117">Request headers</span></span>

| <span data-ttu-id="7e1bd-118">名称</span><span class="sxs-lookup"><span data-stu-id="7e1bd-118">Name</span></span>          | <span data-ttu-id="7e1bd-119">说明</span><span class="sxs-lookup"><span data-stu-id="7e1bd-119">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="7e1bd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e1bd-120">Authorization</span></span> | <span data-ttu-id="7e1bd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e1bd-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7e1bd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e1bd-123">Content-Type</span></span>  | <span data-ttu-id="7e1bd-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7e1bd-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e1bd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e1bd-126">Request body</span></span>

<span data-ttu-id="7e1bd-127">在请求正文中，提供[externalConnection](../resources/externalconnection.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e1bd-127">In the request body, supply a JSON representation of a [externalConnection](../resources/externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7e1bd-128">响应</span><span class="sxs-lookup"><span data-stu-id="7e1bd-128">Response</span></span>

<span data-ttu-id="7e1bd-129">如果成功，此方法在`201 Created`响应正文中返回响应代码和新的[externalConnection](../resources/externalconnection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7e1bd-129">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e1bd-130">示例</span><span class="sxs-lookup"><span data-stu-id="7e1bd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e1bd-131">请求</span><span class="sxs-lookup"><span data-stu-id="7e1bd-131">Request</span></span>

<span data-ttu-id="7e1bd-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e1bd-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7e1bd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e1bd-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e1bd-134">C#</span><span class="sxs-lookup"><span data-stu-id="7e1bd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connection-from-external-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e1bd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e1bd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connection-from-external-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e1bd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e1bd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connection-from-external-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="7e1bd-137">响应</span><span class="sxs-lookup"><span data-stu-id="7e1bd-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7e1bd-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e1bd-138">The following is an example of the response.</span></span>

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
