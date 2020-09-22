---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f265c4e8665d607b1bed87e7c61949131877fa99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019115"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="6a8ec-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="6a8ec-103">Update deviceManagement</span></span>

<span data-ttu-id="6a8ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a8ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a8ec-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a8ec-106">更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-106">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a8ec-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a8ec-107">Prerequisites</span></span>
<span data-ttu-id="6a8ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a8ec-110">&nbsp; &nbsp; 工作流)  (的权限类型 &nbsp;</span><span class="sxs-lookup"><span data-stu-id="6a8ec-110">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="6a8ec-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a8ec-111">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="6a8ec-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a8ec-112">Delegated (work or school account)</span></span> |
| <span data-ttu-id="6a8ec-113">&nbsp;&nbsp;审核</span><span class="sxs-lookup"><span data-stu-id="6a8ec-113">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="6a8ec-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-115">&nbsp;&nbsp;公司条款</span><span class="sxs-lookup"><span data-stu-id="6a8ec-115">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="6a8ec-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-117">&nbsp;&nbsp;公司注册</span><span class="sxs-lookup"><span data-stu-id="6a8ec-117">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="6a8ec-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="6a8ec-119">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="6a8ec-119">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="6a8ec-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-121">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="6a8ec-121">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="6a8ec-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-123">&nbsp;&nbsp;Endpoint protection</span><span class="sxs-lookup"><span data-stu-id="6a8ec-123">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="6a8ec-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-125">&nbsp;&nbsp;通知</span><span class="sxs-lookup"><span data-stu-id="6a8ec-125">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="6a8ec-126">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-126">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-127">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="6a8ec-127">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="6a8ec-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-129">&nbsp;&nbsp;基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="6a8ec-129">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="6a8ec-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-130">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-131">&nbsp;&nbsp;远程协助</span><span class="sxs-lookup"><span data-stu-id="6a8ec-131">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="6a8ec-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-133">&nbsp;&nbsp;电信费用管理</span><span class="sxs-lookup"><span data-stu-id="6a8ec-133">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="6a8ec-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-135">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="6a8ec-135">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="6a8ec-136">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-136">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-137">&nbsp;&nbsp;Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="6a8ec-137">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="6a8ec-138">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a8ec-138">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="6a8ec-139">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a8ec-139">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a8ec-140">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-140">Not supported.</span></span>|
| <span data-ttu-id="6a8ec-141">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a8ec-141">Application</span></span> | <span data-ttu-id="6a8ec-142">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-142">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a8ec-143">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a8ec-143">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="6a8ec-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a8ec-144">Request headers</span></span>
|<span data-ttu-id="6a8ec-145">标头</span><span class="sxs-lookup"><span data-stu-id="6a8ec-145">Header</span></span>|<span data-ttu-id="6a8ec-146">值</span><span class="sxs-lookup"><span data-stu-id="6a8ec-146">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a8ec-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a8ec-147">Authorization</span></span>|<span data-ttu-id="6a8ec-148">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-148">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a8ec-149">接受</span><span class="sxs-lookup"><span data-stu-id="6a8ec-149">Accept</span></span>|<span data-ttu-id="6a8ec-150">application/json</span><span class="sxs-lookup"><span data-stu-id="6a8ec-150">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a8ec-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a8ec-151">Request body</span></span>
<span data-ttu-id="6a8ec-152">在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-152">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="6a8ec-153">下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-153">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="6a8ec-154">属性</span><span class="sxs-lookup"><span data-stu-id="6a8ec-154">Property</span></span>|<span data-ttu-id="6a8ec-155">类型</span><span class="sxs-lookup"><span data-stu-id="6a8ec-155">Type</span></span>|<span data-ttu-id="6a8ec-156">说明</span><span class="sxs-lookup"><span data-stu-id="6a8ec-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a8ec-157">id</span><span class="sxs-lookup"><span data-stu-id="6a8ec-157">id</span></span>|<span data-ttu-id="6a8ec-158">String</span><span class="sxs-lookup"><span data-stu-id="6a8ec-158">String</span></span>|<span data-ttu-id="6a8ec-159">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="6a8ec-159">Unique Identifier for the device</span></span>|
|<span data-ttu-id="6a8ec-160">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="6a8ec-160">**Device configuration**</span></span>|
|<span data-ttu-id="6a8ec-161">settings</span><span class="sxs-lookup"><span data-stu-id="6a8ec-161">settings</span></span>|[<span data-ttu-id="6a8ec-162">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6a8ec-162">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="6a8ec-163">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-163">Account level settings.</span></span>|
|<span data-ttu-id="6a8ec-164">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="6a8ec-164">**Device management**</span></span>|
|<span data-ttu-id="6a8ec-165">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="6a8ec-165">subscriptionState</span></span>|[<span data-ttu-id="6a8ec-166">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="6a8ec-166">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="6a8ec-167">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-167">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="6a8ec-168">可取值包括：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-168">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="6a8ec-169">**载入**</span><span class="sxs-lookup"><span data-stu-id="6a8ec-169">**Onboarding**</span></span>|
|<span data-ttu-id="6a8ec-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="6a8ec-170">intuneBrand</span></span>|[<span data-ttu-id="6a8ec-171">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="6a8ec-171">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="6a8ec-172">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-172">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="6a8ec-173">请求正文属性支持因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-173">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="6a8ec-174">响应</span><span class="sxs-lookup"><span data-stu-id="6a8ec-174">Response</span></span>
<span data-ttu-id="6a8ec-175">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-175">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a8ec-176">示例</span><span class="sxs-lookup"><span data-stu-id="6a8ec-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a8ec-177">请求</span><span class="sxs-lookup"><span data-stu-id="6a8ec-177">Request</span></span>
<span data-ttu-id="6a8ec-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a><span data-ttu-id="6a8ec-179">响应</span><span class="sxs-lookup"><span data-stu-id="6a8ec-179">Response</span></span>

<span data-ttu-id="6a8ec-180">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-180">Here is an example of the response.</span></span> <span data-ttu-id="6a8ec-181">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6a8ec-182">返回的属性根据工作流和上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="6a8ec-182">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```









