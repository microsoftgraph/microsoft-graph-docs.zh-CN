---
title: 列出 deviceHealthScriptDeviceStates
description: 列出 deviceHealthScriptDeviceState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c34e8d285794afa182fc3bf5d566439293707974
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732794"
---
# <a name="list-devicehealthscriptdevicestates"></a><span data-ttu-id="7a21e-103">列出 deviceHealthScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="7a21e-103">List deviceHealthScriptDeviceStates</span></span>

<span data-ttu-id="7a21e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a21e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a21e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a21e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a21e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a21e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a21e-107">列出 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a21e-107">List properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a21e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7a21e-108">Prerequisites</span></span>
<span data-ttu-id="7a21e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a21e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a21e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a21e-111">Permission type</span></span>|<span data-ttu-id="7a21e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7a21e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a21e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a21e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a21e-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a21e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7a21e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a21e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a21e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a21e-116">Not supported.</span></span>|
|<span data-ttu-id="7a21e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a21e-117">Application</span></span>|<span data-ttu-id="7a21e-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a21e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a21e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a21e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="7a21e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a21e-120">Request headers</span></span>
|<span data-ttu-id="7a21e-121">标头</span><span class="sxs-lookup"><span data-stu-id="7a21e-121">Header</span></span>|<span data-ttu-id="7a21e-122">值</span><span class="sxs-lookup"><span data-stu-id="7a21e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a21e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a21e-123">Authorization</span></span>|<span data-ttu-id="7a21e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7a21e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a21e-125">接受</span><span class="sxs-lookup"><span data-stu-id="7a21e-125">Accept</span></span>|<span data-ttu-id="7a21e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a21e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a21e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a21e-127">Request body</span></span>
<span data-ttu-id="7a21e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a21e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a21e-129">响应</span><span class="sxs-lookup"><span data-stu-id="7a21e-129">Response</span></span>
<span data-ttu-id="7a21e-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7a21e-130">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a21e-131">示例</span><span class="sxs-lookup"><span data-stu-id="7a21e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a21e-132">请求</span><span class="sxs-lookup"><span data-stu-id="7a21e-132">Request</span></span>
<span data-ttu-id="7a21e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a21e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="7a21e-134">响应</span><span class="sxs-lookup"><span data-stu-id="7a21e-134">Response</span></span>
<span data-ttu-id="7a21e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a21e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 892

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
      "id": "fd2e4505-4505-fd2e-0545-2efd05452efd",
      "detectionState": "success",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
      "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
      "remediationScriptError": "Remediation Script Error value",
      "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
      "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
      "remediationState": "skipped"
    }
  ]
}
```





