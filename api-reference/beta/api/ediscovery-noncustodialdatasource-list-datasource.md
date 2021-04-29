---
title: 列出 dataSource
description: 从 dataSource 导航属性获取 dataSource 资源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 60cec935db8e451efa6e855c56b71eb026ca4f99
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080736"
---
# <a name="list-datasource"></a><span data-ttu-id="6cdc3-103">列出 dataSource</span><span class="sxs-lookup"><span data-stu-id="6cdc3-103">List dataSource</span></span>

<span data-ttu-id="6cdc3-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6cdc3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cdc3-105">获取与非外部数据源关联的 dataSources 列表。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-105">Get the list of dataSources associated with a non-custodial data source.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cdc3-106">权限</span><span class="sxs-lookup"><span data-stu-id="6cdc3-106">Permissions</span></span>

<span data-ttu-id="6cdc3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cdc3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cdc3-109">Permission type</span></span>|<span data-ttu-id="6cdc3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cdc3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cdc3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cdc3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6cdc3-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cdc3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="6cdc3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cdc3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cdc3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-114">Not supported.</span></span>|
|<span data-ttu-id="6cdc3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cdc3-115">Application</span></span>|<span data-ttu-id="6cdc3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cdc3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cdc3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}/dataSource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cdc3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6cdc3-118">Optional query parameters</span></span>

<span data-ttu-id="6cdc3-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6cdc3-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cdc3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cdc3-121">Request headers</span></span>

|<span data-ttu-id="6cdc3-122">名称</span><span class="sxs-lookup"><span data-stu-id="6cdc3-122">Name</span></span>|<span data-ttu-id="6cdc3-123">说明</span><span class="sxs-lookup"><span data-stu-id="6cdc3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6cdc3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cdc3-124">Authorization</span></span>|<span data-ttu-id="6cdc3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cdc3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cdc3-127">Request body</span></span>

<span data-ttu-id="6cdc3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cdc3-129">响应</span><span class="sxs-lookup"><span data-stu-id="6cdc3-129">Response</span></span>

<span data-ttu-id="6cdc3-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [dataSource](../resources/ediscovery-datasource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-130">If successful, this method returns a `200 OK` response code and a collection of [dataSource](../resources/ediscovery-datasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6cdc3-131">示例</span><span class="sxs-lookup"><span data-stu-id="6cdc3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6cdc3-132">请求</span><span class="sxs-lookup"><span data-stu-id="6cdc3-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_datasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/datasource
```

### <a name="response"></a><span data-ttu-id="6cdc3-133">响应</span><span class="sxs-lookup"><span data-stu-id="6cdc3-133">Response</span></span>

<span data-ttu-id="6cdc3-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6cdc3-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
        "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources('8e402dd7f3c94a3abc086e5d07db1c6d')/dataSource/$entity",
        "@odata.type": "#microsoft.graph.ediscovery.userSource",
        "displayName": "Adele Vance",
        "createdDateTime": "2021-02-17T19:41:22.5902664Z",
        "id": "8e402dd7f3c94a3abc086e5d07db1c6d",
        "email": "AdeleV@contoso.com",
        "includedSources": "mailbox",
        "createdBy": {
            "user": {
                "id": "ediscovery admin",
                "displayName": "c1db6f13-332a-4d84-b111-914383ff9fc9"
            }
        }
      }
  ]

}
```
