---
title: 获取 deviceManagementPartner
description: 读取 deviceManagementPartner 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e4381162d7adc4e10423323522349a0639c4728
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791817"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="efd85-103">获取 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="efd85-103">Get deviceManagementPartner</span></span>

<span data-ttu-id="efd85-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efd85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efd85-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efd85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efd85-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efd85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efd85-107">读取 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="efd85-107">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efd85-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="efd85-108">Prerequisites</span></span>
<span data-ttu-id="efd85-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="efd85-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="efd85-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efd85-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd85-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="efd85-111">Permission type</span></span>|<span data-ttu-id="efd85-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="efd85-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efd85-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efd85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efd85-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="efd85-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="efd85-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efd85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efd85-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd85-116">Not supported.</span></span>|
|<span data-ttu-id="efd85-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="efd85-117">Application</span></span>|<span data-ttu-id="efd85-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="efd85-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efd85-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efd85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="efd85-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="efd85-120">Optional query parameters</span></span>
<span data-ttu-id="efd85-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="efd85-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efd85-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="efd85-122">Request headers</span></span>
|<span data-ttu-id="efd85-123">标头</span><span class="sxs-lookup"><span data-stu-id="efd85-123">Header</span></span>|<span data-ttu-id="efd85-124">值</span><span class="sxs-lookup"><span data-stu-id="efd85-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efd85-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="efd85-125">Authorization</span></span>|<span data-ttu-id="efd85-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="efd85-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efd85-127">接受</span><span class="sxs-lookup"><span data-stu-id="efd85-127">Accept</span></span>|<span data-ttu-id="efd85-128">application/json</span><span class="sxs-lookup"><span data-stu-id="efd85-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efd85-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="efd85-129">Request body</span></span>
<span data-ttu-id="efd85-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="efd85-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efd85-131">响应</span><span class="sxs-lookup"><span data-stu-id="efd85-131">Response</span></span>
<span data-ttu-id="efd85-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="efd85-132">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efd85-133">示例</span><span class="sxs-lookup"><span data-stu-id="efd85-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="efd85-134">请求</span><span class="sxs-lookup"><span data-stu-id="efd85-134">Request</span></span>
<span data-ttu-id="efd85-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efd85-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="efd85-136">响应</span><span class="sxs-lookup"><span data-stu-id="efd85-136">Response</span></span>
<span data-ttu-id="efd85-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="efd85-137">Here is an example of the response.</span></span> <span data-ttu-id="efd85-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="efd85-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="efd85-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="efd85-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1184

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementPartner",
    "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "partnerAppType": "singleTenantApp",
    "singleTenantAppId": "Single Tenant App Id value",
    "displayName": "Display Name value",
    "isConfigured": true,
    "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
    "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
    "groupsRequiringPartnerEnrollment": [
      {
        "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include"
        }
      }
    ]
  }
}
```



