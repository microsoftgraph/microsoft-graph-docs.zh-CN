---
title: 列出 cloudPcOnPremisesConnections
description: 获取 cloudPcOnPremisesConnection 对象及其属性的列表。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 4382453196900685363d72aa514b67cf98d94b1e
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992840"
---
# <a name="list-onpremisesconnections"></a><span data-ttu-id="5619d-103">列出 onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="5619d-103">List onPremisesConnections</span></span>

<span data-ttu-id="5619d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5619d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5619d-105">列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5619d-105">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="5619d-106">权限</span><span class="sxs-lookup"><span data-stu-id="5619d-106">Permissions</span></span>

<span data-ttu-id="5619d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5619d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5619d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5619d-109">Permission type</span></span>|<span data-ttu-id="5619d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5619d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5619d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5619d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5619d-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5619d-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="5619d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5619d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5619d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5619d-114">Not supported.</span></span>|
|<span data-ttu-id="5619d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5619d-115">Application</span></span>|<span data-ttu-id="5619d-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5619d-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5619d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5619d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5619d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5619d-118">Optional query parameters</span></span>

<span data-ttu-id="5619d-119">此方法支持 `$select` `$filter` 和 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5619d-119">This method supports `$select` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="5619d-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5619d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5619d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5619d-121">Request headers</span></span>

| <span data-ttu-id="5619d-122">名称</span><span class="sxs-lookup"><span data-stu-id="5619d-122">Name</span></span>          | <span data-ttu-id="5619d-123">说明</span><span class="sxs-lookup"><span data-stu-id="5619d-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5619d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5619d-124">Authorization</span></span> | <span data-ttu-id="5619d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5619d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5619d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5619d-127">Request body</span></span>

<span data-ttu-id="5619d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5619d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5619d-129">响应</span><span class="sxs-lookup"><span data-stu-id="5619d-129">Response</span></span>

<span data-ttu-id="5619d-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5619d-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5619d-131">示例</span><span class="sxs-lookup"><span data-stu-id="5619d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5619d-132">请求</span><span class="sxs-lookup"><span data-stu-id="5619d-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5619d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5619d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpconpremisesconnections"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections
```
# <a name="c"></a>[<span data-ttu-id="5619d-134">C#</span><span class="sxs-lookup"><span data-stu-id="5619d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpconpremisesconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5619d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5619d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpconpremisesconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5619d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5619d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpconpremisesconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5619d-137">Java</span><span class="sxs-lookup"><span data-stu-id="5619d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpconpremisesconnections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5619d-138">响应</span><span class="sxs-lookup"><span data-stu-id="5619d-138">Response</span></span>

<span data-ttu-id="5619d-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5619d-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcOnPremisesConnection)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
      "id": "07f12770-a225-4957-9127-0d247cf4ffff",
      "displayName": "Display Name value",
      "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
      "subscriptionName": "Subscription Name value",
      "adDomainName": "Active Directory Domain Name value",
      "adDomainUsername": "Active Directory Domain User Name value",
      "organizationalUnit": "Organization Unit value",
      "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
      "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
      "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
      "healthCheckStatus": "passed"
    }
  ]
}
```
