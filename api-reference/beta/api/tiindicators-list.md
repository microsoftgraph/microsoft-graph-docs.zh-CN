---
title: 列出威胁智能指示器
description: 检索 tiindicator 对象的列表。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c2b2549167f4bd861389672e211a854cc284a832
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637582"
---
# <a name="list-threat-intelligence-indicators"></a><span data-ttu-id="2bc77-103">列出威胁智能指示器</span><span class="sxs-lookup"><span data-stu-id="2bc77-103">List threat intelligence indicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bc77-104">检索[tiIndicator](../resources/tiindicator.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2bc77-104">Retrieve a list of [tiIndicator](../resources/tiindicator.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bc77-105">权限</span><span class="sxs-lookup"><span data-stu-id="2bc77-105">Permissions</span></span>

<span data-ttu-id="2bc77-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bc77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2bc77-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bc77-108">Permission type</span></span>     | <span data-ttu-id="2bc77-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2bc77-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2bc77-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bc77-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2bc77-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2bc77-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="2bc77-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bc77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bc77-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bc77-113">Not supported.</span></span> |
| <span data-ttu-id="2bc77-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bc77-114">Application</span></span>                            | <span data-ttu-id="2bc77-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2bc77-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bc77-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bc77-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2bc77-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2bc77-117">Optional query parameters</span></span>

<span data-ttu-id="2bc77-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2bc77-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2bc77-119">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2bc77-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bc77-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bc77-120">Request headers</span></span>

| <span data-ttu-id="2bc77-121">名称</span><span class="sxs-lookup"><span data-stu-id="2bc77-121">Name</span></span>      |<span data-ttu-id="2bc77-122">说明</span><span class="sxs-lookup"><span data-stu-id="2bc77-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2bc77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bc77-123">Authorization</span></span> | <span data-ttu-id="2bc77-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2bc77-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bc77-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bc77-125">Request body</span></span>

<span data-ttu-id="2bc77-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2bc77-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bc77-127">响应</span><span class="sxs-lookup"><span data-stu-id="2bc77-127">Response</span></span>

<span data-ttu-id="2bc77-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[tiIndicator](../resources/tiindicator.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="2bc77-128">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2bc77-129">示例</span><span class="sxs-lookup"><span data-stu-id="2bc77-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2bc77-130">请求</span><span class="sxs-lookup"><span data-stu-id="2bc77-130">Request</span></span>

<span data-ttu-id="2bc77-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2bc77-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tiindicators"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators
```

### <a name="response"></a><span data-ttu-id="2bc77-132">响应</span><span class="sxs-lookup"><span data-stu-id="2bc77-132">Response</span></span>

<span data-ttu-id="2bc77-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2bc77-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="2bc77-134">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2bc77-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2bc77-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2bc77-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2bc77-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="2bc77-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2bc77-137">语言</span><span class="sxs-lookup"><span data-stu-id="2bc77-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tiindicators-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2bc77-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="2bc77-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tiindicators-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicators-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicators-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
