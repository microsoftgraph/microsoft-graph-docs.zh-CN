---
title: 获取 userExperienceAnalyticsAppHealthDeviceModelPerformance
description: 读取 userExperienceAnalyticsAppHealthDeviceModelPerformance 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62ef197ee7d428ce11137752c6644f77e1cb17d8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734096"
---
# <a name="get-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="d88be-103">获取 userExperienceAnalyticsAppHealthDeviceModelPerformance</span><span class="sxs-lookup"><span data-stu-id="d88be-103">Get userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="d88be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d88be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d88be-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d88be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d88be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d88be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d88be-107">读取 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d88be-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d88be-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d88be-108">Prerequisites</span></span>
<span data-ttu-id="d88be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d88be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d88be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d88be-111">Permission type</span></span>|<span data-ttu-id="d88be-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d88be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d88be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d88be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d88be-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d88be-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d88be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d88be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d88be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d88be-116">Not supported.</span></span>|
|<span data-ttu-id="d88be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d88be-117">Application</span></span>|<span data-ttu-id="d88be-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d88be-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d88be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d88be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d88be-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d88be-120">Optional query parameters</span></span>
<span data-ttu-id="d88be-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d88be-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d88be-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d88be-122">Request headers</span></span>
|<span data-ttu-id="d88be-123">标头</span><span class="sxs-lookup"><span data-stu-id="d88be-123">Header</span></span>|<span data-ttu-id="d88be-124">值</span><span class="sxs-lookup"><span data-stu-id="d88be-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d88be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d88be-125">Authorization</span></span>|<span data-ttu-id="d88be-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d88be-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d88be-127">接受</span><span class="sxs-lookup"><span data-stu-id="d88be-127">Accept</span></span>|<span data-ttu-id="d88be-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d88be-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d88be-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d88be-129">Request body</span></span>
<span data-ttu-id="d88be-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d88be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d88be-131">响应</span><span class="sxs-lookup"><span data-stu-id="d88be-131">Response</span></span>
<span data-ttu-id="d88be-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d88be-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d88be-133">示例</span><span class="sxs-lookup"><span data-stu-id="d88be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d88be-134">请求</span><span class="sxs-lookup"><span data-stu-id="d88be-134">Request</span></span>
<span data-ttu-id="d88be-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d88be-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

### <a name="response"></a><span data-ttu-id="d88be-136">响应</span><span class="sxs-lookup"><span data-stu-id="d88be-136">Response</span></span>
<span data-ttu-id="d88be-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d88be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





