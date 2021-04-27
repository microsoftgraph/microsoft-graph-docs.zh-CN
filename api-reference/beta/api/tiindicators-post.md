---
title: 创建威胁情报指示器
description: 创建新的 tiIndicator。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 14620ff345c5d74075548b17e26bc7923f942da6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050757"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="b1bf1-103">创建威胁情报指示器</span><span class="sxs-lookup"><span data-stu-id="b1bf1-103">Create threat intelligence indicator</span></span>

<span data-ttu-id="b1bf1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1bf1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1bf1-105">创建新的 [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1bf1-105">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1bf1-106">权限</span><span class="sxs-lookup"><span data-stu-id="b1bf1-106">Permissions</span></span>

<span data-ttu-id="b1bf1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1bf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1bf1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1bf1-109">Permission type</span></span>                        | <span data-ttu-id="b1bf1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1bf1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b1bf1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1bf1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1bf1-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="b1bf1-112">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="b1bf1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1bf1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1bf1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1bf1-114">Not supported.</span></span> |
| <span data-ttu-id="b1bf1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1bf1-115">Application</span></span>                            | <span data-ttu-id="b1bf1-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="b1bf1-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1bf1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1bf1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="b1bf1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1bf1-118">Request headers</span></span>

| <span data-ttu-id="b1bf1-119">名称</span><span class="sxs-lookup"><span data-stu-id="b1bf1-119">Name</span></span>          | <span data-ttu-id="b1bf1-120">说明</span><span class="sxs-lookup"><span data-stu-id="b1bf1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b1bf1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1bf1-121">Authorization</span></span> | <span data-ttu-id="b1bf1-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b1bf1-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1bf1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1bf1-123">Request body</span></span>

<span data-ttu-id="b1bf1-124">在请求正文中，提供[tiIndicator](../resources/tiindicator.md)对象的 JSON 表示形式，该对象包含至少一[](../resources/tiindicator.md#indicator-observables---file)个[电子邮件](../resources/tiindicator.md#indicator-observables---email)、[](../resources/tiindicator.md#indicator-observables---network)文件或网络可观测对象，以及以下必填 `action` 字段 `description` `expirationDateTime` `targetProduct` `threatType` `tlpLevel` ：、。</span><span class="sxs-lookup"><span data-stu-id="b1bf1-124">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span> 

## <a name="response"></a><span data-ttu-id="b1bf1-125">响应</span><span class="sxs-lookup"><span data-stu-id="b1bf1-125">Response</span></span>

<span data-ttu-id="b1bf1-126">如果成功，此方法在响应正文中返回 响应代码 `201 Created` 和 [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1bf1-126">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1bf1-127">示例</span><span class="sxs-lookup"><span data-stu-id="b1bf1-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1bf1-128">请求</span><span class="sxs-lookup"><span data-stu-id="b1bf1-128">Request</span></span>

<span data-ttu-id="b1bf1-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b1bf1-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1bf1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1bf1-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b1bf1-131">C#</span><span class="sxs-lookup"><span data-stu-id="b1bf1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tiindicator-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1bf1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1bf1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tiindicator-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1bf1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1bf1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tiindicator-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1bf1-134">Java</span><span class="sxs-lookup"><span data-stu-id="b1bf1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tiindicator-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b1bf1-135">响应</span><span class="sxs-lookup"><span data-stu-id="b1bf1-135">Response</span></span>

<span data-ttu-id="b1bf1-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b1bf1-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b1bf1-137">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b1bf1-137">The response object shown here might be shortened for readability.</span></span>

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


