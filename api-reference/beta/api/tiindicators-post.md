---
title: 创建威胁情报指标
description: 创建新的 tiIndicator。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 5de9e8b01fa02f02fbfa8248a7f307360cd1c6ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076496"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="9009f-103">创建威胁情报指标</span><span class="sxs-lookup"><span data-stu-id="9009f-103">Create threat intelligence indicator</span></span>

<span data-ttu-id="9009f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9009f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9009f-105">创建新的 [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9009f-105">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9009f-106">权限</span><span class="sxs-lookup"><span data-stu-id="9009f-106">Permissions</span></span>

<span data-ttu-id="9009f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9009f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9009f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9009f-109">Permission type</span></span>                        | <span data-ttu-id="9009f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9009f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9009f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9009f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9009f-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9009f-112">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="9009f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9009f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9009f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9009f-114">Not supported.</span></span> |
| <span data-ttu-id="9009f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9009f-115">Application</span></span>                            | <span data-ttu-id="9009f-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9009f-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="9009f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9009f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="9009f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9009f-118">Request headers</span></span>

| <span data-ttu-id="9009f-119">名称</span><span class="sxs-lookup"><span data-stu-id="9009f-119">Name</span></span>          | <span data-ttu-id="9009f-120">说明</span><span class="sxs-lookup"><span data-stu-id="9009f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9009f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9009f-121">Authorization</span></span> | <span data-ttu-id="9009f-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9009f-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9009f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9009f-123">Request body</span></span>

<span data-ttu-id="9009f-124">在请求正文中，提供包含至少一个[电子邮件](../resources/tiindicator.md#indicator-observables---email)、[文件](../resources/tiindicator.md#indicator-observables---file)或[网络](../resources/tiindicator.md#indicator-observables---network)可观测对象的[tiIndicator](../resources/tiindicator.md)对象的 JSON 表示形式，并提供以下必需字段： `action` 、、、、 `description` `expirationDateTime` `targetProduct` `threatType` 、 `tlpLevel` 。</span><span class="sxs-lookup"><span data-stu-id="9009f-124">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span> 

## <a name="response"></a><span data-ttu-id="9009f-125">响应</span><span class="sxs-lookup"><span data-stu-id="9009f-125">Response</span></span>

<span data-ttu-id="9009f-126">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9009f-126">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9009f-127">示例</span><span class="sxs-lookup"><span data-stu-id="9009f-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9009f-128">请求</span><span class="sxs-lookup"><span data-stu-id="9009f-128">Request</span></span>

<span data-ttu-id="9009f-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9009f-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9009f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9009f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tiindicator_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators
Content-type: application/json

{
  "action": "alert",
  "activityGroupNames": [],
  "confidence": 0,
  "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
  "expirationDateTime": "2019-03-01T21:43:37.5031462+00:00",
  "externalId": "Test--8586509942679764298MS501",
  "fileHashType": "sha256",
  "fileHashValue": "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
  "killChain": [],
  "malwareFamilyNames": [],
  "severity": 0,
  "tags": [],
  "targetProduct": "Azure Sentinel",
  "threatType": "WatchList",
  "tlpLevel": "green"
}
```
# <a name="c"></a>[<span data-ttu-id="9009f-131">C#</span><span class="sxs-lookup"><span data-stu-id="9009f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tiindicator-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9009f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9009f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tiindicator-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9009f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9009f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tiindicator-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9009f-134">响应</span><span class="sxs-lookup"><span data-stu-id="9009f-134">Response</span></span>

<span data-ttu-id="9009f-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9009f-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9009f-136">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9009f-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9009f-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9009f-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXX",
    "action": "alert",
    "additionalInformation": null,
    "activityGroupNames": [],
    "confidence": 0,
    "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


