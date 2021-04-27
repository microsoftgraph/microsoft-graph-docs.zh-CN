---
title: 获取威胁情报指示器
description: 检索 tiindicator 对象的属性和关系。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 7ae7d1dc59493454a3fef55948bb712a3aa1c772
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036399"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="1ce98-103">获取威胁情报指示器</span><span class="sxs-lookup"><span data-stu-id="1ce98-103">Get threat intelligence indicator</span></span>

<span data-ttu-id="1ce98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ce98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ce98-105">检索 [tiIndicator](../resources/tiindicator.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ce98-105">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ce98-106">权限</span><span class="sxs-lookup"><span data-stu-id="1ce98-106">Permissions</span></span>

<span data-ttu-id="1ce98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ce98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ce98-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ce98-109">Permission type</span></span>                        | <span data-ttu-id="1ce98-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ce98-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ce98-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ce98-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ce98-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1ce98-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="1ce98-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ce98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ce98-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ce98-114">Not supported.</span></span> |
| <span data-ttu-id="1ce98-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ce98-115">Application</span></span>                            | <span data-ttu-id="1ce98-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1ce98-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ce98-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ce98-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ce98-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1ce98-118">Optional query parameters</span></span>

<span data-ttu-id="1ce98-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1ce98-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1ce98-120">有关一般信息，请参阅 [OData Query Parameters](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1ce98-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ce98-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ce98-121">Request headers</span></span>

| <span data-ttu-id="1ce98-122">名称</span><span class="sxs-lookup"><span data-stu-id="1ce98-122">Name</span></span>      |<span data-ttu-id="1ce98-123">说明</span><span class="sxs-lookup"><span data-stu-id="1ce98-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1ce98-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ce98-124">Authorization</span></span> | <span data-ttu-id="1ce98-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1ce98-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ce98-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ce98-126">Request body</span></span>

<span data-ttu-id="1ce98-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ce98-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ce98-128">响应</span><span class="sxs-lookup"><span data-stu-id="1ce98-128">Response</span></span>

<span data-ttu-id="1ce98-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ce98-129">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ce98-130">示例</span><span class="sxs-lookup"><span data-stu-id="1ce98-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ce98-131">请求</span><span class="sxs-lookup"><span data-stu-id="1ce98-131">Request</span></span>

<span data-ttu-id="1ce98-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ce98-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ce98-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ce98-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="c"></a>[<span data-ttu-id="1ce98-134">C#</span><span class="sxs-lookup"><span data-stu-id="1ce98-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ce98-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ce98-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ce98-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ce98-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ce98-137">Java</span><span class="sxs-lookup"><span data-stu-id="1ce98-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1ce98-138">响应</span><span class="sxs-lookup"><span data-stu-id="1ce98-138">Response</span></span>

<span data-ttu-id="1ce98-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ce98-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1ce98-140">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1ce98-140">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "action": "action-value",
  "activityGroupNames": [
    "activityGroupNames-value"
  ],
  "additionalInformation": "additionalInformation-value",
  "azureTenantId": "azureTenantId-value",
  "confidence": 99,
  "description": "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


