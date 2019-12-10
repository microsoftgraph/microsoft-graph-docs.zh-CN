---
title: 获取 deviceManagementAutopilotEvent
description: 读取 deviceManagementAutopilotEvent 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6fecd5746417e0907feb39a7fa231528153a3f6a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939027"
---
# <a name="get-devicemanagementautopilotevent"></a><span data-ttu-id="4a622-103">获取 deviceManagementAutopilotEvent</span><span class="sxs-lookup"><span data-stu-id="4a622-103">Get deviceManagementAutopilotEvent</span></span>

> <span data-ttu-id="4a622-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a622-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a622-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a622-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a622-106">读取[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a622-106">Read properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a622-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4a622-107">Prerequisites</span></span>
<span data-ttu-id="4a622-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a622-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a622-110">Permission type</span></span>|<span data-ttu-id="4a622-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4a622-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a622-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a622-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a622-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a622-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4a622-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a622-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a622-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a622-115">Not supported.</span></span>|
|<span data-ttu-id="4a622-116">Application</span><span class="sxs-lookup"><span data-stu-id="4a622-116">Application</span></span>|<span data-ttu-id="4a622-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a622-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a622-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a622-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a622-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4a622-119">Optional query parameters</span></span>
<span data-ttu-id="4a622-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4a622-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a622-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a622-121">Request headers</span></span>
|<span data-ttu-id="4a622-122">标头</span><span class="sxs-lookup"><span data-stu-id="4a622-122">Header</span></span>|<span data-ttu-id="4a622-123">值</span><span class="sxs-lookup"><span data-stu-id="4a622-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a622-124">授权</span><span class="sxs-lookup"><span data-stu-id="4a622-124">Authorization</span></span>|<span data-ttu-id="4a622-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4a622-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a622-126">接受</span><span class="sxs-lookup"><span data-stu-id="4a622-126">Accept</span></span>|<span data-ttu-id="4a622-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4a622-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a622-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a622-128">Request body</span></span>
<span data-ttu-id="4a622-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a622-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a622-130">响应</span><span class="sxs-lookup"><span data-stu-id="4a622-130">Response</span></span>
<span data-ttu-id="4a622-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4a622-131">If successful, this method returns a `200 OK` response code and [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a622-132">示例</span><span class="sxs-lookup"><span data-stu-id="4a622-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a622-133">请求</span><span class="sxs-lookup"><span data-stu-id="4a622-133">Request</span></span>
<span data-ttu-id="4a622-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a622-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}
```

### <a name="response"></a><span data-ttu-id="4a622-135">响应</span><span class="sxs-lookup"><span data-stu-id="4a622-135">Response</span></span>
<span data-ttu-id="4a622-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4a622-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
    "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
    "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
    "enrollmentType": "azureADJoinedWithAutopilotProfile",
    "deviceSerialNumber": "Device Serial Number value",
    "managedDeviceName": "Managed Device Name value",
    "userPrincipalName": "User Principal Name value",
    "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
    "enrollmentState": "enrolled",
    "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
    "deploymentState": "success",
    "osVersion": "Os Version value",
    "deploymentDuration": "PT3M21.5549443S",
    "deploymentTotalDuration": "PT1M43.5284261S",
    "devicePreparationDuration": "-PT1M32.1347897S",
    "deviceSetupDuration": "-PT2M57.2190107S",
    "accountSetupDuration": "-PT2M32.0507894S",
    "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
    "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
    "targetedAppCount": 0,
    "targetedPolicyCount": 3,
    "enrollmentFailureDetails": "Enrollment Failure Details value"
  }
}
```





