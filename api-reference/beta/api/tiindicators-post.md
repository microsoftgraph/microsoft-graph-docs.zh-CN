---
title: 创建威胁情报指标
description: 创建新的 tiIndicator。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 440515a45b4c530f32dd20fe29497e338b54a6bf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335226"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="49698-103">创建威胁情报指标</span><span class="sxs-lookup"><span data-stu-id="49698-103">Create threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49698-104">创建新的[tiIndicator](../resources/tiindicator.md)对象。</span><span class="sxs-lookup"><span data-stu-id="49698-104">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="49698-105">权限</span><span class="sxs-lookup"><span data-stu-id="49698-105">Permissions</span></span>

<span data-ttu-id="49698-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49698-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="49698-108">Permission type</span></span>                        | <span data-ttu-id="49698-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49698-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="49698-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49698-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="49698-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="49698-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="49698-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49698-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49698-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="49698-113">Not supported.</span></span> |
| <span data-ttu-id="49698-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="49698-114">Application</span></span>                            | <span data-ttu-id="49698-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="49698-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="49698-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49698-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="49698-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="49698-117">Request headers</span></span>

| <span data-ttu-id="49698-118">名称</span><span class="sxs-lookup"><span data-stu-id="49698-118">Name</span></span>          | <span data-ttu-id="49698-119">说明</span><span class="sxs-lookup"><span data-stu-id="49698-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="49698-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="49698-120">Authorization</span></span> | <span data-ttu-id="49698-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="49698-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="49698-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="49698-122">Request body</span></span>

<span data-ttu-id="49698-123">在请求正文中, 提供包含至少一个[电子邮件](../resources/tiindicator.md#indicator-observables---email)、[文件](../resources/tiindicator.md#indicator-observables---file)或[网络](../resources/tiindicator.md#indicator-observables---network)可观测对象的[tiIndicator](../resources/tiindicator.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49698-123">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable.</span></span>

## <a name="response"></a><span data-ttu-id="49698-124">响应</span><span class="sxs-lookup"><span data-stu-id="49698-124">Response</span></span>

<span data-ttu-id="49698-125">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[tiIndicator](../resources/tiindicator.md)对象。</span><span class="sxs-lookup"><span data-stu-id="49698-125">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49698-126">示例</span><span class="sxs-lookup"><span data-stu-id="49698-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49698-127">请求</span><span class="sxs-lookup"><span data-stu-id="49698-127">Request</span></span>

<span data-ttu-id="49698-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49698-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="49698-129">响应</span><span class="sxs-lookup"><span data-stu-id="49698-129">Response</span></span>

<span data-ttu-id="49698-130">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="49698-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="49698-131">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="49698-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49698-132">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49698-132">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
