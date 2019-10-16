---
title: 列出 deviceManagementAutopilotEvents
description: 列出 deviceManagementAutopilotEvent 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 13103a6beef14c01c541b41882f38d0228239873
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537739"
---
# <a name="list-devicemanagementautopilotevents"></a><span data-ttu-id="3ed54-103">列出 deviceManagementAutopilotEvents</span><span class="sxs-lookup"><span data-stu-id="3ed54-103">List deviceManagementAutopilotEvents</span></span>

> <span data-ttu-id="3ed54-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ed54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ed54-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ed54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ed54-106">列出[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ed54-106">List properties and relationships of the [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ed54-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3ed54-107">Prerequisites</span></span>
<span data-ttu-id="3ed54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ed54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ed54-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ed54-110">Permission type</span></span>|<span data-ttu-id="3ed54-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3ed54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ed54-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ed54-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ed54-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3ed54-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ed54-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ed54-115">Not supported.</span></span>|
|<span data-ttu-id="3ed54-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ed54-116">Application</span></span>|<span data-ttu-id="3ed54-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ed54-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ed54-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ed54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a><span data-ttu-id="3ed54-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ed54-119">Request headers</span></span>
|<span data-ttu-id="3ed54-120">标头</span><span class="sxs-lookup"><span data-stu-id="3ed54-120">Header</span></span>|<span data-ttu-id="3ed54-121">值</span><span class="sxs-lookup"><span data-stu-id="3ed54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ed54-122">授权</span><span class="sxs-lookup"><span data-stu-id="3ed54-122">Authorization</span></span>|<span data-ttu-id="3ed54-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3ed54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ed54-124">接受</span><span class="sxs-lookup"><span data-stu-id="3ed54-124">Accept</span></span>|<span data-ttu-id="3ed54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ed54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ed54-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ed54-126">Request body</span></span>
<span data-ttu-id="3ed54-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ed54-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ed54-128">响应</span><span class="sxs-lookup"><span data-stu-id="3ed54-128">Response</span></span>
<span data-ttu-id="3ed54-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3ed54-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ed54-130">示例</span><span class="sxs-lookup"><span data-stu-id="3ed54-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ed54-131">请求</span><span class="sxs-lookup"><span data-stu-id="3ed54-131">Request</span></span>
<span data-ttu-id="3ed54-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ed54-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
```

### <a name="response"></a><span data-ttu-id="3ed54-133">响应</span><span class="sxs-lookup"><span data-stu-id="3ed54-133">Response</span></span>
<span data-ttu-id="3ed54-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ed54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






