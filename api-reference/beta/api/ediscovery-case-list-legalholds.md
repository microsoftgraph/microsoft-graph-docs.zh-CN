---
title: 列出 legalHolds
description: 从 legalHolds 导航属性获取 legalHold 资源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 15798da638a43f6a126c1aef6bd9e88c1015e67a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446097"
---
# <a name="list-legalholds"></a><span data-ttu-id="700b5-103">列出 legalHolds</span><span class="sxs-lookup"><span data-stu-id="700b5-103">List legalHolds</span></span>

<span data-ttu-id="700b5-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="700b5-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="700b5-105">获取应用于案例的[legalHolds。](../resources/ediscovery-legalhold.md)</span><span class="sxs-lookup"><span data-stu-id="700b5-105">Get the [legalHolds](../resources/ediscovery-legalhold.md) that are applied to a case.</span></span>

## <a name="permissions"></a><span data-ttu-id="700b5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="700b5-106">Permissions</span></span>

<span data-ttu-id="700b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="700b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="700b5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="700b5-109">Permission type</span></span>|<span data-ttu-id="700b5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="700b5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="700b5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="700b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="700b5-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="700b5-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="700b5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="700b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="700b5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="700b5-114">Not supported.</span></span>|
|<span data-ttu-id="700b5-115">Application</span><span class="sxs-lookup"><span data-stu-id="700b5-115">Application</span></span>|<span data-ttu-id="700b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="700b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="700b5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="700b5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds
```

## <a name="optional-query-parameters"></a><span data-ttu-id="700b5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="700b5-118">Optional query parameters</span></span>

<span data-ttu-id="700b5-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="700b5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="700b5-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="700b5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="700b5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="700b5-121">Request headers</span></span>

|<span data-ttu-id="700b5-122">名称</span><span class="sxs-lookup"><span data-stu-id="700b5-122">Name</span></span>|<span data-ttu-id="700b5-123">说明</span><span class="sxs-lookup"><span data-stu-id="700b5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="700b5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="700b5-124">Authorization</span></span>|<span data-ttu-id="700b5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="700b5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="700b5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="700b5-127">Request body</span></span>

<span data-ttu-id="700b5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="700b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="700b5-129">响应</span><span class="sxs-lookup"><span data-stu-id="700b5-129">Response</span></span>

<span data-ttu-id="700b5-130">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [legalHold](../resources/ediscovery-legalhold.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="700b5-130">If successful, this method returns a `200 OK` response code and a collection of [legalHold](../resources/ediscovery-legalhold.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="700b5-131">示例</span><span class="sxs-lookup"><span data-stu-id="700b5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="700b5-132">请求</span><span class="sxs-lookup"><span data-stu-id="700b5-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_legalhold"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds
```

### <a name="response"></a><span data-ttu-id="700b5-133">响应</span><span class="sxs-lookup"><span data-stu-id="700b5-133">Response</span></span>

<span data-ttu-id="700b5-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="700b5-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.legalHold)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```
