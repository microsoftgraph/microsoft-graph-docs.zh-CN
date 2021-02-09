---
title: 列出 userExperienceAnalyticsResourcePerformances
description: 列出 userExperienceAnalyticsResourcePerformance 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d06e48ed7533ec351305e075b6eb38f44504f7e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162246"
---
# <a name="list-userexperienceanalyticsresourceperformances"></a><span data-ttu-id="821d3-103">列出 userExperienceAnalyticsResourcePerformances</span><span class="sxs-lookup"><span data-stu-id="821d3-103">List userExperienceAnalyticsResourcePerformances</span></span>

<span data-ttu-id="821d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="821d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="821d3-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="821d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="821d3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="821d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="821d3-107">列出 [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="821d3-107">List properties and relationships of the [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="821d3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="821d3-108">Prerequisites</span></span>
<span data-ttu-id="821d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="821d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="821d3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="821d3-111">Permission type</span></span>|<span data-ttu-id="821d3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="821d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="821d3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="821d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="821d3-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="821d3-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="821d3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="821d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="821d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="821d3-116">Not supported.</span></span>|
|<span data-ttu-id="821d3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="821d3-117">Application</span></span>|<span data-ttu-id="821d3-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="821d3-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="821d3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="821d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a><span data-ttu-id="821d3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="821d3-120">Request headers</span></span>
|<span data-ttu-id="821d3-121">标头</span><span class="sxs-lookup"><span data-stu-id="821d3-121">Header</span></span>|<span data-ttu-id="821d3-122">值</span><span class="sxs-lookup"><span data-stu-id="821d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="821d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="821d3-123">Authorization</span></span>|<span data-ttu-id="821d3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="821d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="821d3-125">接受</span><span class="sxs-lookup"><span data-stu-id="821d3-125">Accept</span></span>|<span data-ttu-id="821d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="821d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="821d3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="821d3-127">Request body</span></span>
<span data-ttu-id="821d3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="821d3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="821d3-129">响应</span><span class="sxs-lookup"><span data-stu-id="821d3-129">Response</span></span>
<span data-ttu-id="821d3-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="821d3-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="821d3-131">示例</span><span class="sxs-lookup"><span data-stu-id="821d3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="821d3-132">请求</span><span class="sxs-lookup"><span data-stu-id="821d3-132">Request</span></span>
<span data-ttu-id="821d3-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="821d3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance
```

### <a name="response"></a><span data-ttu-id="821d3-134">响应</span><span class="sxs-lookup"><span data-stu-id="821d3-134">Response</span></span>
<span data-ttu-id="821d3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="821d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 691

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
      "id": "d34d78e8-78e8-d34d-e878-4dd3e8784dd3",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "model": "Model value",
      "deviceCount": 11,
      "manufacturer": "Manufacturer value",
      "cpuSpikeTimePercentage": 7.333333333333333,
      "ramSpikeTimePercentage": 7.333333333333333,
      "cpuSpikeTimeScore": 1,
      "cpuSpikeTimePercentageThreshold": 10.333333333333334,
      "ramSpikeTimeScore": 1,
      "ramSpikeTimePercentageThreshold": 10.333333333333334,
      "deviceResourcePerformanceScore": 14
    }
  ]
}
```




