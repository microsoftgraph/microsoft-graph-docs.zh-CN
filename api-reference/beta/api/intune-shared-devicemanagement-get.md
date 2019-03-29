---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09563eeced6f557df2c2e40f126623f974cea2d7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976503"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="3604b-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3604b-103">Get deviceManagement</span></span>

> <span data-ttu-id="3604b-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3604b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3604b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3604b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3604b-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3604b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3604b-107">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3604b-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3604b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3604b-108">Prerequisites</span></span>

<span data-ttu-id="3604b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3604b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3604b-111">权限&nbsp;类型&nbsp;(按&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="3604b-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="3604b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3604b-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="3604b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3604b-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="3604b-114">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="3604b-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="3604b-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="3604b-116">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="3604b-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="3604b-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="3604b-118">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="3604b-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="3604b-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3604b-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="3604b-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3604b-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="3604b-122">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="3604b-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3604b-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="3604b-124">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="3604b-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="3604b-125">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="3604b-126">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="3604b-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="3604b-127">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3604b-128">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="3604b-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="3604b-129">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="3604b-130">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="3604b-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="3604b-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3604b-132">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="3604b-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3604b-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3604b-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="3604b-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="3604b-135">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="3604b-136">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="3604b-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="3604b-137">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="3604b-138">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="3604b-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="3604b-139">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3604b-140">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="3604b-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="3604b-141">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3604b-142">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="3604b-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3604b-143">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="3604b-144">&nbsp;&nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="3604b-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="3604b-145">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3604b-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="3604b-146">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3604b-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3604b-147">不支持。</span><span class="sxs-lookup"><span data-stu-id="3604b-147">Not supported.</span></span>|
| <span data-ttu-id="3604b-148">应用程序</span><span class="sxs-lookup"><span data-stu-id="3604b-148">Application</span></span> | <span data-ttu-id="3604b-149">不支持。</span><span class="sxs-lookup"><span data-stu-id="3604b-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="3604b-150">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3604b-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3604b-151">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3604b-151">Optional query parameters</span></span>

<span data-ttu-id="3604b-152">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3604b-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3604b-153">请求标头</span><span class="sxs-lookup"><span data-stu-id="3604b-153">Request headers</span></span>
|<span data-ttu-id="3604b-154">标头</span><span class="sxs-lookup"><span data-stu-id="3604b-154">Header</span></span>|<span data-ttu-id="3604b-155">值</span><span class="sxs-lookup"><span data-stu-id="3604b-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3604b-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="3604b-156">Authorization</span></span>|<span data-ttu-id="3604b-157">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3604b-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3604b-158">接受</span><span class="sxs-lookup"><span data-stu-id="3604b-158">Accept</span></span>|<span data-ttu-id="3604b-159">application/json</span><span class="sxs-lookup"><span data-stu-id="3604b-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3604b-160">请求正文</span><span class="sxs-lookup"><span data-stu-id="3604b-160">Request body</span></span>

<span data-ttu-id="3604b-161">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3604b-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3604b-162">响应</span><span class="sxs-lookup"><span data-stu-id="3604b-162">Response</span></span>

<span data-ttu-id="3604b-163">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3604b-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3604b-164">示例</span><span class="sxs-lookup"><span data-stu-id="3604b-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="3604b-165">请求</span><span class="sxs-lookup"><span data-stu-id="3604b-165">Request</span></span>

<span data-ttu-id="3604b-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3604b-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="3604b-167">响应</span><span class="sxs-lookup"><span data-stu-id="3604b-167">Response</span></span>

<span data-ttu-id="3604b-168">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="3604b-168">Here are example of the response.</span></span> 

<span data-ttu-id="3604b-169">注意: 为简洁起见, 可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3604b-169">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="3604b-170">将返回适用于工作流的属性。</span><span class="sxs-lookup"><span data-stu-id="3604b-170">Properties appropriate for the workflow are returned.</span></span>

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



