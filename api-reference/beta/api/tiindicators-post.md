---
title: 创建威胁情报指标
description: 创建新的 tiIndicator。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: be0e89fd353cbe54a9f3d9d6dbb3108a1b4da8db
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981468"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="874b0-103">创建威胁情报指标</span><span class="sxs-lookup"><span data-stu-id="874b0-103">Create threat intelligence indicator</span></span>

<span data-ttu-id="874b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="874b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="874b0-105">创建新的 [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="874b0-105">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="874b0-106">权限</span><span class="sxs-lookup"><span data-stu-id="874b0-106">Permissions</span></span>

<span data-ttu-id="874b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="874b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="874b0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="874b0-109">Permission type</span></span>                        | <span data-ttu-id="874b0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="874b0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="874b0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="874b0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="874b0-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="874b0-112">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="874b0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="874b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="874b0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="874b0-114">Not supported.</span></span> |
| <span data-ttu-id="874b0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="874b0-115">Application</span></span>                            | <span data-ttu-id="874b0-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="874b0-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="874b0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="874b0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="874b0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="874b0-118">Request headers</span></span>

| <span data-ttu-id="874b0-119">名称</span><span class="sxs-lookup"><span data-stu-id="874b0-119">Name</span></span>          | <span data-ttu-id="874b0-120">说明</span><span class="sxs-lookup"><span data-stu-id="874b0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="874b0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="874b0-121">Authorization</span></span> | <span data-ttu-id="874b0-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="874b0-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="874b0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="874b0-123">Request body</span></span>

<span data-ttu-id="874b0-124">在请求正文中，提供包含至少一个[电子邮件](../resources/tiindicator.md#indicator-observables---email)、[文件](../resources/tiindicator.md#indicator-observables---file)或[网络](../resources/tiindicator.md#indicator-observables---network)可观测对象的[tiIndicator](../resources/tiindicator.md)对象的 JSON 表示形式，并提供以下必需字段： `action` 、、、、 `description` `expirationDateTime` `targetProduct` `threatType` 、 `tlpLevel` 。</span><span class="sxs-lookup"><span data-stu-id="874b0-124">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span> 

## <a name="response"></a><span data-ttu-id="874b0-125">响应</span><span class="sxs-lookup"><span data-stu-id="874b0-125">Response</span></span>

<span data-ttu-id="874b0-126">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="874b0-126">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="874b0-127">示例</span><span class="sxs-lookup"><span data-stu-id="874b0-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="874b0-128">请求</span><span class="sxs-lookup"><span data-stu-id="874b0-128">Request</span></span>

<span data-ttu-id="874b0-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="874b0-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="874b0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="874b0-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="874b0-131">C#</span><span class="sxs-lookup"><span data-stu-id="874b0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tiindicator-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="874b0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="874b0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tiindicator-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="874b0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="874b0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tiindicator-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="874b0-134">Java</span><span class="sxs-lookup"><span data-stu-id="874b0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tiindicator-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="874b0-135">响应</span><span class="sxs-lookup"><span data-stu-id="874b0-135">Response</span></span>

<span data-ttu-id="874b0-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="874b0-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="874b0-137">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="874b0-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="874b0-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="874b0-138">All the properties will be returned from an actual call.</span></span>

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


