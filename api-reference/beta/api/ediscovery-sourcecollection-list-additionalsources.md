---
title: 列出 additionalSources
description: 获取与源集合关联的其他 DataSource 对象的列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5f9c08fe286be1dd983fa81a4b9ee9b61563b503
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446003"
---
# <a name="list-additionalsources"></a><span data-ttu-id="43e3a-103">列出 additionalSources</span><span class="sxs-lookup"><span data-stu-id="43e3a-103">List additionalSources</span></span>

<span data-ttu-id="43e3a-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="43e3a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43e3a-105">获取与源集合关联的其他 [DataSource](../resources/ediscovery-datasource.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="43e3a-105">Get a list of additional [dataSource](../resources/ediscovery-datasource.md) objects associated with a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="43e3a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="43e3a-106">Permissions</span></span>

<span data-ttu-id="43e3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43e3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43e3a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="43e3a-109">Permission type</span></span>|<span data-ttu-id="43e3a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43e3a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43e3a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43e3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="43e3a-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43e3a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="43e3a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43e3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43e3a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="43e3a-114">Not supported.</span></span>|
|<span data-ttu-id="43e3a-115">Application</span><span class="sxs-lookup"><span data-stu-id="43e3a-115">Application</span></span>|<span data-ttu-id="43e3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="43e3a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43e3a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43e3a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43e3a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="43e3a-118">Optional query parameters</span></span>

<span data-ttu-id="43e3a-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="43e3a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="43e3a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="43e3a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="43e3a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="43e3a-121">Request headers</span></span>

|<span data-ttu-id="43e3a-122">名称</span><span class="sxs-lookup"><span data-stu-id="43e3a-122">Name</span></span>|<span data-ttu-id="43e3a-123">说明</span><span class="sxs-lookup"><span data-stu-id="43e3a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="43e3a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="43e3a-124">Authorization</span></span>|<span data-ttu-id="43e3a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43e3a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="43e3a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="43e3a-127">Request body</span></span>

<span data-ttu-id="43e3a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="43e3a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43e3a-129">响应</span><span class="sxs-lookup"><span data-stu-id="43e3a-129">Response</span></span>

<span data-ttu-id="43e3a-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="43e3a-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43e3a-131">示例</span><span class="sxs-lookup"><span data-stu-id="43e3a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43e3a-132">请求</span><span class="sxs-lookup"><span data-stu-id="43e3a-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

### <a name="response"></a><span data-ttu-id="43e3a-133">响应</span><span class="sxs-lookup"><span data-stu-id="43e3a-133">Response</span></span>

<span data-ttu-id="43e3a-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="43e3a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.dataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.dataSource",
      "id": "0fb67fc5-7fc5-0fb6-c57f-b60fc57fb60f",
      "displayName": "String",
      "createdDateTime": "String (timestamp)",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ]
}
```
