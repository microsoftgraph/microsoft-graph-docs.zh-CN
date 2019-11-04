---
title: 创建连接
description: 使用此 API 创建新的 externalConnection。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6b85c5a9a09690f91f3e0934512f3cc874e54b46
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938679"
---
# <a name="create-connection"></a><span data-ttu-id="7fff3-103">创建连接</span><span class="sxs-lookup"><span data-stu-id="7fff3-103">Create connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fff3-104">创建新的[externalConnection](../resources/externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="7fff3-104">Create a new [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7fff3-105">权限</span><span class="sxs-lookup"><span data-stu-id="7fff3-105">Permissions</span></span>

<span data-ttu-id="7fff3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7fff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7fff3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fff3-108">Permission type</span></span>                        | <span data-ttu-id="7fff3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7fff3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7fff3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fff3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7fff3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fff3-111">Not supported.</span></span> |
| <span data-ttu-id="7fff3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fff3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fff3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fff3-113">Not supported.</span></span> |
| <span data-ttu-id="7fff3-114">Application</span><span class="sxs-lookup"><span data-stu-id="7fff3-114">Application</span></span>                            | <span data-ttu-id="7fff3-115">ExternalItem</span><span class="sxs-lookup"><span data-stu-id="7fff3-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fff3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fff3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="7fff3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fff3-117">Request headers</span></span>

| <span data-ttu-id="7fff3-118">名称</span><span class="sxs-lookup"><span data-stu-id="7fff3-118">Name</span></span>          | <span data-ttu-id="7fff3-119">说明</span><span class="sxs-lookup"><span data-stu-id="7fff3-119">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="7fff3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fff3-120">Authorization</span></span> | <span data-ttu-id="7fff3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7fff3-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7fff3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7fff3-123">Content-Type</span></span>  | <span data-ttu-id="7fff3-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7fff3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fff3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fff3-126">Request body</span></span>

<span data-ttu-id="7fff3-127">在请求正文中，提供[externalConnection](../resources/externalconnection.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fff3-127">In the request body, supply a JSON representation of a [externalConnection](../resources/externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7fff3-128">响应</span><span class="sxs-lookup"><span data-stu-id="7fff3-128">Response</span></span>

<span data-ttu-id="7fff3-129">如果成功，此方法在`201 Created`响应正文中返回响应代码和新的[externalConnection](../resources/externalconnection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7fff3-129">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fff3-130">示例</span><span class="sxs-lookup"><span data-stu-id="7fff3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7fff3-131">请求</span><span class="sxs-lookup"><span data-stu-id="7fff3-131">Request</span></span>

<span data-ttu-id="7fff3-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7fff3-132">The following is an example of the request.</span></span>
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

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="7fff3-133">响应</span><span class="sxs-lookup"><span data-stu-id="7fff3-133">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7fff3-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7fff3-134">The following is an example of the response.</span></span>

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
