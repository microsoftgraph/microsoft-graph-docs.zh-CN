---
title: tiIndicator：updateTiIndicators
description: 在一个 (（) 请求）中更新多个威胁情报和 TI) 指示器。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 4c594c9ba75ea0ee1cd1fcb8390d4b9ff738d48c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050771"
---
# <a name="tiindicator-updatetiindicators"></a><span data-ttu-id="000bb-103">tiIndicator：updateTiIndicators</span><span class="sxs-lookup"><span data-stu-id="000bb-103">tiIndicator: updateTiIndicators</span></span>

<span data-ttu-id="000bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="000bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="000bb-105">在一个 (（) 请求）中更新多个威胁情报和 TI) 指示器。</span><span class="sxs-lookup"><span data-stu-id="000bb-105">Update multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="000bb-106">权限</span><span class="sxs-lookup"><span data-stu-id="000bb-106">Permissions</span></span>

<span data-ttu-id="000bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="000bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="000bb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="000bb-109">Permission type</span></span>   | <span data-ttu-id="000bb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="000bb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="000bb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="000bb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="000bb-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="000bb-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="000bb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="000bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="000bb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="000bb-114">Not supported.</span></span> |
| <span data-ttu-id="000bb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="000bb-115">Application</span></span>                            | <span data-ttu-id="000bb-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="000bb-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="000bb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="000bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/updateTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="000bb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="000bb-118">Request headers</span></span>

| <span data-ttu-id="000bb-119">名称</span><span class="sxs-lookup"><span data-stu-id="000bb-119">Name</span></span>          | <span data-ttu-id="000bb-120">说明</span><span class="sxs-lookup"><span data-stu-id="000bb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="000bb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="000bb-121">Authorization</span></span> | <span data-ttu-id="000bb-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="000bb-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="000bb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="000bb-123">Request body</span></span>

<span data-ttu-id="000bb-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="000bb-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="000bb-125">有关可更新的属性的详细信息，请参阅[更新 tiIndicator。](tiindicator-update.md)</span><span class="sxs-lookup"><span data-stu-id="000bb-125">For details about properties that can be updated, see [update tiIndicator](tiindicator-update.md).</span></span> <span data-ttu-id="000bb-126">每个 tiIndicator 的必填字段为 `id` `expirationDateTime` `targetProduct` ：、、。</span><span class="sxs-lookup"><span data-stu-id="000bb-126">Required fields for each tiIndicator are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="000bb-127">参数</span><span class="sxs-lookup"><span data-stu-id="000bb-127">Parameter</span></span>    | <span data-ttu-id="000bb-128">类型</span><span class="sxs-lookup"><span data-stu-id="000bb-128">Type</span></span>        | <span data-ttu-id="000bb-129">说明</span><span class="sxs-lookup"><span data-stu-id="000bb-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="000bb-130">值</span><span class="sxs-lookup"><span data-stu-id="000bb-130">value</span></span>|<span data-ttu-id="000bb-131">tiIndicator 集合</span><span class="sxs-lookup"><span data-stu-id="000bb-131">tiIndicator collection</span></span>| <span data-ttu-id="000bb-132">要 **更新的 tiIndicator** 集合。</span><span class="sxs-lookup"><span data-stu-id="000bb-132">Collection of **tiIndicators** to update.</span></span> <span data-ttu-id="000bb-133">每个实体必须具有 **id** 和其他可编辑属性以进行更新。</span><span class="sxs-lookup"><span data-stu-id="000bb-133">Each entity must have **id** and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="000bb-134">响应</span><span class="sxs-lookup"><span data-stu-id="000bb-134">Response</span></span>

<span data-ttu-id="000bb-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tiIndicator](../resources/tiindicator.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="000bb-135">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="000bb-136">如果出现错误，此方法将返回 响应 `206 Partial Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="000bb-136">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="000bb-137">有关详细信息 [，](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) 请参阅错误。</span><span class="sxs-lookup"><span data-stu-id="000bb-137">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="000bb-138">示例</span><span class="sxs-lookup"><span data-stu-id="000bb-138">Examples</span></span>

<span data-ttu-id="000bb-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="000bb-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="000bb-140">请求</span><span class="sxs-lookup"><span data-stu-id="000bb-140">Request</span></span>

<span data-ttu-id="000bb-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="000bb-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="000bb-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="000bb-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="000bb-143">C#</span><span class="sxs-lookup"><span data-stu-id="000bb-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-updatetiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="000bb-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="000bb-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-updatetiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="000bb-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="000bb-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-updatetiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="000bb-146">Java</span><span class="sxs-lookup"><span data-stu-id="000bb-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-updatetiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="000bb-147">响应</span><span class="sxs-lookup"><span data-stu-id="000bb-147">Response</span></span>

<span data-ttu-id="000bb-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="000bb-148">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="000bb-149">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="000bb-149">The response object shown here might be shortened for readability.</span></span>

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


