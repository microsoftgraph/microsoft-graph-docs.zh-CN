---
title: 获取 cloudPcOnPremisesConnection
description: 读取 cloudPcOnPremisesConnection 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 291e6e17494bf8dcfc467b8d3c594f27d6b2e710
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546838"
---
# <a name="get-cloudpconpremisesconnection"></a><span data-ttu-id="a3b3d-103">获取 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="a3b3d-103">Get cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="a3b3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3b3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3b3d-105">读取 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-105">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="a3b3d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a3b3d-106">Permissions</span></span>

<span data-ttu-id="a3b3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3b3d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3b3d-109">Permission type</span></span>| <span data-ttu-id="a3b3d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3b3d-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="a3b3d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3b3d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3b3d-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3b3d-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a3b3d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3b3d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3b3d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-114">Not supported.</span></span>|
|<span data-ttu-id="a3b3d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3b3d-115">Application</span></span>|<span data-ttu-id="a3b3d-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3b3d-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3b3d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3b3d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3b3d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a3b3d-118">Optional query parameters</span></span>

<span data-ttu-id="a3b3d-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="a3b3d-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3b3d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3b3d-121">Request headers</span></span>

| <span data-ttu-id="a3b3d-122">名称</span><span class="sxs-lookup"><span data-stu-id="a3b3d-122">Name</span></span>          | <span data-ttu-id="a3b3d-123">说明</span><span class="sxs-lookup"><span data-stu-id="a3b3d-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a3b3d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3b3d-124">Authorization</span></span> | <span data-ttu-id="a3b3d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3b3d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3b3d-127">Request body</span></span>

<span data-ttu-id="a3b3d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3b3d-129">响应</span><span class="sxs-lookup"><span data-stu-id="a3b3d-129">Response</span></span>

<span data-ttu-id="a3b3d-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-130">If successful, this method returns a `200 OK` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3b3d-131">示例</span><span class="sxs-lookup"><span data-stu-id="a3b3d-131">Examples</span></span>

### <a name="example-1-get-the-default-properties-of-an-on-premises-connection"></a><span data-ttu-id="a3b3d-132">示例 1：获取本地连接的默认属性</span><span class="sxs-lookup"><span data-stu-id="a3b3d-132">Example 1: Get the default properties of an on-premises connection</span></span>

#### <a name="request"></a><span data-ttu-id="a3b3d-133">请求</span><span class="sxs-lookup"><span data-stu-id="a3b3d-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a3b3d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3b3d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="a3b3d-135">C#</span><span class="sxs-lookup"><span data-stu-id="a3b3d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3b3d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3b3d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3b3d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3b3d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3b3d-138">Java</span><span class="sxs-lookup"><span data-stu-id="a3b3d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3b3d-139">响应</span><span class="sxs-lookup"><span data-stu-id="a3b3d-139">Response</span></span>

<span data-ttu-id="a3b3d-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
    "id": "9ec90ff8-fd63-4fb9-ab5a-aa4fdccffff",
    "displayName": "Display Name value",
    "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
    "subscriptionName": "Subscription Name value",
    "adDomainName": "Active Directory Domain Name value",
    "adDomainUsername": "Active Directory Domain User Name value",
    "organizationalUnit": "Organization Unit value",
    "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
    "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
    "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
    "healthCheckStatus": "running"
  }
}
```

### <a name="example-2-get-the-selected-properties-of-an-on-premises-connection-including-healthcheckstatusdetails"></a><span data-ttu-id="a3b3d-141">示例 2：获取本地连接的选定属性，包括 healthCheckStatusDetails</span><span class="sxs-lookup"><span data-stu-id="a3b3d-141">Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails</span></span>

#### <a name="request"></a><span data-ttu-id="a3b3d-142">请求</span><span class="sxs-lookup"><span data-stu-id="a3b3d-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a3b3d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3b3d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection_withDetails"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}?$select=id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse
```
# <a name="c"></a>[<span data-ttu-id="a3b3d-144">C#</span><span class="sxs-lookup"><span data-stu-id="a3b3d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-withdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3b3d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3b3d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-withdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3b3d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3b3d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-withdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3b3d-147">Java</span><span class="sxs-lookup"><span data-stu-id="a3b3d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-withdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a3b3d-148">响应</span><span class="sxs-lookup"><span data-stu-id="a3b3d-148">Response</span></span>

<span data-ttu-id="a3b3d-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3b3d-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
    "id": "9ec90ff8-fd63-4fb9-ab5a-aa4fdccffff",
    "displayName": "Display Name value",
    "healthCheckStatus": "failed",
    "healthCheckStatusDetails": {
      "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
      "startDateTime": "2020-11-03T12:43:14Z",
      "endDateTime": "2020-11-03T12:43:32Z",
      "healthChecks": [
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "failed",
          "displayName": "Display Name value",
          "startDateTime": "2020-11-03T12:43:14Z",
          "endDateTime": "2020-11-03T12:43:15Z",
          "errorType": "dnsCheckFqdnNotFound",
          "recommendedAction": "We did not find the provided domain name; please re-enter",
          "additionalDdetails": null
        },
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "passed",
          "displayName": "Display Name value",
          "startDateTime": "2020-11-03T12:43:15Z",
          "endDateTime": "2020-11-03T12:43:26Z",
          "errorType": null,
          "recommendedAction": null,
          "additionalDetails": null
        },
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "failed",
          "displayName": "Display Name value",
          "startDateTime": "2020-11-03T12:43:27Z",
          "endDateTime": "2020-11-03T12:43:32Z",
          "errorType": "endpointConnectivityCheckUrlNotWhitelisted",
          "recommendedAction": "Recommended Action value",
          "additionaldDetails": "Additional Details value"
        },
        {
          "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
          "status": "passed",
          "displayName": "Display Name value",
          "startDateTime": null,
          "endDateTime": null,
          "errorType": null,
          "recommendedAction": null,
          "additionaldDetails": null
        }
      ]
    },
    "inUse": false
  }
}
```
