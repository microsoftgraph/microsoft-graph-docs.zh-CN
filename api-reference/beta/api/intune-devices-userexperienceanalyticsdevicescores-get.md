---
title: 获取 userExperienceAnalyticsDeviceScores
description: 读取 userExperienceAnalyticsDeviceScores 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11114c40aa29de5c78283d065c30355a46fbea1f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868475"
---
# <a name="get-userexperienceanalyticsdevicescores"></a><span data-ttu-id="13581-103">获取 userExperienceAnalyticsDeviceScores</span><span class="sxs-lookup"><span data-stu-id="13581-103">Get userExperienceAnalyticsDeviceScores</span></span>

<span data-ttu-id="13581-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13581-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13581-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13581-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13581-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13581-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13581-107">读取 [userExperienceAnalyticsDeviceScores 对象的属性和](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="13581-107">Read properties and relationships of the [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13581-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="13581-108">Prerequisites</span></span>
<span data-ttu-id="13581-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13581-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="13581-111">Permission type</span></span>|<span data-ttu-id="13581-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13581-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13581-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13581-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13581-114">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13581-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13581-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13581-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13581-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="13581-116">Not supported.</span></span>|
|<span data-ttu-id="13581-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="13581-117">Application</span></span>|<span data-ttu-id="13581-118">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13581-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13581-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13581-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13581-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="13581-120">Optional query parameters</span></span>
<span data-ttu-id="13581-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="13581-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13581-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="13581-122">Request headers</span></span>
|<span data-ttu-id="13581-123">标头</span><span class="sxs-lookup"><span data-stu-id="13581-123">Header</span></span>|<span data-ttu-id="13581-124">值</span><span class="sxs-lookup"><span data-stu-id="13581-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13581-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="13581-125">Authorization</span></span>|<span data-ttu-id="13581-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="13581-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13581-127">接受</span><span class="sxs-lookup"><span data-stu-id="13581-127">Accept</span></span>|<span data-ttu-id="13581-128">application/json</span><span class="sxs-lookup"><span data-stu-id="13581-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13581-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="13581-129">Request body</span></span>
<span data-ttu-id="13581-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13581-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13581-131">响应</span><span class="sxs-lookup"><span data-stu-id="13581-131">Response</span></span>
<span data-ttu-id="13581-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13581-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13581-133">示例</span><span class="sxs-lookup"><span data-stu-id="13581-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="13581-134">请求</span><span class="sxs-lookup"><span data-stu-id="13581-134">Request</span></span>
<span data-ttu-id="13581-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13581-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
```

### <a name="response"></a><span data-ttu-id="13581-136">响应</span><span class="sxs-lookup"><span data-stu-id="13581-136">Response</span></span>
<span data-ttu-id="13581-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="13581-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
    "id": "0dd9f6cf-f6cf-0dd9-cff6-d90dcff6d90d",
    "deviceName": "Device Name value",
    "model": "Model value",
    "manufacturer": "Manufacturer value",
    "endpointAnalyticsScore": 7.333333333333333,
    "startupPerformanceScore": 7.666666666666667,
    "appReliabilityScore": 6.333333333333333
  }
}
```




