---
title: summarizeDevicePerformanceDevices 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1a0abea2af97b68a60f2fe0abc52ce3431adf92
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529212"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="6f67a-103">summarizeDevicePerformanceDevices 函数</span><span class="sxs-lookup"><span data-stu-id="6f67a-103">summarizeDevicePerformanceDevices function</span></span>

> <span data-ttu-id="6f67a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6f67a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f67a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f67a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f67a-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6f67a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f67a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f67a-107">Prerequisites</span></span>
<span data-ttu-id="6f67a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f67a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f67a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f67a-110">Permission type</span></span>|<span data-ttu-id="6f67a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f67a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f67a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f67a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f67a-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f67a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6f67a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f67a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f67a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f67a-115">Not supported.</span></span>|
|<span data-ttu-id="6f67a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f67a-116">Application</span></span>|<span data-ttu-id="6f67a-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f67a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f67a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f67a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="6f67a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f67a-119">Request headers</span></span>
|<span data-ttu-id="6f67a-120">标头</span><span class="sxs-lookup"><span data-stu-id="6f67a-120">Header</span></span>|<span data-ttu-id="6f67a-121">值</span><span class="sxs-lookup"><span data-stu-id="6f67a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f67a-122">授权</span><span class="sxs-lookup"><span data-stu-id="6f67a-122">Authorization</span></span>|<span data-ttu-id="6f67a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f67a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f67a-124">接受</span><span class="sxs-lookup"><span data-stu-id="6f67a-124">Accept</span></span>|<span data-ttu-id="6f67a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f67a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f67a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f67a-126">Request body</span></span>
<span data-ttu-id="6f67a-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="6f67a-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6f67a-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="6f67a-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6f67a-129">属性</span><span class="sxs-lookup"><span data-stu-id="6f67a-129">Property</span></span>|<span data-ttu-id="6f67a-130">类型</span><span class="sxs-lookup"><span data-stu-id="6f67a-130">Type</span></span>|<span data-ttu-id="6f67a-131">说明</span><span class="sxs-lookup"><span data-stu-id="6f67a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f67a-132">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="6f67a-132">summarizeBy</span></span>|[<span data-ttu-id="6f67a-133">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="6f67a-133">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="6f67a-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6f67a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6f67a-135">响应</span><span class="sxs-lookup"><span data-stu-id="6f67a-135">Response</span></span>
<span data-ttu-id="6f67a-136">如果成功，此函数会在`200 OK`响应正文中返回响应代码和[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)集合。</span><span class="sxs-lookup"><span data-stu-id="6f67a-136">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f67a-137">示例</span><span class="sxs-lookup"><span data-stu-id="6f67a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f67a-138">请求</span><span class="sxs-lookup"><span data-stu-id="6f67a-138">Request</span></span>
<span data-ttu-id="6f67a-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f67a-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="6f67a-140">响应</span><span class="sxs-lookup"><span data-stu-id="6f67a-140">Response</span></span>
<span data-ttu-id="6f67a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f67a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 636

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
      "id": "852ae826-e826-852a-26e8-2a8526e82a85",
      "deviceName": "Device Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "diskType": "hdd",
      "operatingSystemVersion": "Operating System Version value",
      "bootScore": 9,
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "healthStatus": "insufficientData",
      "loginScore": 10,
      "coreLoginTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "deviceCount": 11
    }
  ]
}
```






