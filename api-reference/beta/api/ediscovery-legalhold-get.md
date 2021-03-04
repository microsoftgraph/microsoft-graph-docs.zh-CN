---
title: 获取 legalHold
description: 读取 legalHold 对象的属性和关系。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f2d276a85a6f95b845acef48fc3e823cb08be79b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446043"
---
# <a name="get-legalhold"></a><span data-ttu-id="f9003-103">获取 legalHold</span><span class="sxs-lookup"><span data-stu-id="f9003-103">Get legalHold</span></span>

<span data-ttu-id="f9003-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f9003-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9003-105">读取 [legalHold 对象的属性和](../resources/ediscovery-legalhold.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="f9003-105">Read the properties and relationships of a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9003-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f9003-106">Permissions</span></span>

<span data-ttu-id="f9003-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9003-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9003-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9003-109">Permission type</span></span>|<span data-ttu-id="f9003-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9003-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9003-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9003-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f9003-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9003-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f9003-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9003-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9003-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9003-114">Not supported.</span></span>|
|<span data-ttu-id="f9003-115">Application</span><span class="sxs-lookup"><span data-stu-id="f9003-115">Application</span></span>|<span data-ttu-id="f9003-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9003-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9003-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9003-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9003-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f9003-118">Optional query parameters</span></span>

<span data-ttu-id="f9003-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f9003-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f9003-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f9003-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9003-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9003-121">Request headers</span></span>

|<span data-ttu-id="f9003-122">名称</span><span class="sxs-lookup"><span data-stu-id="f9003-122">Name</span></span>|<span data-ttu-id="f9003-123">说明</span><span class="sxs-lookup"><span data-stu-id="f9003-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f9003-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9003-124">Authorization</span></span>|<span data-ttu-id="f9003-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9003-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9003-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9003-127">Request body</span></span>

<span data-ttu-id="f9003-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9003-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9003-129">响应</span><span class="sxs-lookup"><span data-stu-id="f9003-129">Response</span></span>

<span data-ttu-id="f9003-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9003-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9003-131">示例</span><span class="sxs-lookup"><span data-stu-id="f9003-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9003-132">请求</span><span class="sxs-lookup"><span data-stu-id="f9003-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_legalhold"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

### <a name="response"></a><span data-ttu-id="f9003-133">响应</span><span class="sxs-lookup"><span data-stu-id="f9003-133">Response</span></span>

<span data-ttu-id="f9003-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f9003-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.legalHold"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.ediscovery.legalHold",
    "id": "700cd868-d868-700c-68d8-0c7068d80c70",
    "description": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "isEnabled": "Boolean",
    "status": "String",
    "contentQuery": "String",
    "errors": [
      "String"
    ],
    "displayName": "String",
    "createdDateTime": "String (timestamp)"
  }
}
```
