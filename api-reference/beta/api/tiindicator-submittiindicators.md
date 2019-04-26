---
title: 'tiIndicator: submitTiIndicators'
description: 在一个请求中 (而不是多个请求) 上载多个威胁情报 (TI) 指示器。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b16f3da7d2c0183da5b7e06cef3bce450bbe0068
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335256"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="724bd-103">tiIndicator: submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="724bd-103">tiIndicator: submitTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="724bd-104">在一个请求中 (而不是多个请求) 上载多个威胁情报 (TI) 指示器。</span><span class="sxs-lookup"><span data-stu-id="724bd-104">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="724bd-105">权限</span><span class="sxs-lookup"><span data-stu-id="724bd-105">Permissions</span></span>

<span data-ttu-id="724bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="724bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="724bd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="724bd-108">Permission type</span></span> | <span data-ttu-id="724bd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="724bd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="724bd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="724bd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="724bd-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="724bd-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="724bd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="724bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="724bd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="724bd-113">Not supported.</span></span> |
| <span data-ttu-id="724bd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="724bd-114">Application</span></span>                            | <span data-ttu-id="724bd-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="724bd-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="724bd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="724bd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="724bd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="724bd-117">Request headers</span></span>

| <span data-ttu-id="724bd-118">名称</span><span class="sxs-lookup"><span data-stu-id="724bd-118">Name</span></span>          | <span data-ttu-id="724bd-119">说明</span><span class="sxs-lookup"><span data-stu-id="724bd-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="724bd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="724bd-120">Authorization</span></span> | <span data-ttu-id="724bd-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="724bd-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="724bd-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="724bd-122">Request body</span></span>

<span data-ttu-id="724bd-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="724bd-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="724bd-124">参数</span><span class="sxs-lookup"><span data-stu-id="724bd-124">Parameter</span></span>    | <span data-ttu-id="724bd-125">类型</span><span class="sxs-lookup"><span data-stu-id="724bd-125">Type</span></span>        | <span data-ttu-id="724bd-126">说明</span><span class="sxs-lookup"><span data-stu-id="724bd-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="724bd-127">值</span><span class="sxs-lookup"><span data-stu-id="724bd-127">value</span></span>|<span data-ttu-id="724bd-128">tiIndicator 集合</span><span class="sxs-lookup"><span data-stu-id="724bd-128">tiIndicator collection</span></span>| <span data-ttu-id="724bd-129">要创建的**tiIndicators**的 JSON 集合。</span><span class="sxs-lookup"><span data-stu-id="724bd-129">JSON collection of **tiIndicators** to be created.</span></span> |

## <a name="response"></a><span data-ttu-id="724bd-130">响应</span><span class="sxs-lookup"><span data-stu-id="724bd-130">Response</span></span>

<span data-ttu-id="724bd-131">如果成功, 此方法在`200, OK`响应正文中返回响应代码和[tiIndicator](../resources/tiindicator.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="724bd-131">If successful, this method returns `200, OK` response code and a [tiIndicator](../resources/tiindicator.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="724bd-132">示例</span><span class="sxs-lookup"><span data-stu-id="724bd-132">Examples</span></span>

<span data-ttu-id="724bd-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="724bd-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="724bd-134">请求</span><span class="sxs-lookup"><span data-stu-id="724bd-134">Request</span></span>

<span data-ttu-id="724bd-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="724bd-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="724bd-136">响应</span><span class="sxs-lookup"><span data-stu-id="724bd-136">Response</span></span>

<span data-ttu-id="724bd-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="724bd-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="724bd-138">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="724bd-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="724bd-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="724bd-139">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
