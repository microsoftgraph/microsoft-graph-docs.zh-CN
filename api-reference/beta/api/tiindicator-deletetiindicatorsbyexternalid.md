---
title: 'tiIndicator: deleteTiIndicatorsByExternalId'
description: 在一个请求中 (而不是多个请求) 删除多个威胁情报 (TI) 指示器, 并且该请求包含外部 Id 而不是 Id。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 835bc4bfdda1cda355b907e0cdf143d09bbc0ccb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270684"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="6a690-103">tiIndicator: deleteTiIndicatorsByExternalId</span><span class="sxs-lookup"><span data-stu-id="6a690-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a690-104">当请求包含外部 Id 而不是 Id 时, 在一个请求中 (而不是多个请求) 删除多个威胁智能 (TI) 指示器。</span><span class="sxs-lookup"><span data-stu-id="6a690-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a690-105">权限</span><span class="sxs-lookup"><span data-stu-id="6a690-105">Permissions</span></span>

<span data-ttu-id="6a690-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a690-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a690-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a690-108">Permission type</span></span>  | <span data-ttu-id="6a690-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a690-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a690-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a690-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a690-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="6a690-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="6a690-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a690-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a690-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a690-113">Not supported.</span></span> |
| <span data-ttu-id="6a690-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a690-114">Application</span></span>                            | <span data-ttu-id="6a690-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="6a690-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a690-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a690-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="6a690-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a690-117">Request headers</span></span>

| <span data-ttu-id="6a690-118">名称</span><span class="sxs-lookup"><span data-stu-id="6a690-118">Name</span></span>          | <span data-ttu-id="6a690-119">说明</span><span class="sxs-lookup"><span data-stu-id="6a690-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6a690-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a690-120">Authorization</span></span> | <span data-ttu-id="6a690-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6a690-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a690-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a690-122">Request body</span></span>

<span data-ttu-id="6a690-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6a690-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6a690-124">参数</span><span class="sxs-lookup"><span data-stu-id="6a690-124">Parameter</span></span>    | <span data-ttu-id="6a690-125">类型</span><span class="sxs-lookup"><span data-stu-id="6a690-125">Type</span></span>        | <span data-ttu-id="6a690-126">说明</span><span class="sxs-lookup"><span data-stu-id="6a690-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a690-127">值</span><span class="sxs-lookup"><span data-stu-id="6a690-127">value</span></span>|<span data-ttu-id="6a690-128">String collection</span><span class="sxs-lookup"><span data-stu-id="6a690-128">String collection</span></span>| <span data-ttu-id="6a690-129">`externalIds`要删除的**tiIndicator**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="6a690-129">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="6a690-130">响应</span><span class="sxs-lookup"><span data-stu-id="6a690-130">Response</span></span>

<span data-ttu-id="6a690-131">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[resultInfo](../resources/resultinfo.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="6a690-131">If successful, this method returns `200 OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a690-132">示例</span><span class="sxs-lookup"><span data-stu-id="6a690-132">Examples</span></span>

<span data-ttu-id="6a690-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6a690-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6a690-134">请求</span><span class="sxs-lookup"><span data-stu-id="6a690-134">Request</span></span>

<span data-ttu-id="6a690-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6a690-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicatorsbyexternalid",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId
Content-type: application/json

{
  "value": [
    "externalId-value1",
    "externalId-value2"
  ]
}
```

### <a name="response"></a><span data-ttu-id="6a690-136">响应</span><span class="sxs-lookup"><span data-stu-id="6a690-136">Response</span></span>

<span data-ttu-id="6a690-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6a690-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="6a690-138">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6a690-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6a690-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6a690-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.resultInfo",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "code": "code-value",
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6a690-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6a690-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6a690-141">C#</span><span class="sxs-lookup"><span data-stu-id="6a690-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicatorsbyexternalid-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a690-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a690-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicatorsbyexternalid-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6a690-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="6a690-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tiindicator_deletetiindicatorsbyexternalid-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-deletetiindicatorsbyexternalid.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicatorsbyexternalid.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-deletetiindicatorsbyexternalid.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
