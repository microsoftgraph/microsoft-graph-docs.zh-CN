---
title: 'tiIndicator: deleteTiIndicatorsByExternalId'
description: 在一个请求中（而不是多个请求）删除多个威胁情报（TI）指示器，并且该请求包含外部 Id 而不是 Id。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 14beffbf72ee486e7182d7ae327e709b75a8c625
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006451"
---
# <a name="tiindicator-deletetiindicatorsbyexternalid"></a><span data-ttu-id="bd7dc-103">tiIndicator: deleteTiIndicatorsByExternalId</span><span class="sxs-lookup"><span data-stu-id="bd7dc-103">tiIndicator: deleteTiIndicatorsByExternalId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd7dc-104">当请求包含外部 Id 而不是 Id 时，在一个请求中（而不是多个请求）删除多个威胁智能（TI）指示器。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-104">Delete multiple threat intelligence (TI) indicators in one request instead of multiple requests, when the request contains external IDs instead of IDs.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd7dc-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="bd7dc-105">Permissions</span></span>

<span data-ttu-id="bd7dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd7dc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd7dc-108">Permission type</span></span>  | <span data-ttu-id="bd7dc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd7dc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd7dc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd7dc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd7dc-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="bd7dc-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="bd7dc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd7dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd7dc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-113">Not supported.</span></span> |
| <span data-ttu-id="bd7dc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd7dc-114">Application</span></span>                            | <span data-ttu-id="bd7dc-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="bd7dc-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd7dc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd7dc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/deleteTiIndicatorsByExternalId
```

## <a name="request-headers"></a><span data-ttu-id="bd7dc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd7dc-117">Request headers</span></span>

| <span data-ttu-id="bd7dc-118">名称</span><span class="sxs-lookup"><span data-stu-id="bd7dc-118">Name</span></span>          | <span data-ttu-id="bd7dc-119">说明</span><span class="sxs-lookup"><span data-stu-id="bd7dc-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd7dc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd7dc-120">Authorization</span></span> | <span data-ttu-id="bd7dc-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bd7dc-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd7dc-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd7dc-122">Request body</span></span>

<span data-ttu-id="bd7dc-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bd7dc-124">参数</span><span class="sxs-lookup"><span data-stu-id="bd7dc-124">Parameter</span></span>    | <span data-ttu-id="bd7dc-125">类型</span><span class="sxs-lookup"><span data-stu-id="bd7dc-125">Type</span></span>        | <span data-ttu-id="bd7dc-126">说明</span><span class="sxs-lookup"><span data-stu-id="bd7dc-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bd7dc-127">值</span><span class="sxs-lookup"><span data-stu-id="bd7dc-127">value</span></span>|<span data-ttu-id="bd7dc-128">String 集合</span><span class="sxs-lookup"><span data-stu-id="bd7dc-128">String collection</span></span>| <span data-ttu-id="bd7dc-129">`externalIds`要删除的**tiIndicator**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-129">Collection of `externalIds` of the **tiIndicator** objects to be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="bd7dc-130">响应</span><span class="sxs-lookup"><span data-stu-id="bd7dc-130">Response</span></span>

<span data-ttu-id="bd7dc-131">如果成功，此方法在`200, OK`响应正文中返回响应代码和[resultInfo](../resources/resultinfo.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-131">If successful, this method returns `200, OK` response code and a [resultInfo](../resources/resultinfo.md) collection object in the response body.</span></span> <span data-ttu-id="bd7dc-132">如果存在错误，则此方法返回`206 Partial Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-132">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="bd7dc-133">有关详细信息，请参阅[错误](../resources/security-error-codes.md#threat-indicator-bulk-action-errors)。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-133">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="bd7dc-134">示例</span><span class="sxs-lookup"><span data-stu-id="bd7dc-134">Examples</span></span>

<span data-ttu-id="bd7dc-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bd7dc-136">请求</span><span class="sxs-lookup"><span data-stu-id="bd7dc-136">Request</span></span>

<span data-ttu-id="bd7dc-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bd7dc-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd7dc-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd7dc-139">C#</span><span class="sxs-lookup"><span data-stu-id="bd7dc-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-deletetiindicatorsbyexternalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd7dc-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd7dc-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-deletetiindicatorsbyexternalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd7dc-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd7dc-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-deletetiindicatorsbyexternalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd7dc-142">响应</span><span class="sxs-lookup"><span data-stu-id="bd7dc-142">Response</span></span>

<span data-ttu-id="bd7dc-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="bd7dc-144">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bd7dc-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bd7dc-145">All the properties will be returned from an actual call.</span></span>

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
      "code": 0,
      "message": "message-value",
      "subCode": "subCode-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: deleteTiIndicatorsByExternalId",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
