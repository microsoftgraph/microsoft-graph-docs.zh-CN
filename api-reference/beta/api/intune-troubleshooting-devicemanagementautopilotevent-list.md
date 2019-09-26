---
title: 列出 deviceManagementAutopilotEvents
description: 列出 deviceManagementAutopilotEvent 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 709fc30929119e42856f92a460944aaf4992d81a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199808"
---
# <a name="list-devicemanagementautopilotevents"></a><span data-ttu-id="d0642-103">列出 deviceManagementAutopilotEvents</span><span class="sxs-lookup"><span data-stu-id="d0642-103">List deviceManagementAutopilotEvents</span></span>

> <span data-ttu-id="d0642-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0642-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0642-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0642-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0642-106">列出[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0642-106">List properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0642-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0642-107">Prerequisites</span></span>
<span data-ttu-id="d0642-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0642-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0642-110">Permission type</span></span>|<span data-ttu-id="d0642-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d0642-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0642-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0642-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0642-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0642-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d0642-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0642-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0642-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0642-115">Not supported.</span></span>|
|<span data-ttu-id="d0642-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0642-116">Application</span></span>|<span data-ttu-id="d0642-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0642-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0642-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0642-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="d0642-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0642-119">Request headers</span></span>
|<span data-ttu-id="d0642-120">标头</span><span class="sxs-lookup"><span data-stu-id="d0642-120">Header</span></span>|<span data-ttu-id="d0642-121">值</span><span class="sxs-lookup"><span data-stu-id="d0642-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0642-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0642-122">Authorization</span></span>|<span data-ttu-id="d0642-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0642-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0642-124">接受</span><span class="sxs-lookup"><span data-stu-id="d0642-124">Accept</span></span>|<span data-ttu-id="d0642-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0642-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0642-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0642-126">Request body</span></span>
<span data-ttu-id="d0642-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0642-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0642-128">响应</span><span class="sxs-lookup"><span data-stu-id="d0642-128">Response</span></span>
<span data-ttu-id="d0642-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d0642-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0642-130">示例</span><span class="sxs-lookup"><span data-stu-id="d0642-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0642-131">请求</span><span class="sxs-lookup"><span data-stu-id="d0642-131">Request</span></span>
<span data-ttu-id="d0642-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0642-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
```

### <a name="response"></a><span data-ttu-id="d0642-133">响应</span><span class="sxs-lookup"><span data-stu-id="d0642-133">Response</span></span>
<span data-ttu-id="d0642-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0642-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1501

{
  "value": [
    {
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
  ]
}
```




