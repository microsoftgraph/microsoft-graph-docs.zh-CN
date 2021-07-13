---
title: 获取 managedDeviceCompliance
description: 读取 managedDeviceCompliance 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: be93e13c483e11327bfe5725d9b779cfccd89354
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402047"
---
# <a name="get-manageddevicecompliance"></a><span data-ttu-id="5946a-103">获取 managedDeviceCompliance</span><span class="sxs-lookup"><span data-stu-id="5946a-103">Get managedDeviceCompliance</span></span>
<span data-ttu-id="5946a-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="5946a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5946a-105">读取 [managedDeviceCompliance 对象的属性和](../resources/managedtenants-manageddevicecompliance.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="5946a-105">Read the properties and relationships of a [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5946a-106">权限</span><span class="sxs-lookup"><span data-stu-id="5946a-106">Permissions</span></span>
<span data-ttu-id="5946a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5946a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5946a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5946a-109">Permission type</span></span>|<span data-ttu-id="5946a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5946a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5946a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5946a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5946a-112">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5946a-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5946a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5946a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5946a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5946a-114">Not supported.</span></span>|
|<span data-ttu-id="5946a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5946a-115">Application</span></span>|<span data-ttu-id="5946a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5946a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5946a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5946a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5946a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5946a-118">Optional query parameters</span></span>
<span data-ttu-id="5946a-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="5946a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5946a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5946a-120">Request headers</span></span>
|<span data-ttu-id="5946a-121">名称</span><span class="sxs-lookup"><span data-stu-id="5946a-121">Name</span></span>|<span data-ttu-id="5946a-122">说明</span><span class="sxs-lookup"><span data-stu-id="5946a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5946a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5946a-123">Authorization</span></span>|<span data-ttu-id="5946a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5946a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5946a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5946a-126">Request body</span></span>
<span data-ttu-id="5946a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5946a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5946a-128">响应</span><span class="sxs-lookup"><span data-stu-id="5946a-128">Response</span></span>

<span data-ttu-id="5946a-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5946a-129">If successful, this method returns a `200 OK` response code and a [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5946a-130">示例</span><span class="sxs-lookup"><span data-stu-id="5946a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5946a-131">请求</span><span class="sxs-lookup"><span data-stu-id="5946a-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceCompliances/{managedDeviceComplianceId}
```


### <a name="response"></a><span data-ttu-id="5946a-132">响应</span><span class="sxs-lookup"><span data-stu-id="5946a-132">Response</span></span>
><span data-ttu-id="5946a-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5946a-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceCompliance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managedDeviceCompliances/$entity",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b_95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceId": "95378ac4-eded-4671-8fa2-4e42e5de3463",
    "managedDeviceName": "vm11",
    "complianceStatus": "Compliant",
    "osDescription": "Windows",
    "osVersion": "10.0.19042.1083",
    "lastSyncDateTime": "2021-07-09T14:41:21.9130091Z",
    "ownerType": "Company",
    "model": "Virtual Machine",
    "manufacturer": "Microsoft Corporation",
    "inGracePeriodUntilDateTime": "9999-12-31T23:59:59.9999999Z",
    "lastRefreshedDateTime": "2021-07-11T07:12:41.0336556Z",
    "deviceType": "WindowsRT",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee"
}
```
