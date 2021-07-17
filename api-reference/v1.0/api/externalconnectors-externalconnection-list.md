---
title: 列出 externalConnections
description: 获取 externalConnection 对象及其属性的列表。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 07b0db1eb735999263bc5d2855e7c263351f02e0
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467286"
---
# <a name="list-externalconnections"></a><span data-ttu-id="1d4d8-103">列出 externalConnections</span><span class="sxs-lookup"><span data-stu-id="1d4d8-103">List externalConnections</span></span>
<span data-ttu-id="1d4d8-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="1d4d8-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="1d4d8-105">获取 [externalConnection 对象](../resources/externalconnectors-externalconnection.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="1d4d8-105">Get a list of the [externalConnection](../resources/externalconnectors-externalconnection.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d4d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="1d4d8-106">Permissions</span></span>
<span data-ttu-id="1d4d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d4d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d4d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d4d8-109">Permission type</span></span>|<span data-ttu-id="1d4d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d4d8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d4d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d4d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d4d8-112">不适用</span><span class="sxs-lookup"><span data-stu-id="1d4d8-112">Not applicable</span></span>|
|<span data-ttu-id="1d4d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d4d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d4d8-114">不适用</span><span class="sxs-lookup"><span data-stu-id="1d4d8-114">Not applicable</span></span>|
|<span data-ttu-id="1d4d8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d4d8-115">Application</span></span>| <span data-ttu-id="1d4d8-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="1d4d8-116">ExternalConnection.ReadWrite.OwnedBy</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d4d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d4d8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d4d8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1d4d8-118">Optional query parameters</span></span>
<span data-ttu-id="1d4d8-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1d4d8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1d4d8-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1d4d8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d4d8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d4d8-121">Request headers</span></span>
|<span data-ttu-id="1d4d8-122">名称</span><span class="sxs-lookup"><span data-stu-id="1d4d8-122">Name</span></span>|<span data-ttu-id="1d4d8-123">说明</span><span class="sxs-lookup"><span data-stu-id="1d4d8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d4d8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d4d8-124">Authorization</span></span>|<span data-ttu-id="1d4d8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d4d8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d4d8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d4d8-127">Request body</span></span>
<span data-ttu-id="1d4d8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1d4d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d4d8-129">响应</span><span class="sxs-lookup"><span data-stu-id="1d4d8-129">Response</span></span>

<span data-ttu-id="1d4d8-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [externalConnection](../resources/externalconnectors-externalconnection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1d4d8-130">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnectors-externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d4d8-131">示例</span><span class="sxs-lookup"><span data-stu-id="1d4d8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d4d8-132">请求</span><span class="sxs-lookup"><span data-stu-id="1d4d8-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_externalconnection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/connections
```


### <a name="response"></a><span data-ttu-id="1d4d8-133">响应</span><span class="sxs-lookup"><span data-stu-id="1d4d8-133">Response</span></span>
<span data-ttu-id="1d4d8-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1d4d8-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.externalConnectors.externalConnection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "contosohr",
      "name": "Contoso HR",
      "description": "Connection to index Contoso HR system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    }
  ]
}
```

