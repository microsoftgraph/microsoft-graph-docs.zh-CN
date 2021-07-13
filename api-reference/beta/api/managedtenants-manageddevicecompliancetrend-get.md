---
title: 获取 managedDeviceComplianceTrend
description: 读取 managedDeviceComplianceTrend 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 046b110c0aad542db3994bc6eecbba9b1d414feb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402046"
---
# <a name="get-manageddevicecompliancetrend"></a><span data-ttu-id="9cd49-103">获取 managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="9cd49-103">Get managedDeviceComplianceTrend</span></span>
<span data-ttu-id="9cd49-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="9cd49-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cd49-105">读取 [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9cd49-105">Read the properties and relationships of a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cd49-106">权限</span><span class="sxs-lookup"><span data-stu-id="9cd49-106">Permissions</span></span>
<span data-ttu-id="9cd49-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cd49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cd49-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cd49-109">Permission type</span></span>|<span data-ttu-id="9cd49-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cd49-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cd49-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cd49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9cd49-112">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cd49-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9cd49-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cd49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cd49-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cd49-114">Not supported.</span></span>|
|<span data-ttu-id="9cd49-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cd49-115">Application</span></span>|<span data-ttu-id="9cd49-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cd49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cd49-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cd49-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9cd49-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9cd49-118">Optional query parameters</span></span>
<span data-ttu-id="9cd49-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="9cd49-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cd49-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cd49-120">Request headers</span></span>
|<span data-ttu-id="9cd49-121">名称</span><span class="sxs-lookup"><span data-stu-id="9cd49-121">Name</span></span>|<span data-ttu-id="9cd49-122">说明</span><span class="sxs-lookup"><span data-stu-id="9cd49-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9cd49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cd49-123">Authorization</span></span>|<span data-ttu-id="9cd49-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cd49-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cd49-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cd49-126">Request body</span></span>
<span data-ttu-id="9cd49-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cd49-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cd49-128">响应</span><span class="sxs-lookup"><span data-stu-id="9cd49-128">Response</span></span>

<span data-ttu-id="9cd49-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9cd49-129">If successful, this method returns a `200 OK` response code and a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9cd49-130">示例</span><span class="sxs-lookup"><span data-stu-id="9cd49-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9cd49-131">请求</span><span class="sxs-lookup"><span data-stu-id="9cd49-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecompliancetrend"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```


### <a name="response"></a><span data-ttu-id="9cd49-132">响应</span><span class="sxs-lookup"><span data-stu-id="9cd49-132">Response</span></span>
><span data-ttu-id="9cd49-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9cd49-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b_2021-07-11T00:00:00Z",
  "tenantDisplayName": "Fourth Coffee",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "unknownDeviceCount": 2,
  "compliantDeviceCount": 0,
  "noncompliantDeviceCount": 41,
  "errorDeviceCount": 1,
  "inGracePeriodDeviceCount": 0,
  "configManagerDeviceCount": 0,
  "totalDeviceCount": 44,
  "countDateTime": "2021-07-11T00:00:00Z"
}
```
