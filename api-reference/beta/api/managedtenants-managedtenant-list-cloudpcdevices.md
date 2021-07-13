---
title: 列出 cloudPcDevices
description: 获取 cloudPcDevice 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 7ecb462727541ab591e921ff9cac5cbafcac612c
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402026"
---
# <a name="list-cloudpcdevices"></a><span data-ttu-id="40f10-103">列出 cloudPcDevices</span><span class="sxs-lookup"><span data-stu-id="40f10-103">List cloudPcDevices</span></span>
<span data-ttu-id="40f10-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="40f10-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40f10-105">获取 [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="40f10-105">Get a list of the [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="40f10-106">权限</span><span class="sxs-lookup"><span data-stu-id="40f10-106">Permissions</span></span>
<span data-ttu-id="40f10-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40f10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40f10-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="40f10-109">Permission type</span></span>|<span data-ttu-id="40f10-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40f10-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40f10-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40f10-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40f10-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40f10-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="40f10-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40f10-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40f10-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="40f10-114">Not supported.</span></span>|
|<span data-ttu-id="40f10-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="40f10-115">Application</span></span>|<span data-ttu-id="40f10-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40f10-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40f10-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40f10-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40f10-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="40f10-118">Optional query parameters</span></span>
<span data-ttu-id="40f10-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="40f10-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40f10-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="40f10-120">Request headers</span></span>
|<span data-ttu-id="40f10-121">名称</span><span class="sxs-lookup"><span data-stu-id="40f10-121">Name</span></span>|<span data-ttu-id="40f10-122">说明</span><span class="sxs-lookup"><span data-stu-id="40f10-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="40f10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40f10-123">Authorization</span></span>|<span data-ttu-id="40f10-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40f10-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40f10-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="40f10-126">Request body</span></span>
<span data-ttu-id="40f10-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40f10-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40f10-128">响应</span><span class="sxs-lookup"><span data-stu-id="40f10-128">Response</span></span>

<span data-ttu-id="40f10-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="40f10-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40f10-130">示例</span><span class="sxs-lookup"><span data-stu-id="40f10-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40f10-131">请求</span><span class="sxs-lookup"><span data-stu-id="40f10-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices
```


### <a name="response"></a><span data-ttu-id="40f10-132">响应</span><span class="sxs-lookup"><span data-stu-id="40f10-132">Response</span></span>
><span data-ttu-id="40f10-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="40f10-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcDevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "00089754-92d2-483c-a073-420723aac8bc_6b97ad6a-be15-4cbe-afbb-4eb74ecb0243",
      "lastUpdated": "2021-07-10T23:05:03.2565097Z",
      "policyId": "2b142388-f36c-40ee-a5cb-7e8871a658a0",
      "displayName": "ImageProd - ImageRunner4PROD",
      "managedDeviceId": "f3a8e53b-0a9f-42f1-be73-4fd30d801f62",
      "managedDeviceName": "A0000060000",
      "userPrincipalName": "ImageRunner4PROD@fourthcoffee001.onmicrosoft.com",
      "servicePlanName": "CloudPC_Lite",
      "status": "Provisioned",
      "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
      "tenantDisplayName": "Fourth Coffee Publishing",
      "lastRefreshedDateTime": "2021-07-10T23:05:03.2565097Z",
      "provisioningPolicyId": "2b142388-f36c-40ee-a5cb-7e8871a658a0",
      "cloudPcStatus": "Provisioned"
    }
  ]
}
```
