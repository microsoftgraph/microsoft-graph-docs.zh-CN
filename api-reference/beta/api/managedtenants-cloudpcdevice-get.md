---
title: 获取 cloudPcDevice
description: 读取 cloudPcDevice 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 26d9b438bf366a0a3b4b367bc96ea74441d5324d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402054"
---
# <a name="get-cloudpcdevice"></a><span data-ttu-id="cfa7c-103">获取 cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="cfa7c-103">Get cloudPcDevice</span></span>
<span data-ttu-id="cfa7c-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="cfa7c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfa7c-105">读取 [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cfa7c-105">Read the properties and relationships of a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfa7c-106">权限</span><span class="sxs-lookup"><span data-stu-id="cfa7c-106">Permissions</span></span>
<span data-ttu-id="cfa7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfa7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfa7c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfa7c-109">Permission type</span></span>|<span data-ttu-id="cfa7c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfa7c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfa7c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfa7c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cfa7c-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfa7c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="cfa7c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfa7c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfa7c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfa7c-114">Not supported.</span></span>|
|<span data-ttu-id="cfa7c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfa7c-115">Application</span></span>|<span data-ttu-id="cfa7c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfa7c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfa7c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfa7c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cfa7c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cfa7c-118">Optional query parameters</span></span>
<span data-ttu-id="cfa7c-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="cfa7c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cfa7c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cfa7c-120">Request headers</span></span>
|<span data-ttu-id="cfa7c-121">名称</span><span class="sxs-lookup"><span data-stu-id="cfa7c-121">Name</span></span>|<span data-ttu-id="cfa7c-122">说明</span><span class="sxs-lookup"><span data-stu-id="cfa7c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cfa7c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfa7c-123">Authorization</span></span>|<span data-ttu-id="cfa7c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cfa7c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfa7c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfa7c-126">Request body</span></span>
<span data-ttu-id="cfa7c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cfa7c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfa7c-128">响应</span><span class="sxs-lookup"><span data-stu-id="cfa7c-128">Response</span></span>

<span data-ttu-id="cfa7c-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cfa7c-129">If successful, this method returns a `200 OK` response code and a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cfa7c-130">示例</span><span class="sxs-lookup"><span data-stu-id="cfa7c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cfa7c-131">请求</span><span class="sxs-lookup"><span data-stu-id="cfa7c-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```


### <a name="response"></a><span data-ttu-id="cfa7c-132">响应</span><span class="sxs-lookup"><span data-stu-id="cfa7c-132">Response</span></span>
><span data-ttu-id="cfa7c-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cfa7c-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
    "id": "1307ab1b-63ee-4942-bdef-bcd4f415c635",
    "lastUpdated": "2021-07-10T23:05:03.2564744Z",
    "policyId": "",
    "displayName": "device01",
    "managedDeviceId": "",
    "managedDeviceName": "",
    "userPrincipalName": "sally@lucernepublishing001.onmicrosoft.com",
    "servicePlanName": "CloudPC_Standard",
    "status": "NotProvisioned",
    "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
    "tenantDisplayName": "Lucerne Publishing",
    "lastRefreshedDateTime": "2021-07-10T23:05:03.2564744Z",
    "provisioningPolicyId": "",
    "cloudPcStatus": "NotProvisioned"
}
```
