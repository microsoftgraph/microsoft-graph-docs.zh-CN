---
title: 获取 deviceHealthScriptDeviceState
description: 读取 deviceHealthScriptDeviceState 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d065d50bb8a8af1e9fb27bd8aee8bf4d8263d01
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762988"
---
# <a name="get-devicehealthscriptdevicestate"></a><span data-ttu-id="22ccf-103">获取 deviceHealthScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="22ccf-103">Get deviceHealthScriptDeviceState</span></span>

> <span data-ttu-id="22ccf-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22ccf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22ccf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22ccf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22ccf-106">读取[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22ccf-106">Read properties and relationships of the [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22ccf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="22ccf-107">Prerequisites</span></span>
<span data-ttu-id="22ccf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22ccf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="22ccf-110">Permission type</span></span>|<span data-ttu-id="22ccf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="22ccf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22ccf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22ccf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22ccf-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22ccf-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22ccf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22ccf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22ccf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="22ccf-115">Not supported.</span></span>|
|<span data-ttu-id="22ccf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="22ccf-116">Application</span></span>|<span data-ttu-id="22ccf-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22ccf-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22ccf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22ccf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22ccf-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="22ccf-119">Optional query parameters</span></span>
<span data-ttu-id="22ccf-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22ccf-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22ccf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="22ccf-121">Request headers</span></span>
|<span data-ttu-id="22ccf-122">标头</span><span class="sxs-lookup"><span data-stu-id="22ccf-122">Header</span></span>|<span data-ttu-id="22ccf-123">值</span><span class="sxs-lookup"><span data-stu-id="22ccf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22ccf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="22ccf-124">Authorization</span></span>|<span data-ttu-id="22ccf-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="22ccf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22ccf-126">接受</span><span class="sxs-lookup"><span data-stu-id="22ccf-126">Accept</span></span>|<span data-ttu-id="22ccf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="22ccf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22ccf-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="22ccf-128">Request body</span></span>
<span data-ttu-id="22ccf-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22ccf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22ccf-130">响应</span><span class="sxs-lookup"><span data-stu-id="22ccf-130">Response</span></span>
<span data-ttu-id="22ccf-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="22ccf-131">If successful, this method returns a `200 OK` response code and [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22ccf-132">示例</span><span class="sxs-lookup"><span data-stu-id="22ccf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="22ccf-133">请求</span><span class="sxs-lookup"><span data-stu-id="22ccf-133">Request</span></span>
<span data-ttu-id="22ccf-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22ccf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="22ccf-135">响应</span><span class="sxs-lookup"><span data-stu-id="22ccf-135">Response</span></span>
<span data-ttu-id="22ccf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22ccf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "value": {
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
}
```




