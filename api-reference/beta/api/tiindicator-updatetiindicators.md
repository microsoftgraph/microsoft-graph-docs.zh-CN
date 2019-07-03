---
title: 'tiIndicator: updateTiIndicators'
description: 在一个请求中 (而不是多个请求) 更新多个威胁情报 (TI) 指示器。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d44ab406998cff70ad6292598d31d6e108f63d4f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35451372"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="79320-103">tiIndicator: updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="79320-103">tiIndicator: updateTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79320-104">在一个请求中 (而不是多个请求) 更新多个威胁情报 (TI) 指示器。</span><span class="sxs-lookup"><span data-stu-id="79320-104">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="79320-105">权限</span><span class="sxs-lookup"><span data-stu-id="79320-105">Permissions</span></span>

<span data-ttu-id="79320-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79320-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="79320-108">Permission type</span></span>   | <span data-ttu-id="79320-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79320-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79320-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79320-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="79320-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="79320-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="79320-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79320-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79320-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="79320-113">Not supported.</span></span> |
| <span data-ttu-id="79320-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="79320-114">Application</span></span>                            | <span data-ttu-id="79320-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="79320-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="79320-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79320-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="79320-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="79320-117">Request headers</span></span>

| <span data-ttu-id="79320-118">名称</span><span class="sxs-lookup"><span data-stu-id="79320-118">Name</span></span>          | <span data-ttu-id="79320-119">说明</span><span class="sxs-lookup"><span data-stu-id="79320-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="79320-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="79320-120">Authorization</span></span> | <span data-ttu-id="79320-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="79320-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="79320-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="79320-122">Request body</span></span>

<span data-ttu-id="79320-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="79320-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="79320-124">有关可更新的属性的详细信息, 请参阅[更新 tiIndicator](tiindicator-update.md)。</span><span class="sxs-lookup"><span data-stu-id="79320-124">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span>

| <span data-ttu-id="79320-125">参数</span><span class="sxs-lookup"><span data-stu-id="79320-125">Parameter</span></span>    | <span data-ttu-id="79320-126">类型</span><span class="sxs-lookup"><span data-stu-id="79320-126">Type</span></span>        | <span data-ttu-id="79320-127">说明</span><span class="sxs-lookup"><span data-stu-id="79320-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79320-128">值</span><span class="sxs-lookup"><span data-stu-id="79320-128">value</span></span>|<span data-ttu-id="79320-129">tiIndicator 集合</span><span class="sxs-lookup"><span data-stu-id="79320-129">tiIndicator collection</span></span>| <span data-ttu-id="79320-130">要更新的**tiIndicators**的集合。</span><span class="sxs-lookup"><span data-stu-id="79320-130">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="79320-131">每个实体都必须具有要更新的**id**和其他可编辑属性。</span><span class="sxs-lookup"><span data-stu-id="79320-131">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="79320-132">响应</span><span class="sxs-lookup"><span data-stu-id="79320-132">Response</span></span>

<span data-ttu-id="79320-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[tiIndicator](../resources/tiindicator.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="79320-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79320-134">示例</span><span class="sxs-lookup"><span data-stu-id="79320-134">Examples</span></span>

<span data-ttu-id="79320-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="79320-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="79320-136">请求</span><span class="sxs-lookup"><span data-stu-id="79320-136">Request</span></span>

<span data-ttu-id="79320-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79320-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79320-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="79320-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="79320-139">C#</span><span class="sxs-lookup"><span data-stu-id="79320-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79320-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="79320-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79320-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="79320-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="79320-142">响应</span><span class="sxs-lookup"><span data-stu-id="79320-142">Response</span></span>

<span data-ttu-id="79320-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="79320-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="79320-144">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79320-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="79320-145">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="79320-145">All the properties will be returned from an actual call.</span></span>

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
