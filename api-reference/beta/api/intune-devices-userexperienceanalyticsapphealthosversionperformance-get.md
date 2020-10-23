---
title: 获取 userExperienceAnalyticsAppHealthOSVersionPerformance
description: 读取 userExperienceAnalyticsAppHealthOSVersionPerformance 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a046dc500ed6626100224d595b9600f4d5bd19b4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691692"
---
# <a name="get-userexperienceanalyticsapphealthosversionperformance"></a><span data-ttu-id="6efb3-103">获取 userExperienceAnalyticsAppHealthOSVersionPerformance</span><span class="sxs-lookup"><span data-stu-id="6efb3-103">Get userExperienceAnalyticsAppHealthOSVersionPerformance</span></span>

<span data-ttu-id="6efb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6efb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6efb3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6efb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6efb3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6efb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6efb3-107">读取 [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6efb3-107">Read properties and relationships of the [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6efb3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6efb3-108">Prerequisites</span></span>
<span data-ttu-id="6efb3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6efb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6efb3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6efb3-111">Permission type</span></span>|<span data-ttu-id="6efb3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6efb3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6efb3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6efb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6efb3-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6efb3-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6efb3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6efb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6efb3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6efb3-116">Not supported.</span></span>|
|<span data-ttu-id="6efb3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6efb3-117">Application</span></span>|<span data-ttu-id="6efb3-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6efb3-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6efb3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6efb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6efb3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6efb3-120">Optional query parameters</span></span>
<span data-ttu-id="6efb3-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6efb3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6efb3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6efb3-122">Request headers</span></span>
|<span data-ttu-id="6efb3-123">标头</span><span class="sxs-lookup"><span data-stu-id="6efb3-123">Header</span></span>|<span data-ttu-id="6efb3-124">值</span><span class="sxs-lookup"><span data-stu-id="6efb3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6efb3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6efb3-125">Authorization</span></span>|<span data-ttu-id="6efb3-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6efb3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6efb3-127">接受</span><span class="sxs-lookup"><span data-stu-id="6efb3-127">Accept</span></span>|<span data-ttu-id="6efb3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6efb3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6efb3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6efb3-129">Request body</span></span>
<span data-ttu-id="6efb3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6efb3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6efb3-131">响应</span><span class="sxs-lookup"><span data-stu-id="6efb3-131">Response</span></span>
<span data-ttu-id="6efb3-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6efb3-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6efb3-133">示例</span><span class="sxs-lookup"><span data-stu-id="6efb3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6efb3-134">请求</span><span class="sxs-lookup"><span data-stu-id="6efb3-134">Request</span></span>
<span data-ttu-id="6efb3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6efb3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
```

### <a name="response"></a><span data-ttu-id="6efb3-136">响应</span><span class="sxs-lookup"><span data-stu-id="6efb3-136">Response</span></span>
<span data-ttu-id="6efb3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6efb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
    "id": "7c28e16b-e16b-7c28-6be1-287c6be1287c",
    "osVersion": "Os Version value",
    "osBuildNumber": "Os Build Number value",
    "activeDeviceCount": 1,
    "meanTimeToFailureInMinutes": 10,
    "osVersionAppHealthScore": 7.666666666666667,
    "osVersionAppHealthStatus": "Os Version App Health Status value"
  }
}
```





