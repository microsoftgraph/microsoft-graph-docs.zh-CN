---
title: 获取 connectionOperation
description: 检索 connectionOperation 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 76936584883549fb2fd2fedbeed42cbe78702e55
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936592"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="94c08-103">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="94c08-103">Get connectionOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94c08-104">检索[connectionOperation](../resources/connectionoperation.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="94c08-104">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94c08-105">权限</span><span class="sxs-lookup"><span data-stu-id="94c08-105">Permissions</span></span>

<span data-ttu-id="94c08-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94c08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94c08-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="94c08-108">Permission type</span></span>                        | <span data-ttu-id="94c08-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94c08-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94c08-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94c08-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="94c08-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="94c08-111">Not supported.</span></span> |
| <span data-ttu-id="94c08-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94c08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94c08-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="94c08-113">Not supported.</span></span> |
| <span data-ttu-id="94c08-114">Application</span><span class="sxs-lookup"><span data-stu-id="94c08-114">Application</span></span>                            | <span data-ttu-id="94c08-115">ExternalItem</span><span class="sxs-lookup"><span data-stu-id="94c08-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94c08-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94c08-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="94c08-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="94c08-117">Request headers</span></span>

| <span data-ttu-id="94c08-118">名称</span><span class="sxs-lookup"><span data-stu-id="94c08-118">Name</span></span>          | <span data-ttu-id="94c08-119">说明</span><span class="sxs-lookup"><span data-stu-id="94c08-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="94c08-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="94c08-120">Authorization</span></span> | <span data-ttu-id="94c08-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94c08-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94c08-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="94c08-123">Request body</span></span>

<span data-ttu-id="94c08-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94c08-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94c08-125">响应</span><span class="sxs-lookup"><span data-stu-id="94c08-125">Response</span></span>

<span data-ttu-id="94c08-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[connectionOperation](../resources/connectionoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94c08-126">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94c08-127">示例</span><span class="sxs-lookup"><span data-stu-id="94c08-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94c08-128">请求</span><span class="sxs-lookup"><span data-stu-id="94c08-128">Request</span></span>

<span data-ttu-id="94c08-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94c08-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```http
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="94c08-130">响应</span><span class="sxs-lookup"><span data-stu-id="94c08-130">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="94c08-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94c08-131">The following is an example of the response.</span></span>

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
