---
title: 'tiIndicator: updateTiIndicators'
description: 在一个请求中（而不是多个请求）更新多个威胁智能 (TI) 指示器。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 0be11755ff976037ab593c3273ed70b30eb4e4dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076509"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="95189-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="95189-103">tiIndicator: updateTiIndicators</span></span>

<span data-ttu-id="95189-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95189-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95189-105">在一个请求中（而不是多个请求）更新多个威胁智能 (TI) 指示器。</span><span class="sxs-lookup"><span data-stu-id="95189-105">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="95189-106">权限</span><span class="sxs-lookup"><span data-stu-id="95189-106">Permissions</span></span>

<span data-ttu-id="95189-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95189-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="95189-109">Permission type</span></span>   | <span data-ttu-id="95189-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95189-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="95189-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95189-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="95189-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="95189-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="95189-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95189-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95189-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="95189-114">Not supported.</span></span> |
| <span data-ttu-id="95189-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="95189-115">Application</span></span>                            | <span data-ttu-id="95189-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="95189-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="95189-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95189-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="95189-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="95189-118">Request headers</span></span>

| <span data-ttu-id="95189-119">名称</span><span class="sxs-lookup"><span data-stu-id="95189-119">Name</span></span>          | <span data-ttu-id="95189-120">说明</span><span class="sxs-lookup"><span data-stu-id="95189-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="95189-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95189-121">Authorization</span></span> | <span data-ttu-id="95189-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="95189-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="95189-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="95189-123">Request body</span></span>

<span data-ttu-id="95189-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="95189-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="95189-125">有关可更新的属性的详细信息，请参阅 [更新 tiIndicator](tiindicator-update.md)。</span><span class="sxs-lookup"><span data-stu-id="95189-125">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span> <span data-ttu-id="95189-126">每个 tiIndicator 的必填字段为： `id` 、 `expirationDateTime` 、 `targetProduct` 。</span><span class="sxs-lookup"><span data-stu-id="95189-126">Required fields for each tiIndicator are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="95189-127">参数</span><span class="sxs-lookup"><span data-stu-id="95189-127">Parameter</span></span>    | <span data-ttu-id="95189-128">类型</span><span class="sxs-lookup"><span data-stu-id="95189-128">Type</span></span>        | <span data-ttu-id="95189-129">说明</span><span class="sxs-lookup"><span data-stu-id="95189-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="95189-130">值</span><span class="sxs-lookup"><span data-stu-id="95189-130">value</span></span>|<span data-ttu-id="95189-131">tiIndicator 集合</span><span class="sxs-lookup"><span data-stu-id="95189-131">tiIndicator collection</span></span>| <span data-ttu-id="95189-132">要更新的 **tiIndicators** 的集合。</span><span class="sxs-lookup"><span data-stu-id="95189-132">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="95189-133">每个实体都必须具有要更新的 **id** 和其他可编辑属性。</span><span class="sxs-lookup"><span data-stu-id="95189-133">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="95189-134">响应</span><span class="sxs-lookup"><span data-stu-id="95189-134">Response</span></span>

<span data-ttu-id="95189-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [tiIndicator](../resources/tiindicator.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="95189-135">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="95189-136">如果存在错误，则此方法返回 `206 Partial Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="95189-136">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="95189-137">有关详细信息，请参阅 [错误](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) 。</span><span class="sxs-lookup"><span data-stu-id="95189-137">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="95189-138">示例</span><span class="sxs-lookup"><span data-stu-id="95189-138">Examples</span></span>

<span data-ttu-id="95189-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="95189-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="95189-140">请求</span><span class="sxs-lookup"><span data-stu-id="95189-140">Request</span></span>

<span data-ttu-id="95189-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="95189-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95189-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="95189-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_updatetiindicators",
  "isCollection":true
}-->
```http
POST https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators
Content-type: application/json

{
  "value": [
    {
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "additionalInformation": "mytest"
    },
    {
      "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
      "additionalInformation": "test again"
    }
  ]
}

```
# <a name="c"></a>[<span data-ttu-id="95189-143">C#</span><span class="sxs-lookup"><span data-stu-id="95189-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95189-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95189-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95189-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95189-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95189-146">响应</span><span class="sxs-lookup"><span data-stu-id="95189-146">Response</span></span>

<span data-ttu-id="95189-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="95189-147">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="95189-148">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="95189-148">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="95189-149">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="95189-149">All the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "azureTenantId": "XXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": "mytest",
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a test indicator for demo purpose. Take no action on any observables set in this indicator.",
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: updateTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


