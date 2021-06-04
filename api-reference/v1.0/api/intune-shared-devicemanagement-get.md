---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7fccbc17390e9cd481c2fd06af09ba5681a1e56
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732416"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="6011c-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6011c-103">Get deviceManagement</span></span>

<span data-ttu-id="6011c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6011c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6011c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6011c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6011c-106">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6011c-106">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6011c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6011c-107">Prerequisites</span></span>
<span data-ttu-id="6011c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6011c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6011c-110">工作流 &nbsp; &nbsp; (的权限 &nbsp; 类型) </span><span class="sxs-lookup"><span data-stu-id="6011c-110">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="6011c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6011c-111">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="6011c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6011c-112">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="6011c-113">&nbsp;&nbsp;审核</span><span class="sxs-lookup"><span data-stu-id="6011c-113">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="6011c-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="6011c-115">&nbsp;&nbsp;公司条款</span><span class="sxs-lookup"><span data-stu-id="6011c-115">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="6011c-116">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6011c-117">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="6011c-117">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="6011c-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="6011c-119">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="6011c-119">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="6011c-120">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="6011c-121">&nbsp;&nbsp;注册</span><span class="sxs-lookup"><span data-stu-id="6011c-121">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="6011c-122">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6011c-123">&nbsp;&nbsp;通知</span><span class="sxs-lookup"><span data-stu-id="6011c-123">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="6011c-124">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6011c-125">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="6011c-125">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="6011c-126">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-126">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6011c-127">&nbsp;&nbsp;RBAC</span><span class="sxs-lookup"><span data-stu-id="6011c-127">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="6011c-128">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-128">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="6011c-129">&nbsp;&nbsp;远程协助</span><span class="sxs-lookup"><span data-stu-id="6011c-129">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="6011c-130">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6011c-131">&nbsp;&nbsp;电信费用管理</span><span class="sxs-lookup"><span data-stu-id="6011c-131">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="6011c-132">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="6011c-133">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="6011c-133">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="6011c-134">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="6011c-135">&nbsp;&nbsp;Windows信息保护</span><span class="sxs-lookup"><span data-stu-id="6011c-135">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="6011c-136">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6011c-136">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="6011c-137">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6011c-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6011c-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="6011c-138">Not supported.</span></span>|
| <span data-ttu-id="6011c-139">应用程序</span><span class="sxs-lookup"><span data-stu-id="6011c-139">Application</span></span> | <span data-ttu-id="6011c-140">不支持。</span><span class="sxs-lookup"><span data-stu-id="6011c-140">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="6011c-141">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6011c-141">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6011c-142">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6011c-142">Optional query parameters</span></span>
<span data-ttu-id="6011c-143">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6011c-143">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6011c-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="6011c-144">Request headers</span></span>
|<span data-ttu-id="6011c-145">标头</span><span class="sxs-lookup"><span data-stu-id="6011c-145">Header</span></span>|<span data-ttu-id="6011c-146">值</span><span class="sxs-lookup"><span data-stu-id="6011c-146">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6011c-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="6011c-147">Authorization</span></span>|<span data-ttu-id="6011c-148">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6011c-148">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6011c-149">接受</span><span class="sxs-lookup"><span data-stu-id="6011c-149">Accept</span></span>|<span data-ttu-id="6011c-150">application/json</span><span class="sxs-lookup"><span data-stu-id="6011c-150">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6011c-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="6011c-151">Request body</span></span>
<span data-ttu-id="6011c-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6011c-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6011c-153">响应</span><span class="sxs-lookup"><span data-stu-id="6011c-153">Response</span></span>
<span data-ttu-id="6011c-154">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6011c-154">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6011c-155">示例</span><span class="sxs-lookup"><span data-stu-id="6011c-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="6011c-156">请求</span><span class="sxs-lookup"><span data-stu-id="6011c-156">Request</span></span>
<span data-ttu-id="6011c-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6011c-157">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="6011c-158">响应</span><span class="sxs-lookup"><span data-stu-id="6011c-158">Response</span></span>
<span data-ttu-id="6011c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6011c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```