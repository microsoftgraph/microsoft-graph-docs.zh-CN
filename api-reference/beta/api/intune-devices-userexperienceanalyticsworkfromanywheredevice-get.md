---
title: 获取 userExperienceAnalyticsWorkFromAnywhereDevice
description: 读取 userExperienceAnalyticsWorkFromAnywhereDevice 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f803b9f0857e32aa02d6fb5e881a6e4df044caaa
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665040"
---
# <a name="get-userexperienceanalyticsworkfromanywheredevice"></a><span data-ttu-id="f3574-103">获取 userExperienceAnalyticsWorkFromAnywhereDevice</span><span class="sxs-lookup"><span data-stu-id="f3574-103">Get userExperienceAnalyticsWorkFromAnywhereDevice</span></span>

<span data-ttu-id="f3574-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3574-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3574-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3574-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3574-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3574-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3574-107">读取 [userExperienceAnalyticsWorkFromAnywhereDevice 对象的属性和](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="f3574-107">Read properties and relationships of the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3574-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f3574-108">Prerequisites</span></span>
<span data-ttu-id="f3574-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3574-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3574-111">Permission type</span></span>|<span data-ttu-id="f3574-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3574-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3574-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3574-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3574-114">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3574-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3574-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3574-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3574-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3574-116">Not supported.</span></span>|
|<span data-ttu-id="f3574-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3574-117">Application</span></span>|<span data-ttu-id="f3574-118">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3574-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3574-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3574-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3574-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f3574-120">Optional query parameters</span></span>
<span data-ttu-id="f3574-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f3574-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3574-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3574-122">Request headers</span></span>
|<span data-ttu-id="f3574-123">标头</span><span class="sxs-lookup"><span data-stu-id="f3574-123">Header</span></span>|<span data-ttu-id="f3574-124">值</span><span class="sxs-lookup"><span data-stu-id="f3574-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3574-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3574-125">Authorization</span></span>|<span data-ttu-id="f3574-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f3574-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3574-127">接受</span><span class="sxs-lookup"><span data-stu-id="f3574-127">Accept</span></span>|<span data-ttu-id="f3574-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f3574-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3574-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3574-129">Request body</span></span>
<span data-ttu-id="f3574-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f3574-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3574-131">响应</span><span class="sxs-lookup"><span data-stu-id="f3574-131">Response</span></span>
<span data-ttu-id="f3574-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3574-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3574-133">示例</span><span class="sxs-lookup"><span data-stu-id="f3574-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3574-134">请求</span><span class="sxs-lookup"><span data-stu-id="f3574-134">Request</span></span>
<span data-ttu-id="f3574-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3574-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

### <a name="response"></a><span data-ttu-id="f3574-136">响应</span><span class="sxs-lookup"><span data-stu-id="f3574-136">Response</span></span>
<span data-ttu-id="f3574-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3574-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 683

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
    "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
    "deviceName": "Device Name value",
    "serialNumber": "Serial Number value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "ownership": "Ownership value",
    "managedBy": "Managed By value",
    "autoPilotRegistered": true,
    "autoPilotProfileAssigned": true,
    "azureAdRegistered": true,
    "azureAdDeviceId": "Azure Ad Device Id value",
    "azureAdJoinType": "Azure Ad Join Type value",
    "osDescription": "Os Description value",
    "osVersion": "Os Version value"
  }
}
```




