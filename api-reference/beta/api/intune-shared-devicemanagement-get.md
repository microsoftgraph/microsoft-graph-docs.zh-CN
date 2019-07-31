---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee8e106047073431c64051077a6aa617e03f6b77
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979769"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="ccd46-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ccd46-103">Get deviceManagement</span></span>

> <span data-ttu-id="ccd46-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ccd46-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ccd46-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ccd46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccd46-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ccd46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccd46-107">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ccd46-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccd46-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ccd46-108">Prerequisites</span></span>

<span data-ttu-id="ccd46-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccd46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ccd46-111">权限&nbsp;类型&nbsp;(按&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="ccd46-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="ccd46-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ccd46-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="ccd46-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccd46-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="ccd46-114">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="ccd46-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="ccd46-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ccd46-116">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="ccd46-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="ccd46-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="ccd46-118">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="ccd46-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="ccd46-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ccd46-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="ccd46-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ccd46-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ccd46-122">&nbsp;&nbsp; **设备意向**</span><span class="sxs-lookup"><span data-stu-id="ccd46-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="ccd46-123">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="ccd46-124">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="ccd46-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ccd46-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="ccd46-126">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="ccd46-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="ccd46-127">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ccd46-128">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="ccd46-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ccd46-129">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ccd46-130">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="ccd46-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="ccd46-131">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ccd46-132">&nbsp;&nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="ccd46-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="ccd46-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ccd46-134">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="ccd46-134">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="ccd46-135">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ccd46-136">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="ccd46-136">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ccd46-137">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ccd46-138">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="ccd46-138">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="ccd46-139">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-139">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="ccd46-140">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="ccd46-140">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="ccd46-141">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-141">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ccd46-142">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="ccd46-142">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="ccd46-143">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ccd46-144">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="ccd46-144">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="ccd46-145">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ccd46-146">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="ccd46-146">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ccd46-147">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-147">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="ccd46-148">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="ccd46-148">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="ccd46-149">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd46-149">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="ccd46-150">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccd46-150">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccd46-151">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccd46-151">Not supported.</span></span>|
| <span data-ttu-id="ccd46-152">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccd46-152">Application</span></span> | <span data-ttu-id="ccd46-153">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccd46-153">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="ccd46-154">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccd46-154">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccd46-155">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ccd46-155">Optional query parameters</span></span>

<span data-ttu-id="ccd46-156">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ccd46-156">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccd46-157">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccd46-157">Request headers</span></span>
|<span data-ttu-id="ccd46-158">标头</span><span class="sxs-lookup"><span data-stu-id="ccd46-158">Header</span></span>|<span data-ttu-id="ccd46-159">值</span><span class="sxs-lookup"><span data-stu-id="ccd46-159">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccd46-160">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccd46-160">Authorization</span></span>|<span data-ttu-id="ccd46-161">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ccd46-161">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccd46-162">接受</span><span class="sxs-lookup"><span data-stu-id="ccd46-162">Accept</span></span>|<span data-ttu-id="ccd46-163">application/json</span><span class="sxs-lookup"><span data-stu-id="ccd46-163">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd46-164">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccd46-164">Request body</span></span>

<span data-ttu-id="ccd46-165">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ccd46-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccd46-166">响应</span><span class="sxs-lookup"><span data-stu-id="ccd46-166">Response</span></span>

<span data-ttu-id="ccd46-167">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ccd46-167">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd46-168">示例</span><span class="sxs-lookup"><span data-stu-id="ccd46-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccd46-169">请求</span><span class="sxs-lookup"><span data-stu-id="ccd46-169">Request</span></span>

<span data-ttu-id="ccd46-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ccd46-170">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="ccd46-171">响应</span><span class="sxs-lookup"><span data-stu-id="ccd46-171">Response</span></span>

<span data-ttu-id="ccd46-172">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="ccd46-172">Here are example of the response.</span></span> 

<span data-ttu-id="ccd46-173">注意: 为简洁起见, 可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ccd46-173">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="ccd46-174">将返回适用于工作流的属性。</span><span class="sxs-lookup"><span data-stu-id="ccd46-174">Properties appropriate for the workflow are returned.</span></span>

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



