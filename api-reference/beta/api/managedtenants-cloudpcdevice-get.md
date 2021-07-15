---
title: 获取 cloudPcDevice
description: 读取 cloudPcDevice 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 7ac75ce4b9ae607d3a616bc630f10d4e7c4e7fa3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440162"
---
# <a name="get-cloudpcdevice"></a><span data-ttu-id="ff608-103">获取 cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="ff608-103">Get cloudPcDevice</span></span>
<span data-ttu-id="ff608-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ff608-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff608-105">读取 [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff608-105">Read the properties and relationships of a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff608-106">权限</span><span class="sxs-lookup"><span data-stu-id="ff608-106">Permissions</span></span>
<span data-ttu-id="ff608-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff608-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff608-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff608-109">Permission type</span></span>|<span data-ttu-id="ff608-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff608-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff608-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff608-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff608-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff608-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ff608-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff608-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff608-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff608-114">Not supported.</span></span>|
|<span data-ttu-id="ff608-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff608-115">Application</span></span>|<span data-ttu-id="ff608-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff608-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff608-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff608-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff608-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ff608-118">Optional query parameters</span></span>
<span data-ttu-id="ff608-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="ff608-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff608-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff608-120">Request headers</span></span>
|<span data-ttu-id="ff608-121">名称</span><span class="sxs-lookup"><span data-stu-id="ff608-121">Name</span></span>|<span data-ttu-id="ff608-122">说明</span><span class="sxs-lookup"><span data-stu-id="ff608-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ff608-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff608-123">Authorization</span></span>|<span data-ttu-id="ff608-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff608-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff608-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff608-126">Request body</span></span>
<span data-ttu-id="ff608-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ff608-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff608-128">响应</span><span class="sxs-lookup"><span data-stu-id="ff608-128">Response</span></span>

<span data-ttu-id="ff608-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff608-129">If successful, this method returns a `200 OK` response code and a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff608-130">示例</span><span class="sxs-lookup"><span data-stu-id="ff608-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff608-131">请求</span><span class="sxs-lookup"><span data-stu-id="ff608-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ff608-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff608-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```
# <a name="c"></a>[<span data-ttu-id="ff608-133">C#</span><span class="sxs-lookup"><span data-stu-id="ff608-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcdevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff608-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff608-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcdevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff608-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff608-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcdevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff608-136">Java</span><span class="sxs-lookup"><span data-stu-id="ff608-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcdevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ff608-137">响应</span><span class="sxs-lookup"><span data-stu-id="ff608-137">Response</span></span>
><span data-ttu-id="ff608-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ff608-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
