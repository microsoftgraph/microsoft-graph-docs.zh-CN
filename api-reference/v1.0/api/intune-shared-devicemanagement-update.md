---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b845a07d8199fcd4a997304f9095d7b364e0988a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023431"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="1e838-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="1e838-103">Update deviceManagement</span></span>

> <span data-ttu-id="1e838-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e838-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e838-105">更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1e838-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e838-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e838-106">Prerequisites</span></span>
<span data-ttu-id="1e838-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e838-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e838-109">权限&nbsp;类型&nbsp;(按&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="1e838-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="1e838-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e838-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="1e838-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e838-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="1e838-112">&nbsp;&nbsp;审核</span><span class="sxs-lookup"><span data-stu-id="1e838-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="1e838-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-114">&nbsp;&nbsp;公司条款</span><span class="sxs-lookup"><span data-stu-id="1e838-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="1e838-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-116">&nbsp;&nbsp;公司注册</span><span class="sxs-lookup"><span data-stu-id="1e838-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="1e838-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="1e838-118">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="1e838-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="1e838-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-120">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="1e838-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="1e838-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-122">&nbsp;&nbsp; Endpoint protection</span><span class="sxs-lookup"><span data-stu-id="1e838-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="1e838-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-124">&nbsp;&nbsp;通知</span><span class="sxs-lookup"><span data-stu-id="1e838-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="1e838-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-126">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="1e838-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="1e838-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-128">&nbsp;&nbsp;基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="1e838-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="1e838-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-130">&nbsp;&nbsp;远程协助</span><span class="sxs-lookup"><span data-stu-id="1e838-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="1e838-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-132">&nbsp;&nbsp;电信费用管理</span><span class="sxs-lookup"><span data-stu-id="1e838-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="1e838-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-134">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="1e838-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="1e838-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-136">&nbsp;&nbsp; Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="1e838-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="1e838-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e838-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="1e838-138">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e838-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e838-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e838-139">Not supported.</span></span>|
| <span data-ttu-id="1e838-140">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e838-140">Application</span></span> | <span data-ttu-id="1e838-141">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e838-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e838-142">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e838-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="1e838-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e838-143">Request headers</span></span>
|<span data-ttu-id="1e838-144">标头</span><span class="sxs-lookup"><span data-stu-id="1e838-144">Header</span></span>|<span data-ttu-id="1e838-145">值</span><span class="sxs-lookup"><span data-stu-id="1e838-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e838-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e838-146">Authorization</span></span>|<span data-ttu-id="1e838-147">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e838-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e838-148">接受</span><span class="sxs-lookup"><span data-stu-id="1e838-148">Accept</span></span>|<span data-ttu-id="1e838-149">application/json</span><span class="sxs-lookup"><span data-stu-id="1e838-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e838-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e838-150">Request body</span></span>
<span data-ttu-id="1e838-151">在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e838-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="1e838-152">下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1e838-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="1e838-153">属性</span><span class="sxs-lookup"><span data-stu-id="1e838-153">Property</span></span>|<span data-ttu-id="1e838-154">类型</span><span class="sxs-lookup"><span data-stu-id="1e838-154">Type</span></span>|<span data-ttu-id="1e838-155">说明</span><span class="sxs-lookup"><span data-stu-id="1e838-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e838-156">id</span><span class="sxs-lookup"><span data-stu-id="1e838-156">id</span></span>|<span data-ttu-id="1e838-157">String</span><span class="sxs-lookup"><span data-stu-id="1e838-157">String</span></span>|<span data-ttu-id="1e838-158">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="1e838-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="1e838-159">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="1e838-159">**Device configuration**</span></span>|
|<span data-ttu-id="1e838-160">settings</span><span class="sxs-lookup"><span data-stu-id="1e838-160">settings</span></span>|[<span data-ttu-id="1e838-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="1e838-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="1e838-162">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="1e838-162">Account level settings.</span></span>|
|<span data-ttu-id="1e838-163">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="1e838-163">**Device management**</span></span>|
|<span data-ttu-id="1e838-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="1e838-164">subscriptionState</span></span>|[<span data-ttu-id="1e838-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="1e838-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="1e838-166">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="1e838-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="1e838-167">可取值包括：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="1e838-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="1e838-168">**载入**</span><span class="sxs-lookup"><span data-stu-id="1e838-168">**Onboarding**</span></span>|
|<span data-ttu-id="1e838-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="1e838-169">intuneBrand</span></span>|[<span data-ttu-id="1e838-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="1e838-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="1e838-171">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="1e838-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="1e838-172">请求正文属性支持因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="1e838-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="1e838-173">响应</span><span class="sxs-lookup"><span data-stu-id="1e838-173">Response</span></span>
<span data-ttu-id="1e838-174">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e838-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e838-175">示例</span><span class="sxs-lookup"><span data-stu-id="1e838-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e838-176">请求</span><span class="sxs-lookup"><span data-stu-id="1e838-176">Request</span></span>
<span data-ttu-id="1e838-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e838-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e838-178">响应</span><span class="sxs-lookup"><span data-stu-id="1e838-178">Response</span></span>

<span data-ttu-id="1e838-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1e838-179">Here is an example of the response.</span></span> <span data-ttu-id="1e838-180">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e838-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1e838-181">返回的属性根据工作流和上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="1e838-181">Returned properties vary according to workflow and context.</span></span>

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



