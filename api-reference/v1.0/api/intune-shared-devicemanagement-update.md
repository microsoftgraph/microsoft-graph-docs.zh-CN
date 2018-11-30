---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
ms.openlocfilehash: f63e9b717f912e255abccedf809772590eb44d1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008820"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="5de9f-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5de9f-103">Update deviceManagement</span></span>

> <span data-ttu-id="5de9f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5de9f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5de9f-105">更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5de9f-105">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5de9f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5de9f-106">Prerequisites</span></span>
<span data-ttu-id="5de9f-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5de9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5de9f-109">权限&nbsp;类型&nbsp;(通过&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="5de9f-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="5de9f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5de9f-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="5de9f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5de9f-111">Delegated (work or school account)</span></span> |
| <span data-ttu-id="5de9f-112">&nbsp;&nbsp;审核</span><span class="sxs-lookup"><span data-stu-id="5de9f-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="5de9f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-113">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-114">&nbsp;&nbsp;公司术语</span><span class="sxs-lookup"><span data-stu-id="5de9f-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="5de9f-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-115">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-116">&nbsp;&nbsp;公司注册</span><span class="sxs-lookup"><span data-stu-id="5de9f-116">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="5de9f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="5de9f-118">&nbsp;&nbsp;设备配置</span><span class="sxs-lookup"><span data-stu-id="5de9f-118">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="5de9f-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-119">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-120">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="5de9f-120">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="5de9f-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-122">&nbsp;&nbsp;终结点保护</span><span class="sxs-lookup"><span data-stu-id="5de9f-122">&nbsp; &nbsp; Endpoint protection</span></span> | <span data-ttu-id="5de9f-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-123">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-124">&nbsp;&nbsp;通知</span><span class="sxs-lookup"><span data-stu-id="5de9f-124">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="5de9f-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-125">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-126">&nbsp;&nbsp;入职培训</span><span class="sxs-lookup"><span data-stu-id="5de9f-126">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="5de9f-127">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-127">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-128">&nbsp;&nbsp;基于角色的访问控制</span><span class="sxs-lookup"><span data-stu-id="5de9f-128">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="5de9f-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-129">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-130">&nbsp;&nbsp;远程协助</span><span class="sxs-lookup"><span data-stu-id="5de9f-130">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="5de9f-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-132">&nbsp;&nbsp;电信支出管理</span><span class="sxs-lookup"><span data-stu-id="5de9f-132">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="5de9f-133">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-133">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-134">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="5de9f-134">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="5de9f-135">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-135">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-136">&nbsp;&nbsp; Windows 信息保护</span><span class="sxs-lookup"><span data-stu-id="5de9f-136">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="5de9f-137">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de9f-137">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="5de9f-138">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5de9f-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5de9f-139">不支持。</span><span class="sxs-lookup"><span data-stu-id="5de9f-139">Not supported.</span></span>|
| <span data-ttu-id="5de9f-140">应用程序</span><span class="sxs-lookup"><span data-stu-id="5de9f-140">Application</span></span> | <span data-ttu-id="5de9f-141">不支持。</span><span class="sxs-lookup"><span data-stu-id="5de9f-141">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5de9f-142">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5de9f-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="5de9f-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="5de9f-143">Request headers</span></span>
|<span data-ttu-id="5de9f-144">标头</span><span class="sxs-lookup"><span data-stu-id="5de9f-144">Header</span></span>|<span data-ttu-id="5de9f-145">值</span><span class="sxs-lookup"><span data-stu-id="5de9f-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5de9f-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="5de9f-146">Authorization</span></span>|<span data-ttu-id="5de9f-147">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5de9f-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5de9f-148">Accept</span><span class="sxs-lookup"><span data-stu-id="5de9f-148">Accept</span></span>|<span data-ttu-id="5de9f-149">application/json</span><span class="sxs-lookup"><span data-stu-id="5de9f-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5de9f-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="5de9f-150">Request body</span></span>
<span data-ttu-id="5de9f-151">在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5de9f-151">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="5de9f-152">下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5de9f-152">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="5de9f-153">属性</span><span class="sxs-lookup"><span data-stu-id="5de9f-153">Property</span></span>|<span data-ttu-id="5de9f-154">类型</span><span class="sxs-lookup"><span data-stu-id="5de9f-154">Type</span></span>|<span data-ttu-id="5de9f-155">说明</span><span class="sxs-lookup"><span data-stu-id="5de9f-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5de9f-156">id</span><span class="sxs-lookup"><span data-stu-id="5de9f-156">id</span></span>|<span data-ttu-id="5de9f-157">String</span><span class="sxs-lookup"><span data-stu-id="5de9f-157">String</span></span>|<span data-ttu-id="5de9f-158">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="5de9f-158">Unique Identifier for the device</span></span>|
|<span data-ttu-id="5de9f-159">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="5de9f-159">**Device configuration**</span></span>|
|<span data-ttu-id="5de9f-160">settings</span><span class="sxs-lookup"><span data-stu-id="5de9f-160">settings</span></span>|[<span data-ttu-id="5de9f-161">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="5de9f-161">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="5de9f-162">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="5de9f-162">Account level settings.</span></span>|
|<span data-ttu-id="5de9f-163">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="5de9f-163">**Device management**</span></span>|
|<span data-ttu-id="5de9f-164">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="5de9f-164">subscriptionState</span></span>|[<span data-ttu-id="5de9f-165">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="5de9f-165">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="5de9f-166">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="5de9f-166">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="5de9f-167">可能的值为： `pending`， `active`， `warning`， `disabled`， `deleted`， `blocked`， `lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="5de9f-167">The possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="5de9f-168">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="5de9f-168">**Onboarding**</span></span>|
|<span data-ttu-id="5de9f-169">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="5de9f-169">intuneBrand</span></span>|[<span data-ttu-id="5de9f-170">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="5de9f-170">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="5de9f-171">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="5de9f-171">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="5de9f-172">请求正文属性支持根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="5de9f-172">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="5de9f-173">响应</span><span class="sxs-lookup"><span data-stu-id="5de9f-173">Response</span></span>
<span data-ttu-id="5de9f-174">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5de9f-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5de9f-175">示例</span><span class="sxs-lookup"><span data-stu-id="5de9f-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5de9f-176">请求</span><span class="sxs-lookup"><span data-stu-id="5de9f-176">Request</span></span>
<span data-ttu-id="5de9f-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5de9f-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5de9f-178">响应</span><span class="sxs-lookup"><span data-stu-id="5de9f-178">Response</span></span>

<span data-ttu-id="5de9f-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5de9f-179">Here is an example of the response.</span></span> <span data-ttu-id="5de9f-180">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5de9f-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5de9f-181">返回的属性根据工作流和上下文而有所不同。</span><span class="sxs-lookup"><span data-stu-id="5de9f-181">Returned properties vary according to workflow and context.</span></span>

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



