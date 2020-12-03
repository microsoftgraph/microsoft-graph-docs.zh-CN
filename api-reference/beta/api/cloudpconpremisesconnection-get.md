---
title: 获取 cloudPcOnPremisesConnection
description: 读取 cloudPcOnPremisesConnection 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e7e70e6ff0f5ea8badb314c1a5fa915d2f657a6b
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563401"
---
# <a name="get-cloudpconpremisesconnection"></a><span data-ttu-id="36699-103">获取 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="36699-103">Get cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="36699-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36699-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36699-105">读取 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="36699-105">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="36699-106">权限</span><span class="sxs-lookup"><span data-stu-id="36699-106">Permissions</span></span>

<span data-ttu-id="36699-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36699-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36699-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36699-109">Permission type</span></span>| <span data-ttu-id="36699-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36699-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="36699-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36699-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36699-112">CloudPC、CloudPC 和全部读。</span><span class="sxs-lookup"><span data-stu-id="36699-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="36699-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36699-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36699-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="36699-114">Not supported.</span></span>|
|<span data-ttu-id="36699-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36699-115">Application</span></span>| <span data-ttu-id="36699-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36699-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36699-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36699-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36699-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="36699-118">Optional query parameters</span></span>

<span data-ttu-id="36699-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="36699-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="36699-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="36699-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="36699-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="36699-121">Request headers</span></span>

| <span data-ttu-id="36699-122">名称</span><span class="sxs-lookup"><span data-stu-id="36699-122">Name</span></span>          | <span data-ttu-id="36699-123">说明</span><span class="sxs-lookup"><span data-stu-id="36699-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="36699-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="36699-124">Authorization</span></span> | <span data-ttu-id="36699-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36699-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36699-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="36699-127">Request body</span></span>

<span data-ttu-id="36699-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36699-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36699-129">响应</span><span class="sxs-lookup"><span data-stu-id="36699-129">Response</span></span>

<span data-ttu-id="36699-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36699-130">If successful, this method returns a `200 OK` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36699-131">示例</span><span class="sxs-lookup"><span data-stu-id="36699-131">Examples</span></span>

### <a name="example-1-get-the-default-properties-of-an-on-premises-connection"></a><span data-ttu-id="36699-132">示例1：获取本地连接的默认属性</span><span class="sxs-lookup"><span data-stu-id="36699-132">Example 1: Get the default properties of an on-premises connection</span></span>

#### <a name="request"></a><span data-ttu-id="36699-133">请求</span><span class="sxs-lookup"><span data-stu-id="36699-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36699-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="36699-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="36699-135">C#</span><span class="sxs-lookup"><span data-stu-id="36699-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36699-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36699-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36699-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36699-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36699-138">Java</span><span class="sxs-lookup"><span data-stu-id="36699-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36699-139">响应</span><span class="sxs-lookup"><span data-stu-id="36699-139">Response</span></span>

<span data-ttu-id="36699-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36699-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "healthCheckStatus": "running",
    "inUse": false
  }
}
```

### <a name="example-2-get-the-selected-properties-of-an-on-premises-connection-including-healthcheckstatusdetails"></a><span data-ttu-id="36699-141">示例2：获取本地连接的选定属性，包括 healthCheckStatusDetails</span><span class="sxs-lookup"><span data-stu-id="36699-141">Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails</span></span>

#### <a name="request"></a><span data-ttu-id="36699-142">请求</span><span class="sxs-lookup"><span data-stu-id="36699-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36699-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="36699-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpconpremisesconnection_withDetails"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}?$select=id,displayName,subscriptionId,subscriptionName,adDomainName,adDomainUsername,organizationalUnit,virtualNetworkId,subnetId,healthCheckStatus,healthCheckStatusDetails,inUse
```
# <a name="c"></a>[<span data-ttu-id="36699-144">C#</span><span class="sxs-lookup"><span data-stu-id="36699-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpconpremisesconnection-withdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36699-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36699-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpconpremisesconnection-withdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36699-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36699-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpconpremisesconnection-withdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36699-147">Java</span><span class="sxs-lookup"><span data-stu-id="36699-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpconpremisesconnection-withdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36699-148">响应</span><span class="sxs-lookup"><span data-stu-id="36699-148">Response</span></span>

<span data-ttu-id="36699-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36699-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
