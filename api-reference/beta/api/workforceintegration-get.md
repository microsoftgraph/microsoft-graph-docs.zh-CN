---
title: 获取 workforceIntegration
description: 检索 workforceintegration 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 98c30115fabbefd32ae0d82ce3cc1e4f0de5cab5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970729"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="4fe34-103">获取 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="4fe34-103">Get workforceIntegration</span></span>

<span data-ttu-id="4fe34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fe34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fe34-105">检索 [workforceintegration](../resources/workforceintegration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4fe34-105">Retrieve the properties and relationships of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fe34-106">权限</span><span class="sxs-lookup"><span data-stu-id="4fe34-106">Permissions</span></span>

<span data-ttu-id="4fe34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fe34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fe34-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fe34-109">Permission type</span></span>                        | <span data-ttu-id="4fe34-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fe34-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4fe34-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fe34-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fe34-112">WorkforceIntegration、WorkforceIntegration 和所有</span><span class="sxs-lookup"><span data-stu-id="4fe34-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="4fe34-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fe34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fe34-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fe34-114">Not supported.</span></span> |
| <span data-ttu-id="4fe34-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fe34-115">Application</span></span>                            | <span data-ttu-id="4fe34-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fe34-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fe34-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fe34-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4fe34-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4fe34-118">Optional query parameters</span></span>

<span data-ttu-id="4fe34-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4fe34-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4fe34-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4fe34-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fe34-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fe34-121">Request headers</span></span>

| <span data-ttu-id="4fe34-122">名称</span><span class="sxs-lookup"><span data-stu-id="4fe34-122">Name</span></span>      |<span data-ttu-id="4fe34-123">说明</span><span class="sxs-lookup"><span data-stu-id="4fe34-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4fe34-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fe34-124">Authorization</span></span> | <span data-ttu-id="4fe34-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4fe34-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fe34-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fe34-126">Request body</span></span>

<span data-ttu-id="4fe34-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4fe34-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fe34-128">响应</span><span class="sxs-lookup"><span data-stu-id="4fe34-128">Response</span></span>

<span data-ttu-id="4fe34-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [workforceIntegration](../resources/workforceintegration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fe34-129">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4fe34-130">示例</span><span class="sxs-lookup"><span data-stu-id="4fe34-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4fe34-131">请求</span><span class="sxs-lookup"><span data-stu-id="4fe34-131">Request</span></span>

<span data-ttu-id="4fe34-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4fe34-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4fe34-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fe34-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceintegrationid}
```
# <a name="c"></a>[<span data-ttu-id="4fe34-134">C#</span><span class="sxs-lookup"><span data-stu-id="4fe34-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4fe34-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fe34-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fe34-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fe34-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4fe34-137">Java</span><span class="sxs-lookup"><span data-stu-id="4fe34-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4fe34-138">响应</span><span class="sxs-lookup"><span data-stu-id="4fe34-138">Response</span></span>

<span data-ttu-id="4fe34-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4fe34-139">The following is an example of the response.</span></span>

> <span data-ttu-id="4fe34-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4fe34-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "KronosWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://contosoWorkforceIntegration.com/Contoso/",
  "supports": "shift"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


