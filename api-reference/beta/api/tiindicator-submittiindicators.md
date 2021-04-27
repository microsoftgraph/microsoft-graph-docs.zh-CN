---
title: tiIndicator：submitTiIndicators
description: Upload一个 (请求) 多个请求（而不是多个请求）中使用多个威胁情报和 TI 指示器。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: ed4ccd5adf087ecf8be69d8d192ae180ec685090
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050778"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="80081-103">tiIndicator：submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="80081-103">tiIndicator: submitTiIndicators</span></span>

<span data-ttu-id="80081-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80081-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80081-105">Upload一个 (请求) 多个请求（而不是多个请求）中使用多个威胁情报和 TI 指示器。</span><span class="sxs-lookup"><span data-stu-id="80081-105">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="80081-106">权限</span><span class="sxs-lookup"><span data-stu-id="80081-106">Permissions</span></span>

<span data-ttu-id="80081-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80081-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80081-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80081-109">Permission type</span></span> | <span data-ttu-id="80081-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80081-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="80081-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80081-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="80081-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="80081-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="80081-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80081-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80081-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80081-114">Not supported.</span></span> |
| <span data-ttu-id="80081-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80081-115">Application</span></span>                            | <span data-ttu-id="80081-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="80081-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="80081-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80081-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="80081-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="80081-118">Request headers</span></span>

| <span data-ttu-id="80081-119">名称</span><span class="sxs-lookup"><span data-stu-id="80081-119">Name</span></span>          | <span data-ttu-id="80081-120">说明</span><span class="sxs-lookup"><span data-stu-id="80081-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="80081-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80081-121">Authorization</span></span> | <span data-ttu-id="80081-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="80081-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="80081-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="80081-123">Request body</span></span>

<span data-ttu-id="80081-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="80081-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="80081-125">参数</span><span class="sxs-lookup"><span data-stu-id="80081-125">Parameter</span></span>    | <span data-ttu-id="80081-126">类型</span><span class="sxs-lookup"><span data-stu-id="80081-126">Type</span></span>        | <span data-ttu-id="80081-127">说明</span><span class="sxs-lookup"><span data-stu-id="80081-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="80081-128">值</span><span class="sxs-lookup"><span data-stu-id="80081-128">value</span></span>|<span data-ttu-id="80081-129">tiIndicator 集合</span><span class="sxs-lookup"><span data-stu-id="80081-129">tiIndicator collection</span></span>| <span data-ttu-id="80081-130">要创建的 **tiIndicator 的** JSON 集合。</span><span class="sxs-lookup"><span data-stu-id="80081-130">JSON collection of **tiIndicators** to be created.</span></span> |

<span data-ttu-id="80081-131">对于每个 tiIndicator，提供包含至少一个电子邮件、文件或网络可观测的[tiIndicator](../resources/tiindicator.md)对象的[](../resources/tiindicator.md#indicator-observables---file)JSON[](../resources/tiindicator.md#indicator-observables---network)表示形式，以及以下必填字段[](../resources/tiindicator.md#indicator-observables---email) `action` `description` `expirationDateTime` `targetProduct` `threatType` `tlpLevel` ：、。</span><span class="sxs-lookup"><span data-stu-id="80081-131">For each tiIndicator, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span>

## <a name="response"></a><span data-ttu-id="80081-132">响应</span><span class="sxs-lookup"><span data-stu-id="80081-132">Response</span></span>

<span data-ttu-id="80081-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tiIndicator](../resources/tiindicator.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="80081-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="80081-134">如果出现错误，此方法将返回 响应 `206 Partial Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="80081-134">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="80081-135">有关详细信息 [，](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) 请参阅错误。</span><span class="sxs-lookup"><span data-stu-id="80081-135">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="80081-136">示例</span><span class="sxs-lookup"><span data-stu-id="80081-136">Examples</span></span>

<span data-ttu-id="80081-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="80081-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="80081-138">请求</span><span class="sxs-lookup"><span data-stu-id="80081-138">Request</span></span>

<span data-ttu-id="80081-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80081-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80081-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="80081-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_submittiindicators",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators
Content-Type: application/json

{
  "value": [
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1668987+00:00",
      "externalId": "Test--8586509942423126760MS164-0",
      "fileHashType": "sha256",
      "fileHashValue": "b555c45c5b1b01304217e72118d6ca1b14b7013644a078273cea27bbdc1cf9d6",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    },
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1748779+00:00",
      "externalId": "Test--8586509942423126760MS164-1",
      "fileHashType": "sha256",
      "fileHashValue": "1796b433950990b28d6a22456c9d2b58ced1bdfcdf5f16f7e39d6b9bdca4213b",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="80081-141">C#</span><span class="sxs-lookup"><span data-stu-id="80081-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-submittiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80081-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80081-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-submittiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80081-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80081-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-submittiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80081-144">Java</span><span class="sxs-lookup"><span data-stu-id="80081-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-submittiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80081-145">响应</span><span class="sxs-lookup"><span data-stu-id="80081-145">Response</span></span>

<span data-ttu-id="80081-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80081-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="80081-147">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="80081-147">The response object shown here might be shortened for readability.</span></span>

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
      "azureTenantId": "XXXXXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": null,
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
  "description": "tiIndicator: submitTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


