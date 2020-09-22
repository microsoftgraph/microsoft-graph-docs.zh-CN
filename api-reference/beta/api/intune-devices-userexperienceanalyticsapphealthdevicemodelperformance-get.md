---
title: 获取 userExperienceAnalyticsAppHealthDeviceModelPerformance
description: 读取 userExperienceAnalyticsAppHealthDeviceModelPerformance 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a28b1ab458139b1ecd542991ef1de0e189b202f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992595"
---
# <a name="get-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="51113-103">获取 userExperienceAnalyticsAppHealthDeviceModelPerformance</span><span class="sxs-lookup"><span data-stu-id="51113-103">Get userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="51113-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51113-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51113-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51113-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51113-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51113-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51113-107">读取 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="51113-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51113-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="51113-108">Prerequisites</span></span>
<span data-ttu-id="51113-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51113-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51113-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="51113-111">Permission type</span></span>|<span data-ttu-id="51113-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51113-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51113-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51113-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51113-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="51113-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="51113-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51113-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51113-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="51113-116">Not supported.</span></span>|
|<span data-ttu-id="51113-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="51113-117">Application</span></span>|<span data-ttu-id="51113-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="51113-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51113-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51113-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51113-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="51113-120">Optional query parameters</span></span>
<span data-ttu-id="51113-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="51113-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51113-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="51113-122">Request headers</span></span>
|<span data-ttu-id="51113-123">标头</span><span class="sxs-lookup"><span data-stu-id="51113-123">Header</span></span>|<span data-ttu-id="51113-124">值</span><span class="sxs-lookup"><span data-stu-id="51113-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51113-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="51113-125">Authorization</span></span>|<span data-ttu-id="51113-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51113-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51113-127">接受</span><span class="sxs-lookup"><span data-stu-id="51113-127">Accept</span></span>|<span data-ttu-id="51113-128">application/json</span><span class="sxs-lookup"><span data-stu-id="51113-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51113-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="51113-129">Request body</span></span>
<span data-ttu-id="51113-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="51113-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51113-131">响应</span><span class="sxs-lookup"><span data-stu-id="51113-131">Response</span></span>
<span data-ttu-id="51113-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51113-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51113-133">示例</span><span class="sxs-lookup"><span data-stu-id="51113-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="51113-134">请求</span><span class="sxs-lookup"><span data-stu-id="51113-134">Request</span></span>
<span data-ttu-id="51113-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51113-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

### <a name="response"></a><span data-ttu-id="51113-136">响应</span><span class="sxs-lookup"><span data-stu-id="51113-136">Response</span></span>
<span data-ttu-id="51113-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51113-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
    "id": "4daddc60-dc60-4dad-60dc-ad4d60dcad4d",
    "deviceModel": "Device Model value",
    "deviceManufacturer": "Device Manufacturer value",
    "activeDeviceCount": 1,
    "meanTimeToFailureInMinutes": 10,
    "modelAppHealthScore": 6.333333333333333,
    "modelAppHealthStatus": "Model App Health Status value"
  }
}
```






